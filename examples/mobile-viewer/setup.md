Minimal setup to get `mobile-viewer` working on mobile Safari. Need to provide:

[for `viewer.html`]
– `pdfjs-dist/web/pdf_viewer.css` (which itself is built from `pdf.js/web/pdf_viewer.css`, importing `pdf.js/web/text_layer_builder.css` & `pdf.js/web/annotation_layer_builder.css`)
– `pdfjs-dist/build/pdf.js` (identical to `pdf.js/build/generic/build/pdf.js`)
– `pdfjs-dist/web/pdf_viewer.js` (possibly `pdf.js/build/generic/web/pdf_viewer.js` despite the former using `__w_pdfjs_require__` while the latter uses `__webpack_require__`)

[for viewer.js]
– `../../node_modules/pdfjs-dist/build/pdf.worker.js` (identical to `pdf.js/build/generic/build/pdf.worker.js`)
– `../../node_modules/pdfjs-dist/cmaps` (identical to `pdf.js/build/generic/build/web/cmaps`)