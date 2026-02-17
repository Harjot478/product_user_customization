# Product User Customization

A small web page to personalize a product mockup by typing a name and styling it.

## Project description

This repository contains a simple static webpage that lets users type their name and preview it over a faint product mockup (T-shirt, Mug, Poster) or over a custom background image. Users can pick color, font, and size and apply preset styles. Settings persist across page refreshes.

## Features

- Live preview of the typed name over a product mockup.
- Controls for: Name, Color, Font, Size.
- Live size indicator: `Size: 36px` updates as you move the slider.
- Product mockups: T-shirt, Mug, Poster (faint silhouettes).
- Upload a background image to use as the product background.
- Preset style buttons: `Minimal`, `Bold`, `Elegant` (apply pre-configured font + color + size).
- Persistent settings: Name, Color, Font, Size, selected mockup, and uploaded background image are saved to `localStorage` so they remain after refresh.
- Reset button clears the name and restores defaults.
- Contrast helper: small text shadow is applied automatically to improve readability against chosen colors.

## Files

- `index.html` — main UI and JavaScript logic
- `style.css` — styling for controls and mockup

## How to run

Open `index.html` in a browser. For a quick local server (recommended):

```bash
# from repo root
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

## Notes

- Uploaded background images are stored in `localStorage` as data URLs (suitable for small images). Clearing browser storage or using the `Reset` button removes the stored image.
- If you want additional presets or product mockups added, tell me which styles or product types you prefer.
