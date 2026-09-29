# KaizenClick

A time study tool that runs in your browser. Tap **SPLIT** as an operator finishes each work element, and get a clean sheet of element times, running totals and (optionally) the manpower needed to hit TAKT. Built for iPad, works on phones and desktops.

**Live app: https://sublegend.github.io/kaizenclick/**

No install, no account. Your data stays on your device.

## How to use it

1. **Set up.** Enter the operation and operator, then tap **START STUDY**. Add TAKT time if you want manpower calculated.
2. **Capture.** Tap **SPLIT** at the end of each element, name it (tap a suggestion or type), and save. Use **PAUSE** for interruptions and **+ADD** to enter a missed element by hand. Tap **END** when finished.
3. **Review.** Tap any name, time or detail to edit it. Drag the ≡ grip to reorder. Tap the bin to delete a row.
4. **Share.** **Share** sends the sheet as a **PDF** or **Excel** file (email, Messages, Drive, etc.). The PDF fits one page when it can and otherwise paginates. **Print** uses your browser's print dialog. **Resume** goes back to capturing; **New** starts over.

## Options

Choose on the setup screen. The **Show** chips on the sheet turn Manpower, Cumulative and Notes on or off at any time.

| Option | What it does |
| --- | --- |
| Manpower / TAKT | TAKT field, manpower figure, and a total-vs-TAKT bar |
| Cumulative time & bars | Running-total column and a bar under each element showing its length |
| Element notes | A note line under each element |
| Round splits to | 15, 5 or 1 second (default 15) |
| Custom fields | Extra header details such as Part No. or Shift |

## Good to know

- **Auto-recovery.** If the tab closes mid-study, reopening offers to resume. The clock comes back paused.
- **Pausing** stops the whole study clock, not just the current split.
- **Internet needed to load.** The page pulls its styling, icons and Excel library from CDNs. Data is never sent anywhere.
- **Share** needs the page served over HTTPS (for example GitHub Pages). Where sharing isn't available, it downloads the file instead. The PDF library loads the first time you open the review screen, so that needs a connection.

## Run it

Open `index.html` in a browser, or host the file on any static site (GitHub Pages works). To test locally:

```bash
python -m http.server 8000
```

## License

[MIT](LICENSE)
