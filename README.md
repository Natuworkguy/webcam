# Camera Feed WebApp

> 🚀 A sleek, futuristic web app for real-time camera streaming, filter effects, and video recording with pause/resume and save functionality. Built for desktop vibes only — mobile peeps get a friendly heads-up.

---

## Table of Contents

* [Overview](#overview)
* [Features](#features)
* [Tech Stack](#tech-stack)
* [How to Use](#how-to-use)
* [Keyboard Shortcuts](#keyboard-shortcuts)
* [Compatibility](#compatibility)
* [Known Limitations](#known-limitations)
* [Future Improvements](#future-improvements)
* [License](#license)

---

## Overview

This web app grabs your camera feed and streams it full-screen with a slick glowing neon vibe. It lets you toggle between multiple cameras, slap on some rad filters, and record video with audio. You can pause/resume recording and save your masterpiece locally as a `.webm` file. The UI slides in from the side and can be toggled with a keyboard shortcut for that ultra-smooth workflow.

---

## Features

* **Live camera feed** with full viewport coverage and neon-glow styling
* **Camera selection** dropdown to switch between multiple video input devices
* **Video filters:** None, Grayscale, Sepia, Invert, High Contrast, Blur — change on the fly!
* **Recording controls:** Record, Pause/Resume, Stop, and Save video locally
* **Project naming:** Name your recording files dynamically
* **Keyboard shortcut:** `Ctrl + Y` toggles the options menu
* **Mobile warning:** Blocks unsupported mobile devices with a polite message
* **Clean, responsive, and minimalistic UI** styled with a futuristic green glow

---

## Tech Stack

* **HTML5** for structure
* **CSS3** for neon-themed styling and transitions
* **Vanilla JavaScript** handling media devices, recording, and UI interactions
* **WebRTC API** for capturing media streams
* **MediaRecorder API** for recording video + audio streams

---

## How to Use

1. Open the web app in a **desktop browser** (mobile not supported — sorry folks).
2. The camera feed will auto-start if permissions are granted.
3. Press `Ctrl + O` to toggle the options menu (slides in/out).
4. Select your preferred camera from the dropdown.
5. Pick a filter from the filter selector to instantly update the video feed.
6. Type your desired project name — this will be your saved video filename.
7. Hit **Record** to start capturing your video with audio.
8. Use **Pause** to pause recording; button toggles to **Resume** to continue.
9. Hit **Stop** to end recording — then the **Save** button appears.
10. Click **Save** to download the `.webm` file to your computer.

---

## Keyboard Shortcuts

| Shortcut   | Action                         |
| ---------- | ------------------------------ |
| `Ctrl + O` | Toggle options menu open/close |

---

## Compatibility

* Designed to run on modern **desktop browsers** with support for:

  * `navigator.mediaDevices.getUserMedia`
  * `MediaRecorder` API
* Tested on Chrome, Firefox, and Edge desktop versions
* Not supported on mobile browsers (detects and displays a warning)

---

## Known Limitations

* No backend — all recording & saving happens client-side
* Limited to `.webm` video format
* Audio input is always from the default microphone paired with the camera feed; no separate audio device selector
* Some browsers may block or limit camera access without HTTPS
* Mobile device support is intentionally blocked due to constraints

---

## Future Improvements (Ideas, cuz why not innovate?)

* Add video format export options (e.g., MP4 via client-side transcoding)
* Include separate audio device selector
* Add ability to save recordings directly to cloud storage (Dropbox, Google Drive)
* Implement advanced filter controls (sliders for intensity, combos)
* UI/UX polish: draggable/resizable options panel, dark/light mode toggle
* Support for mobile devices with adapted UI and fallback handling

---

## License

This project is open-source and free to use under the [MIT License](https://opensource.org/licenses/MIT). Feel free to remix, hack, and share!

---

# 🚨 Pro Tip

Make sure you’re testing with HTTPS on localhost or a secure domain — browsers get super paranoid about camera access without it.
