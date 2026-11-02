# Cosmic Window

A one-page app that shows NASA's [Astronomy Picture of the Day](https://apod.nasa.gov/) using the [APOD API](https://api.nasa.gov/).

- Twinkling starfield and a slow zoom on each photo
- Previous / next day, date picker, and "Surprise me" for a random day since 1995
- Click the photo (or press **F**) for full-screen HD
- Keyboard: **←** / **→** change day, **R** random

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8765
```

then visit http://localhost:8765.

## API key

The app uses a free NASA API key (1,000 requests per hour), set near the top of the script in `index.html`. If you fork this project, get your own key at [api.nasa.gov](https://api.nasa.gov) and replace it there.
