# Embedded Media Viewer

A zero-dependency, single-file PHP & Vanilla JS manga reader optimized for embedded devices, home servers, and mobile reading.

### Features

- **Single File & Lightweight:** Runs out-of-the-box on standard PHP (requires GD extension).
- **Fast Progressive Loading:** Displays an instant thumbnail preview while loading and caching the full-resolution image.
- **Client-Side OPFS Caching:** Uses the browser's Origin Private File System (OPFS) to cache visited pages locally for offline/instant revisiting.
- **Dynamic Thumbnails:** On-the-fly server-side thumbnail generation (`?t=1`).
- **Touch & Gesture Ready:** Supports mobile swipe physics, keyboard arrows, and tap navigation.
- **Secure:** Built-in path traversal safeguards and restrictive Content Security Policy (CSP).
- **Formats:** Supports `.jpg`, `.jpeg`, `.png`, `.gif`, and `.webp`.

---

### Controls

| Action | Control |
|---|---|
| **Previous Page** | Tap left edge (0–28%), Left Arrow key, or Swipe right |
| **Next Page** | Tap right edge (72–100%), Right Arrow key, or Swipe left |
| **Thumbnail Bar** | Tap center screen |

---

### Setup & Usage

1. Save the code as `index.php` (or `viewer.php`) in your manga/image directory.
2. Ensure the PHP GD extension is enabled.
3. Access it directly via your browser:
   - `http://localhost/manga/` (loads the current folder)
   - `http://localhost/manga/index.php/Chapter_01/` (loads a subfolder)
   - `http://localhost/manga/index.php/Chapter_01/05.jpg` (jumps directly to a specific page)
