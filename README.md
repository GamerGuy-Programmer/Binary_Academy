# Binary Academy

A dependency-free educational app built with HTML, CSS, JavaScript, SVG, and browser-native APIs.

## Run locally

Open `index.html` in a modern browser. For a consistent storage origin, serve this folder instead:

```sh
python -m http.server 8765
```

Then visit http://localhost:8765. Keep the same browser and URL to retain your progress.

## Learning experience

- Nine sequential modules and 27 challenges: binary fundamentals, conversions, arithmetic, text encoding, storage, logic, hexadecimal, signed integers, and fractions.
- Correct answers earn 15 XP once per challenge. Completed lessons remain available for review.
- Six achievements are calculated from saved challenge progress.
- Number conversion, UTF-8 encoding/decoding, and interactive bit switches.
- Responsive dark interface, SVG icons, keyboard focus management, skip link, and reduced-motion support.

## Local progress

Challenge completion and XP use the existing `binary-academy-v1` LocalStorage key, retaining progress from the original six modules. Saving failures are shown in the interface. Progress belongs to the current browser profile and site origin; clearing site data removes it. Private browsing may discard it when closed. No accounts, backend, analytics, or external fonts are used.

## Verify

```sh
node --check script.js
node verify.cjs
```

The verification script exercises application logic with a small DOM/storage harness: challenge progression, retries, XP, achievements, reloads, numeric limits, invalid UTF-8, and unavailable storage. It does not replace visual browser testing.

## Static hosting

Upload `index.html`, `style.css`, and `script.js` to any static host. No build command is needed; use the project root as the output directory. Moving to a different origin starts a separate local progress store.
