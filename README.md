# Afterglow — Proposal Music Player

Afterglow is a romantic, proposal-themed browser music player. It pairs a local playlist with a polished responsive interface, animated lyric moments, a personal proposal note, and Bollywood romantic-song discovery.

## Features

- Full playback of the bundled local MP3 files
- Play, pause, seek, previous/next, shuffle, repeat, mute, and volume controls
- Keyboard shortcuts: Space to play/pause; left/right arrows to seek
- Responsive desktop and mobile layouts
- Floating heart ambience, animated track indicators, and lyric transitions
- A proposal note modal that can be personalised in `index.html`
- Song discovery for Bollywood romantic music using the iTunes Search API
- Curated romantic-song recommendations when the online catalog is unavailable

## Run locally

The app has no build step and no dependencies.

1. Open the project folder.
2. Start any static web server in this folder.
3. Open `index.html` through that server.

With Node.js installed, run: `npx http-server . -p 4173`

Then open `http://127.0.0.1:4173`.

## Adding your own songs

1. Put an MP3 file in the project folder.
2. Add an item to the `songs` array in `index.html`.
3. Provide its title, artist, album label, filename, duration, and a short lyric moment.

The player deliberately plays only tracks stored locally in the project. This keeps the full listening experience under your control.

## Music discovery API

The “Discover love songs” button searches Apple’s public iTunes catalog for Bollywood romantic songs. Where Apple provides one, the result includes a **Preview 30 sec** button that loads the official preview directly into the player. Every discovery card also includes official **YouTube**, **Spotify**, and Apple/iTunes links, so listeners can choose their preferred free or signed-in listening service. The app does not download or copy music.

Network access can be blocked by a browser, firewall, privacy extension, or offline connection. In that case, Afterglow automatically shows curated suggestions such as *Tum Se Hi*, *Agar Tum Saath Ho*, *Kesariya*, and *Pehla Nasha*, each with a direct Apple Music search link.

The iTunes Search API returns catalog metadata such as track name, artist, artwork, and a store URL. See Apple’s [Search API documentation](https://developer.apple.com/library/archive/documentation/AudioVideo/Conceptual/iTuneSearchAPI/Searching.html).

## Personalising the proposal

Edit the text in the `noteDialog` section of `index.html` to change the proposal message and signature. You can also update the `heart-field`, colors, and song lyric moments to match the occasion.
