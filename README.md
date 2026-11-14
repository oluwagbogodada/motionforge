# MotionForge — Motion Ad Studio

MotionForge turns event information and host/speaker portraits into animated promotional videos.

## Phase 2 features
- Canvas-based animated ad composition with four scenes: opening, people, event details and call to action
- Editorial motion language inspired by the supplied reference: animated data lines, grid, kinetic typography, subtle RGB/glitch accents and moving particles
- Speaker and host portrait uploads
- In-browser background removal using @imgly/background-removal
- Transparent speaker cutouts composited into the people scene
- Four art directions: Signal / Editorial, Afterglow, Electric and Mono / Luxe
- Story/Reel, feed portrait, square and landscape output sizes
- Optional background soundtrack mixed into supported browser recordings
- Browser video recording and MP4 conversion with FFmpeg.wasm when needed
- Scene-by-scene preview, poster-frame export and local autosave

## Run
```bash
npm install
npm run dev
```

## Build
```bash
npm run build
```

## Rendering notes
Video is composed and recorded in the user's browser. Browsers that can record MP4 directly use that format; other browsers record WebM and convert it to MP4 locally using FFmpeg.wasm. The first MP4 conversion downloads FFmpeg core WASM assets into the browser. Video export is resource-intensive; a desktop browser is recommended for long or high-resolution renders.

Portrait background removal runs in the browser and downloads model assets on first use. Uploaded portraits are not sent to a MotionForge server.

## Current storage
Event text settings are saved in local browser storage. Portraits and music remain in the current browser session; cloud project storage and user accounts are not implemented yet.
