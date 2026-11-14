# Mahmoud Hamed — Pharmacist CV site

A one-page personal CV website plus a print-ready A4 CV, built as plain HTML/CSS/JS (no build step, no dependencies).

## Files

| File | Purpose |
|---|---|
| `index.html` | Landing page: summary, experience, skills, education, contact |
| `assets/styles.css` | All styling (responsive + reduced-motion support) |
| `assets/script.js` | Mobile menu, scroll spy, reveal animations |
| `cv.html` | Print-optimised A4 CV — opens with "Print / Save as PDF" |
| `assets/Mahmoud_Hamed_CV_KSA.pdf` | The generated one-page CV sent with applications |

## Edit the content

1. Open `index.html` and change the text directly.
2. Open `cv.html` for the printable CV.
3. Regenerate the PDF after editing `cv.html`:

```powershell
& "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" `
  --headless=new --disable-gpu --no-pdf-header-footer `
  --print-to-pdf="assets\Mahmoud_Hamed_CV_KSA.pdf" `
  "file:///C:/Users/Mahmoud/Documents/Default Project/mahmoud-cv-site/cv.html"
```

## Preview locally

```powershell
python -m http.server 8899 --bind 127.0.0.1
# then open http://127.0.0.1:8899/
```

## Placeholder to complete

The community pharmacy role has no employer name or dates yet (the source CV did not include them).
Update both `index.html` and `cv.html` when available, then regenerate the PDF.

## Deployment

Hosted with GitHub Pages from the `main` branch root.
