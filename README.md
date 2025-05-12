# TtPhotoTool (Photolog Generator)

A web-based tool for generating photo documentation reports. Upload images (ZIP, multi-select, or folder) alongside an Excel metadata sheet, and export formatted Word documents using one of two report templates.

---

## Features

- Upload photos via:
  - ZIP file
  - Multi-select image upload
  - Folder upload
- Upload metadata via Excel (.xlsx)
- Automatically match metadata to images
- Preview report in-browser
- Export to Word in:
  - **Template A** (2 photos per page)
  - **Template B** (1 photo per page)
- Download a log of unmatched images or metadata rows
- Built with:
  - JavaScript
  - Bootstrap 5
  - SheetJS, EXIF.js, JSZip
  - html-docx-js / docx.js

---

## Folder Structure

```
/
├── index.html           # Main tool interface
├── favicon.svg          # Site icon
├── photolog-preview.png # Thumbnail/preview for social/media embeds
├── tetra-tech-logo.png  # Logo used in reports
├── epa-logo.png         # Logo used in reports
├── README.md            # This file
```

---

## How to Use

1. Open `index.html` in a browser (no server required)
2. Enter project details
3. Upload photo set and Excel metadata
4. Click **Generate Report**
5. Preview report in browser
6. Download as Word document using Template A or B
7. Optionally download the error log for unmatched files

---

## Excel Metadata Requirements

The Excel file must include a column named `Attachment_Name` that matches image filenames exactly. Other helpful fields:

- `Description`
- `Photographer`
- `FeatureLatitude` / `FeatureLongitude`
- `Direction_Photo`
- `Category`
- `EXIF_ImageDateTime_Text`

---

## License

Private/internal tool — not currently licensed for public distribution.
