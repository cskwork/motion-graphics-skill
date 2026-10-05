# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static HTML/CSS/JS served by GitHub Pages from `main` at the repository root (inferred from the owner's other skill repos, cskwork/skills and cskwork/context-diet-skill, which ship the same way). No build step.

## Users

Developers and indie makers who work with coding agents (Claude Code, Codex, other agents that read SKILL.md). They arrive from GitHub, X, or the cskwork/skills collection, usually on a desktop, deciding whether to install the skill. Secondary: creators who want YouTube Shorts made by an agent.

## Product Purpose

`motion-graphics` is an agent skill that makes motion-graphics videos in code. Two formats: a keynote-style product launch video built from real captures of the user's running app (iOS Simulator, Android emulator, web, macOS), and vertical shorts for YouTube Shorts, Reels, and TikTok. Success for the landing page: a visitor sees the engine work and copies the install command.

## Positioning

A video is one HTML page where every pixel is a pure function of time `t`; a bundled engine renders it frame by frame in headless Chromium and encodes with ffmpeg. The agent writes the video like code, so it is reproducible, reviewable, and needs no editing app. Launch videos show only real captured UI of the product, never invented screens.

## Operating Context

Installed with `npx skills@latest add cskwork/motion-graphics-skill` or from `cskwork/skills`. The agent works in a per-video folder: brief, beat sheet, assets manifest, `motion.html`, `motion.json`, engine copy, renders. QA uses stills at beat times and an ffmpeg contact sheet.

## Capabilities and Constraints

- Engine: `runtime.js` (scenes, springs, tweens, kinetic type split, deterministic noise, frame-accurate screen-recording clips), `render.mjs` (parallel Playwright workers, H.264 output, stills mode).
- Formats: launch video default 30 s, 1920×1080, 60 fps; shorts default 20–30 s, 1080×1920.
- Requires Node.js 18+, ffmpeg, Playwright Chromium.
- Audio only from licensed or user-supplied files; otherwise silent.
- MIT license.

## Brand Commitments

Owner directive (2026-10-05): the landing page must contain an actual motion graphic introducing the skill, and the page itself is designed with impeccable.

## Evidence on Hand

- Live demo compositions in `demo/` run on the skill's own engine (authored for this page; they show the skill, not customer work).
- No testimonials, users, download counts, or benchmarks exist. Do not invent them.
- Measured render speed from the owner's own production notes: about 10–11 minutes for a 25 s 1080p60 render with 4 workers.

## Product Principles

1. Show the engine working; never describe what a visitor could watch instead.
2. Real material only: real captures in videos, real commands and code on the page.
3. Determinism is the product: same `t`, same frame.
4. Craft bar of a senior motion designer's showreel, not a slideshow.
