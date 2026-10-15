# Curial — home page redesign

Single-page marketing site for Curial. Plain HTML, CSS and JavaScript in one
`index.html`, no build step. Fonts load from Google Fonts (Inter).

## Run locally

Requires Python 3.

```bash
python serve.py 5520 .
```

Then open http://localhost:5520.

`serve.py` is a small static server with HTTP Range support. Use it instead of
`python -m http.server`: without Range requests the browser cannot seek the
demo video, so the chapter cards in the walkthrough section would not jump to
their timestamps.

## Structure

```
index.html   page markup, styles and scripts
assets/      demo video, captions (.vtt) and photos
serve.py     local dev server with Range support
```

## Notes

- Product screens, quotes and numbers on the page are sample data.
- The demo form shows a local confirmation only; connect it to your CRM before launch.
- Animations respect `prefers-reduced-motion`.
