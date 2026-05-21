# PDF Repaginator

> A FBI tool — realigns the page numbers of a scanned PDF with the ones printed in the book.

**[Use the tool →](https://arm3l.github.io/pdf-repaginator/)**

---

## What it does

Scanned PDFs of fake books, methods and song collections almost always have a mismatch between the file pagination and the printed book pagination (cover, foreword, index all sit before page 1).

This utility adds *page labels* to the PDF so that the numbers shown by your PDF reader match the ones printed in the book. No more mental arithmetic: when [Fake Book Index](https://arm3l.github.io/fbi-data/) says "page 142", you type 142 in your reader and land right on the standard.

## Features

- **100% local** — your PDF never leaves your machine, no server, no upload
- **Single HTML file** — everything is embedded, works offline (`file://`) or online
- **Bilingual FR / EN** — auto-detects browser language, switch persists across sessions
- **Real Book conventions** — covers (`Cover 1`, `Cover 2`...), front matter in lowercase Roman (`i`, `ii`, `iii`...), body in Arabic numerals (`1`, `2`, `3`...)
- **Per-page adjustments** — skip a page (duplicate, junk), force a specific number (jumps, inserted pages)
- **Lazy thumbnail rendering** — handles large PDFs gracefully (tested OK on 230 MB files)

## How to use

1. Drop a PDF onto the drop zone (or click to pick one)
2. Set the number of cover pages, front matter pages, and the starting body number
3. Click any body thumbnail to make per-page adjustments if needed
4. Generate the new PDF — your original file is never modified

## Reader compatibility

Page labels are read by most serious PDF readers:

| Reader | Reads page labels |
|---|---|
| Preview (macOS) | ✅ |
| Adobe Acrobat | ✅ |
| forScore (iPad) | ✅ |
| PDF Expert | ✅ |
| Goodnotes | ✅ |
| Chrome / Safari / Firefox (built-in viewer) | ❌ |

Built-in browser PDF viewers don't display page labels — that's a viewer limitation, not an output issue. The generated file is correct and will work properly in any of the supported readers.

## Tech stack

- [pdf-lib](https://pdf-lib.js.org/) for PDF rewriting
- [pdf.js](https://mozilla.github.io/pdf.js/) for thumbnails and preview
- Vanilla HTML / CSS / JS, no local dependencies

## Collection

`PDF Repaginator` is part of the **FBI tools** collection — utilities for musicians, companion to the [Fake Book Index](https://arm3l.github.io/fbi-data/) app (iOS / Android).

---

*— Armel C.*
