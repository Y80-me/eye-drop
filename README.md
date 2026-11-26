# eye-drop
# hcam

Lightweight local launcher: displays wallpaper, spawns CMD windows, and triggers an OpenCV camera stream in one run.

مشغّل محلي خفيف يفتح الصورة، يطلق نوافذ الطرفية، ويشغّل بث الكاميرا عبر OpenCV بأمر واحد.

---

## Overview | نظرة عامة

`hcam` combines a Python embedding script with a Windows batch trigger (`h.bat`) inside the `hacking` directory. When executed, it:
1. Opens the bundled image (`bundle.png`).
2. Extracts and runs the embedded CMD sequence (five sequential command prompt windows).
3. Extracts and runs the embedded OpenCV camera script (`cv2`) with live FPS display, snapshot capture (`S`), and quit (`Q`).

---

## Project Structure | هيكل الملفات

```text
hacking/
├── bundle.png          # Bundled image containing the embedded JSON payload
├── cam.py              # Standalone OpenCV camera script (reference)
├── cmd.bat             # Standalone CMD window loop script (reference)
├── h.bat               # Main launcher script
└── README.md           # Project documentation
