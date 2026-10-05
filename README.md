# motion-graphics-skill

An agent skill that makes motion-graphics videos in code: product launch videos built from your real running app, and vertical shorts for YouTube Shorts, Reels, and TikTok. Works with Claude Code, Codex, and any agent that reads `SKILL.md`.

한국어 요약은 [아래](#한국어-요약)에 있습니다.

## Install

```bash
npx skills@latest add cskwork/motion-graphics-skill
```

Needs Node.js 18+, ffmpeg, and Playwright's Chromium (the skill installs Playwright into each video's work folder).

## What it makes

| Format | What you get |
| --- | --- |
| Launch video | A 30 s, 1920×1080 keynote-style launch or feature video (the SaaS launches you see on X). Every screen is captured from your real app on iOS Simulator, Android emulator, web, or desktop. |
| Shorts | A 20–30 s, 1080×1920 vertical video: hook in the first 0.3 s, one idea per beat, safe zones respected, loops cleanly. |

Ask in plain words, for example: "Make a launch video for our app from the iOS simulator" or "Make a YouTube Short explaining compound interest".

## How it works

A video is one HTML page where every pixel is a pure function of time. `engine/render.mjs` steps through every frame in headless Chromium and encodes with ffmpeg, so renders are frame-accurate and reproducible. Screen recordings play frame by frame through `MG.clip`.

```
skills/motion-graphics/
  SKILL.md                  workflow, composition API, craft bar, render, audio, QA
  formats/launch-video.md   brief, capture, beat sheet, motion vocabulary
  formats/shorts.md         brief, script, type and safe zones, facts on screen
  references/capture.md     capture commands for iOS, Android, web, macOS
  references/pitfalls.md    lessons from real renders
  engine/                   runtime.js, runtime.css, render.mjs
```

## License

MIT. Music, SFX, fonts, and images you add keep their own licenses; the skill records each one in the video's asset manifest.

## 한국어 요약

모션그래픽 영상을 코드로 만드는 에이전트 스킬입니다. 실제 실행 중인 앱 화면으로 만드는 제품 출시 영상(30초, 가로)과 YouTube Shorts·릴스·틱톡용 세로 영상(20–30초)을 지원합니다. `npx skills@latest add cskwork/motion-graphics-skill`로 설치하고, "iOS 시뮬레이터에 떠 있는 우리 앱으로 출시 영상 만들어줘"처럼 요청하면 됩니다.
