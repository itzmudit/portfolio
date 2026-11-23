# muditjindal.vercel.app

My portfolio, built as one hand-written HTML file: no frameworks, no build step, no templates.

[![Live site](https://img.shields.io/badge/▶_live-muditjindal.vercel.app-ffb547?style=flat-square&labelColor=0d1113)](https://muditjindal.vercel.app)
![Vanilla](https://img.shields.io/badge/HTML_·_CSS_·_JS-0_frameworks-62c784?style=flat-square&labelColor=0d1113)
![Installable](https://img.shields.io/badge/PWA-installable-5fd4e3?style=flat-square&labelColor=0d1113)

![Preview](og.jpg)

## What's on the page

| | |
|---|---|
| **A working shell** | Type `help`. Tab completes, ↑ ↓ for history, `/` jumps there from anywhere. Try `ohm 9V 4.7k`, `resistor 4.7k`, `solve bridge`, `./caughtbot --score` or `fortune`. |
| **MiniSPICE, live** | The same nodal-analysis + Gaussian-elimination algorithm as my C project [MiniSPICE](https://github.com/itzmudit/MiniSPICE), ported to JavaScript. Edit any resistor and it re-solves instantly. **Share circuit** copies a link that opens your exact circuit. |
| **Image lab** | Grayscale, threshold, invert, histogram equalisation, gamma, Gaussian blur and Sobel edges, all written from scratch. Uploaded photos never leave the browser. |
| **Resistor decoder** | Pick four colour bands to get the value and tolerance range. The shell's `resistor` command goes the other way. |
| **CaughtBot case study** | Results from [CaughtBot](https://github.com/itzmudit/CaughtBot), the AI red-teaming tool my team built at Hackin' Summer 2026. |
| **Background** | Falling code and circuit traces drawn on canvas. Traces light up under the cursor; clicks send sparks. |
| **Easter eggs** | A few. `eggs` in the shell tracks how many you've found. |

## Details I cared about

- **Phones get a calmer layout**: lighter animation, fewer panels, and eggs that fit the screen (hold the name for a surprise).
- **Respects "reduce motion"**: if your device asks for less animation, the page goes still.
- **Prints cleanly**: `print` in the shell (or *save as PDF* in the footer) gives a plain, readable copy.
- **Installable**: add it to your home screen from Chrome or Safari; it opens full-screen with the MJ icon and works offline.
- **Keyboard friendly**: skip link, visible focus, `?` shows shortcuts.
- **Link previews**: sharing the URL shows a proper preview card.
- **Privacy**: no cookies. Visit counts come from Vercel Web Analytics, which stores no personal data.

## Files

```
index.html             the whole site: markup, styles and scripts
404.html               the "no such file or directory" page
og.jpg                 the link-preview image
manifest.webmanifest   makes the site installable
sw.js                  offline support (network first, cache as fallback)
favicon.svg, icon-*.png, apple-touch-icon.png   the MJ icons
robots.txt, sitemap.xml
```

## Run it locally

It's static. Open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
```

Deploys to Vercel on every push to `main`.

---

[GitHub](https://github.com/itzmudit) · [LinkedIn](https://www.linkedin.com/in/itzmudit) · muditjindal100@gmail.com
