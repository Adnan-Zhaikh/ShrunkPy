# ShrunkPy

Compress, resize, and convert images and PDFs, free, in your browser. No upload, no signup, no watermark, no file limits.

**Live:** <https://adnan-zhaikh.github.io/ShrunkPy/>

<!-- Add a screenshot or GIF of the tool in action here. -->

## Why I built this

Most online compressors lock basic features behind a paywall, or upload your files to a server you know nothing about. Compressing an image is not hard, so I built my own. Everything runs on your device and your files never leave it.

## What it does

| Tool | What it does |
| --- | --- |
| **Size Analyzer** | Shows file sizes at a glance |
| **Image Resizer** | Scales by width and keeps proportions |
| **Image Converter** | Converts between JPG, PNG, and WebP, and handles transparency correctly |
| **Image Compressor** | Compresses an image to hit a target file size automatically |
| **PDF Compressor** | Shrinks the JPEG images inside a PDF while keeping the text selectable |

## How it works

- **Images:** the browser's Canvas API redraws the image at a new size or quality and exports it in the format you pick.
- **PDFs:** [pdf-lib](https://pdf-lib.js.org/) opens the PDF in the browser, finds the embedded JPEG images, and recompresses them. Text is untouched, so it stays selectable.
- **Privacy:** there is no backend. Files are processed in your browser's memory and never sent anywhere.

## Tech

Plain HTML, CSS, and JavaScript in a single `index.html`. No framework, no build step, no dependencies to install.

## What I learned

This was a project of firsts.

- **Static sites:** I built a real, useful tool with no framework and no backend. Plain HTML/CSS/JS is enough for a lot.
- **Browser APIs:** I learned how the Canvas API handles resizing, format conversion, and quality settings, and why transparency needs special care when converting to formats like JPG.
- **PDF internals:** PDFs are structured files, and you can shrink one by recompressing the images inside it.
- **Deploying with GitHub Pages:** this was my first deployment. Pushing to a repo and getting a public URL was a good feeling.
- **SEO:** I optimized the page and got it indexed on Google. A page nobody can find is not much use, so making a tool discoverable is part of building it.
- **Client-side privacy:** doing the work in the browser means there are no servers, no storage costs, and nothing for users to worry about.

<!-- Optional: add 1-2 specifics of what you did for SEO (title/meta description, headings, sitemap, Search Console), and one hard bug you hit and how you fixed it. -->

## Run it locally

No setup needed. Download or clone the repo and open `index.html` in your browser.

```bash
git clone https://github.com/Adnan-Zhaikh/ShrunkPy.git
```

## Related

The CLI/Python versions of these tools live in [side-quests](https://github.com/Adnan-Zhaikh/side-quests). They also include a file organizer and bulk renamer, which need OS-level file access that a browser can't give.

## Author

**Adnan** — [@Adnan-Zhaikh](https://github.com/Adnan-Zhaikh)
