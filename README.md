# OZA — Open Zink Archive

OZA (Open Zink Archive) is an **experimental web-based archive format**.  
It runs entirely in your browser using HTML + JavaScript.  
No installation, no native binaries — just open the page and start compressing.  

---

## ✨ Features

- Select multiple files (up to `9,999,990,123,013` — theoretical limit).
- Compress files into a single `.oza` archive directly in the browser.
- Decompress `.oza` archives back into their original files.
- 100% client-side: no server, no upload, all processing is local.
- Uses [pako (zlib/deflate)](https://github.com/nodeca/pako) for compression.

---

## ⚠️ Notes

- **Not a replacement for ZIP/RAR/TAR.** This is just a prototype to explore browser-based compression.
- Compression ratio depends on file type:  
  - Text/JSON/CSV can shrink dramatically (e.g. 3MB → 1MB).  
  - Already compressed files (JPG, MP4, MP3) may barely shrink at all.
- Large files (>100MB) may freeze or crash your browser.

---

## 🚀 How to Use

1. Open [`index.html`](index.html) in your browser.
2. Select files to compress.
3. Download the generated `.oza` archive.
4. To decompress, re-open `index.html` and load your `.oza` file.

---

## 📂 Project Structure
