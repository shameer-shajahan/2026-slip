# A5 Print Overlay

This project is a simple browser-based tool for generating A5 voter-slip style pages from spreadsheet data.

## What It Does

- Upload a background template image
- Upload an Excel or CSV file
- Generate one A5 page per row
- Print all pages directly from the browser
- Export the generated pages as a PDF

## Supported Data

The tool reads the first sheet from:

- `.xlsx`
- `.xls`
- `.csv`

It expects columns `A` through `G`.

If the first row contains headers named `A`, `B`, `C`, `D`, `E`, `F`, and `G`, those headers will be used.
If not, the file is treated as raw row data in column order.

## How To Use

1. Open [`index.html`](/Users/shameershajahan/Desktop/e2p/index.html) in a web browser.
2. Upload a background image in JPG, PNG, or WebP format.
3. Upload your Excel or CSV file.
4. Review the generated A5 pages.
5. Use `Print All Pages` or `Download PDF (A5)`.

## Notes

- Each spreadsheet row creates one page.
- The layout is optimized for A5 portrait output.
- PDF export uses `html2canvas` and `jsPDF`.
- Spreadsheet parsing uses `SheetJS (xlsx)`.
