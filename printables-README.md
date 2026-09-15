# Printables

Put worksheet PDFs here, one folder per theme, using these exact names:

```
printables/
  football/   colouring.pdf  writing.pdf  reading.pdf
  sea/        colouring.pdf  writing.pdf  reading.pdf
  farm/       ...
  road/
  space/
  food/
  dojo/
  dino/
  bugs/
```

The folder name must match the theme id exactly: `football`, `sea`, `farm`,
`road`, `space`, `food`, `dojo`, `dino`, `bugs`.

Then open `index.html`, find the `PRINTABLES` block near the top of the script,
and uncomment or add a line for each theme listing the sheets that exist:

```js
var PRINTABLES = {
  football: ["colouring", "writing", "reading"],
  sea:      ["colouring"],
};
```

Only the sheets you list get a button, so a missing PDF can never produce a
broken link. Buttons appear under the three game cards on that theme's screen.

## Making the PDFs

- A4 portrait, so they print without scaling on a UK printer
- Colouring pages: thick black outlines, no fills, no grey shading
- Keep a 10mm margin — home printers cannot print to the edge
- Aim for under about 1MB each so the repo stays quick to clone
