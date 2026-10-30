# Orbit — Everyday Tools

A responsive, single-page browser toolkit built with plain HTML, CSS and JavaScript.

## Run it

1. Extract the ZIP.
2. Open the folder in VS Code.
3. Start the page with **Live Server**, or run `python -m http.server 8000` inside the folder.
4. Visit `http://localhost:8000`.

Opening through `localhost` (or HTTPS) is recommended because camera, microphone, geolocation and motion APIs require a secure browser context and user permission.

## What's included

- Calculator
- Unit converter (length, mass, temperature, volume, area, data and speed)
- Currency converter (latest available rates from open.er-api.com)
- Notes and to-do list (saved in localStorage)
- Alarm, countdown timer and stopwatch
- Calendar with local reminders
- Flashlight / camera torch attempt, QR scanner and geolocation
- File picker / file list, PDF preview, camera scan pages and PDF export
- Music and video players for local files
- Photo gallery with simple visual filters and export
- Drawing canvas with PNG export
- Voice recorder and camera capture
- Tic-tac-toe, 2048, Snake, Word guess and Sudoku
- General knowledge quiz
- Habit tracker and expense tracker (saved in localStorage)
- Weather lookup using Open-Meteo
- Motion-based step estimate with manual fallback
- Generated ambient sounds for meditation / sleep

## Browser and privacy notes

- No backend or account is required. Notes, tasks, reminders, habits, expenses, budget and step counts stay in this browser's local storage. Clearing site data removes them.
- The file manager only lists files you explicitly choose; a normal webpage cannot browse your whole device.
- Camera, microphone, location, motion and flashlight controls depend on hardware/browser support and require permission. Flashlight control is especially device-dependent.
- The alarm and timer need this page to remain open. They are not guaranteed replacements for a phone's native alarm app.
- Current currency rates and weather require an internet connection. Currency rates use ExchangeRate-API’s open endpoint (updated daily; attribution required). Weather data comes from Open-Meteo; its free endpoint is intended for non-commercial use and the data requires CC BY 4.0 attribution. Review Open-Meteo’s current terms before any commercial deployment; the weather page identifies the provider.
- QR image decoding and PDF export use jsQR and jsPDF from public CDNs. Google Fonts also loads from the internet. Core UI and local tools still work without those services, but those specific online-dependent features may not.
- The PDF reader uses the browser's built-in PDF viewer. “Scan” means capturing/choosing page images and exporting them into a PDF; it does not run OCR or automatically extract text.
- Photo filters are basic visual effects; this is not a full professional image editor. The step counter uses a rough motion threshold and is not a medical-grade fitness measurement.

## Files

- `index.html` — app layout and tool panels
- `style.css` — responsive dark interface and component styling
- `script.js` — interactions, browser APIs, local storage and game logic