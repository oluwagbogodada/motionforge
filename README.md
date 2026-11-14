# MotionForge — Event Motion Studio

A dark, editorial event-design workspace. Add event information and speaker portraits, choose an art direction, and preview a live animated event composition.

## Current features
- Responsive studio dashboard
- Event name, tagline, date, time, venue and organiser fields
- Multiple speaker / host profiles with local image uploads
- Four visual directions: Noir/Gold, Electric, Monochrome and Pulse
- Live animated composition with four selectable scenes
- Portrait (9:16) and landscape (16:9) layouts
- High-resolution PNG poster export
- Downloadable JSON project file
- Local browser autosave

## Run locally
```bash
npm install
npm run dev
```

## Build
```bash
npm run build
npm run preview
```

## Roadmap
1. Remotion-based video composition and server-side MP4 rendering.
2. Background music and sound design controls.
3. More scene templates, editable transitions and per-scene timing.
4. Cloud project storage, user accounts and team workspaces.
5. Print-ready poster and platform-specific social exports.

**Important:** This first milestone exports PNG posters and project JSON. The animated preview is client-side; MP4 rendering is not yet implemented. Uploaded portraits are stored in the browser session/project state, not uploaded to a server.
