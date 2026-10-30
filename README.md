# Zip Image Converter

Convert a single image, every page of a PDF, or a whole zip of documents to **JPG, PNG or WebP**, with an optional size limit per file (for example, JPG ≤ 250 KB for upload portals).

Everything runs in your browser. Files are never uploaded anywhere.

## How to use

1. **Pick what you're converting:** Image, PDF or Zip.
2. **Choose output settings:** format, quality, max file size, max dimensions, PDF page resolution (DPI).
3. **Upload and convert,** then download.
   - Image → one converted file
   - PDF → one image per page (`file_page-1.jpg`, …), zipped if more than one page
   - Zip → the same zip back, folders and names kept, images converted and PDF pages turned into images

## Hosting

It's a single static `index.html`, served with GitHub Pages (Settings → Pages → Deploy from branch `main`, folder `/root`).

Libraries load from cdnjs: [JSZip](https://stuk.github.io/jszip/) 3.10.1 and [PDF.js](https://mozilla.github.io/pdf.js/) 3.11.174 (loaded only when a PDF is converted).
