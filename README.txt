MediaGrabber Pro - Video & Audio converter (folder: video-audio)

HOW TO PUT IT ONLINE (GitHub Pages)
1. Upload this whole "video-audio" folder to your repo (keep the folder and file names exactly as they are).
2. Open it from the https:// address, for example:
   https://YOUR-NAME.github.io/YOUR-REPO/video-audio/
   Do NOT double-click the files: converting and exporting do not work from a local file.
3. To test on your computer: open a terminal in the folder that CONTAINS "video-audio" and run
   python3 -m http.server 8000
   then open http://localhost:8000/video-audio/

FILES
index.html    the converter (Video Converter / Audio Converter tools).
              "Add audio / music" opens the Timeline studio. A "Simple" switch brings back the old version.
studio.html   Timeline studio: video + music/audio + text + elements, export up to 4K (only if you choose it).
              Used inside the Add audio / music tool; it also works on its own.
editor.html   The full video editor (filters, crop, transitions, animations, projects...). Works on its own.
ffmpeg/       The converting engine used by index.html (needed). Keep all 4 files.
*.png, *.ico  Logos and icons.
vendor/       Not needed any more: studio.html and editor.html now contain the MP4/WebM writers inside.
              Kept only so nothing is deleted. Licenses are in vendor/licenses.

NOTES
- studio.html and editor.html are self-contained: they work even if only that one file is uploaded
  (MP4 on browsers without a built-in H.264 encoder also needs the ffmpeg/ folder).
- Microphone recording needs https:// (or http://localhost).
