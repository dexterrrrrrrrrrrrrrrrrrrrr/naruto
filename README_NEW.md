# Naruto / Sasuke Gesture Power (MediaPipe Hands)

A browser-based gesture demo that uses **MediaPipe Hands** to detect whether your **right/left hand is open** and then plays **Naruto** or **Sasuke** power video overlays.

## Demo / Run locally

Open the page in your browser:

- `naruto/index.html`

### Notes
- Most browsers require **camera permission**.
- If camera doesn’t start, try serving via a local web server or allow camera access for the site.

## Controls

- **Right hand open** → shows **Sasuke** power video
- **Left hand open** → shows **Naruto** power video
- **Blue lines** → skeleton/landmarks so you can confirm tracking is working

## How it works

- MediaPipe Hands runs directly in the browser via CDN.
- The script checks finger landmarks relative to the wrist to decide if the hand is open.
- When power is active, it positions the overlay based on wrist/knuckle landmarks.

## Project structure

- `index.html` – main application
- `assets/naruto.mp4` – Naruto overlay video
- `assets/sasuke.mp4` – Sasuke overlay video

## License

MIT

