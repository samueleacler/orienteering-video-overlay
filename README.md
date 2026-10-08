# Orienteering Video Overlay HUD 🧭🏃‍♂️

A lightweight, web-based tool designed for orienteering content creators. It generates a real-time Head-Up Display (HUD) ready to be recorded over a green screen and superimposed onto your POV headcam footage (GoPro, DJI, etc.) using any video editing software like Final Cut Pro, Premiere Pro, or DaVinci Resolve.

## ✨ Features
*   **Dynamic Leaderboard:** Import race results directly via Excel (`.xlsx`) or CSV. The leaderboard automatically calculates gaps and updates smoothly using FLIP animations whenever you punch a new control.
*   **GPX Data Sync:** Upload your `.gpx` track (from Garmin, Polar, Suunto) to display real-time **Heart Rate (bpm)** and calculated **Pace (min/km)**.
*   **Green Screen Ready:** The UI is set on a pure `#00FF00` background, optimized for flawless Chroma Key extraction.
*   **Customizable Race Info:** Add your event name, category, and target athlete name directly from the UI.
*   **No Installation Required:** Runs entirely in your local browser using vanilla HTML, CSS, and JS (with SheetJS for Excel parsing).

## 🚀 How to Use

1. **Open the App:** Open `index.html` in any modern web browser.
2. **Load Data:**
   * Enter your name exactly as it appears in the results.
   * Upload the race results (`.xlsx` or `.csv`).
   * Upload your `.gpx` file containing Heart Rate data.
3. **Set Race Info:** Type the Event Name and Category.
4. **Record:** 
   * Set the slider to `0` (or your desired starting point).
   * Start your screen recording software (e.g., QuickTime Player on Mac, OBS).
   * Click **"▶ Avvia Tempo (1x) & Registra"** to start the real-time simulation.
5. **Video Editing:**
   * Import the screen recording into your NLE (Final Cut Pro, DaVinci Resolve).
   * Place it on the track above your headcam footage.
   * Apply a **Keyer / 3D Keyer** effect to remove the green background.
   * *Pro tip: Use the crop tool to remove the browser edges and add a Drop Shadow effect to make the UI stand out.*

## ⌨️ Controls
*   **Click anywhere** on the green background or press **ESC** to pause the timer and bring back the setup panel.
*   Use the **Slider** to preview specific legs of the course before recording.

## 🛠 Tech Stack
* HTML5 / CSS3
* Vanilla JavaScript
* [SheetJS](https://sheetjs.com/) (for parsing Excel files locally)

## 📄 License
This project is open-source and available under the MIT License.
