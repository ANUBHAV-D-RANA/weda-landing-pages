# The Winning Edge Defence — Landing Pages 2026-27

Static landing pages for the 2026-27 classroom batches at the new centre,
Shiv Shakti Tower, Near Donali Chowk, Dehradun.

## Pages

| Route          | Batch                    | Sub-brand                            |
| -------------- | ------------------------ | ------------------------------------ |
| `/`            | Hub — all four batches   | The Winning Edge Defence             |
| `/rimc`        | RIMC 2026-27             | The Winning Edge Defence Academy     |
| `/sainik-rms`  | Sainik School & RMS 2026-27 | The Winning Edge Defence Academy  |
| `/cds`         | CDS 2026-27              | The Winning Edge Defence Plus        |
| `/ssc-gd`      | SSC GD 2026-27           | The Winning Edge Uniform Ready       |

Each batch page is a single self-contained `index.html` — all CSS is inline and
all images are embedded as base64 data URIs, so a page can also be opened
straight from disk or emailed as one file. The only external requests are the
Google Fonts stylesheet (Oswald + Poppins).

## Structure

```
.
├── index.html          hub page linking to all four batches
├── assets/logo.png     shared logo, used by the hub only
├── cds/index.html
├── rimc/index.html
├── sainik-rms/index.html
├── ssc-gd/index.html
└── vercel.json
```

## Editing

The batch pages are hand-written HTML with no build step. Edit the `index.html`
inside the relevant folder and push — Vercel redeploys on every push to `main`.

Details shared across all pages, worth changing together if they change at all:

- Phone: `+91 8437001122`
- WhatsApp: `https://wa.me/917417920356`
- Address: Shiv Shakti Tower, Near Donali Chowk, Dehradun, Uttarakhand
- Classes start: 18 September 2026 · Free demo classes: 18–30 September 2026

## Local preview

No tooling required — open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```
