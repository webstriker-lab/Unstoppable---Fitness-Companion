# Unstoppable Fitness Companion

This repository hosts the Unstoppable weights and test companion as a free static GitHub Pages site.

## Live site

After GitHub Pages finishes deploying, the companion should be available at:

```text
https://webstriker-lab.github.io/Unstoppable---Fitness-Companion/
```

## What is included

- `index.html`: the hosted companion page.
- `Unstoppable_Weights.html`: duplicate filename kept for compatibility with older local links.
- `.nojekyll`: tells GitHub Pages to serve the files exactly as-is.
- `.github/workflows/pages.yml`: deploys the static site to GitHub Pages whenever `main` is updated.

## Rebuild the PDF with mobile-safe links

From the folder where `build_unstoppable_pdf.py` lives, run:

```powershell
.\Rebuild_PDF_With_Website_Link.ps1 "https://webstriker-lab.github.io/Unstoppable---Fitness-Companion/"
```

That rebuilds `Unstoppable.pdf` so every `GET WEIGHTS` link opens the hosted companion website on mobile.

## Storage note

The companion stores your entered numbers in the browser's `localStorage`. That means values stay on the same device/browser, but they do not automatically sync between devices.
