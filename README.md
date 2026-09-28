# Chart Lab

A browser-only chart studio for daily intranet work. Open `index.html` to start. No server or build step is required.

## What the MVP does

- Edit a data table, add or delete rows and columns, or paste a rectangular selection from Excel.
- Switch among common chart types and adjust fonts, sizes, colors, labels, axes, titles, and canvas background.
- Present the interactive chart in a clean presentation view.
- Download Excel (`.xlsx`) with editable Data and linked Summary sheets, CSV, PNG, or JPEG.

The Excel Summary has formulas for total, average, highest and lowest of the first selected numeric series. It does not yet contain a native Excel chart. PNG and JPEG are images, so their chart elements are not editable in Office. Native editable PowerPoint chart export is a future phase.

## Hosting and embedding

Upload the complete `chart-lab` folder to a GitHub repository. Configure GitHub Pages to serve from the repository root; its `index.html` opens `dist/index.html`. The scripts under `dist` are bundled locally so chart rendering does not need a public CDN. For an intranet page, add the Pages URL through your SharePoint Embed web part if your tenant permits that domain, or use a normal link.

Chart data stays in browser memory while the page is open. It is not uploaded by this app and is lost on refresh unless downloaded first. Review your organisation's policy before putting real internal data into a publicly reachable site, even though the app itself does not transmit it.
