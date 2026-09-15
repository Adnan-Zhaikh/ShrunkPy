# ShrunkPy

Compress, resize, and convert images — free, in your browser. No upload, no signup, no watermark, no file limits.

**Live:** https://adnan-zhaikh.github.io/ShrunkPy/

## Why
Most online image compressors charge for basic functionality that's genuinely simple to build. This runs entirely client-side — your files never leave your device.

## Tools
- **Size Analyzer** — inspect file sizes at a glance
- **Image Resizer** — scale by width, keeps proportions
- **Image Converter** — switch between JPG / PNG / WebP, handles transparency correctly
- **Image Compressor** — hit a target file size automatically
- **PDF Compressor** — shrinks embedded JPEG images inside a PDF, keeps text selectable

## Tech
Plain HTML/CSS/JS. No build step, no framework. Canvas API for image processing, pdf-lib for PDF manipulation.

## Related
CLI/Python versions of these tools (plus a file organizer, bulk renamer not included here since they need OS-level file access) live in [side-quests](https://github.com/Adnan-Zhaikh/side-quests).