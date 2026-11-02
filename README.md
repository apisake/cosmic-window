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

## Where the data comes from

In late 2026 NASA moved APOD from apod.nasa.gov to [science.nasa.gov/apod](https://science.nasa.gov/apod/), and the official API at api.nasa.gov started returning a placeholder for every day. Until that's fixed, the app uses:

- **Picture info** from [apod.ellanan.com](https://apod.ellanan.com), an unofficial community mirror of the APOD API (no key needed). It has real entries up to 28 September 2026.
- **Image and video files** from the [Internet Archive's](https://web.archive.org) copies of the old apod.nasa.gov site, picked by each picture's date.

The newest picture is therefore 28 September 2026 for now.
