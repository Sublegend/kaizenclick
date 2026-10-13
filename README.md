# KaizenClick

A time study tool that runs in your browser. Tap **SPLIT** as an operator finishes each work element, and get a clean sheet of element times, running totals and (optionally) the manpower needed to hit TAKT. Built for iPad, works on phones and desktops.

**Live app: https://sublegend.github.io/kaizenclick/**

No install, no account. Your data stays on your device.

## How to use it

1. **Set up.** Enter the operation and operator, then tap **START STUDY**. Add TAKT time if you want manpower calculated.
2. **Capture.** Tap **SPLIT** at the end of each element, name it (tap a suggestion or type), and save. Use **PAUSE** for interruptions and **+ADD** to enter a missed element by hand. Tap **END** when finished.
3. **Review.** Tap any name, time or detail to edit it. Drag the ≡ grip to reorder. Tap the bin to delete a row.
4. **Share.** **Share** sends the sheet as a **PDF** or **Excel** file (email, Messages, Drive, etc.). The PDF fits one page when it can and otherwise paginates. To print, share the PDF and choose **Print** from the share sheet (or open the downloaded PDF on a desktop). **Resume** goes back to capturing; **New** starts another study.

## Studies

You can keep several studies on the device and switch between them. Tap the study name in the top-right corner to open the list.

- **Switch** by tapping a study. A study whose clock is running keeps running in the background (a green dot on the header button shows this).
- **New study** opens setup without touching the others.
- **Delete** a study with its bin icon, or clear out all finished ones with **Delete finished**.
- **Search** appears once you have more than five studies.

### Import and back up

Studies are kept in the browser, which IT policies or a cleanup can wipe, so treat a shared file as the real copy.

- **Excel exports can be imported.** An Excel file shared from the app carries the full study in a hidden sheet. **Import** (in the studies list) brings it back exactly, with notes, options and custom fields. If you changed element names or times in Excel, those edits are used. Older exports without the hidden sheet are read from the visible sheet. PDFs can't be imported.
- **Back up all** puts every study into one Excel file to email or save. Importing it restores them all (studies already on the device are skipped). The list shows when you last backed up.

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

- **Auto-recovery.** If the tab closes mid-study, reopening brings back every study and the one you had open. Clocks come back paused.
- **Studies live in this browser only.** Clearing browsing data (or a work device's cleanup policy) deletes them. Share any study you need to keep. On iPad, add the app to the Home Screen so Safari doesn't clear it after a week without use.
- **Pausing** stops the whole study clock, not just the current split.
- **Reset the split.** While paused, tap the green SPLIT clock at the top to set the current split back to 0:00 (handy if the clock ran when it should have been paused). That time also comes off the elapsed clock.
- **Internet needed to load.** The page pulls its styling, icons and Excel library from CDNs. Data is never sent anywhere.
- **Share** needs the page served over HTTPS (for example GitHub Pages). Where sharing isn't available, it downloads the file instead. The PDF library loads the first time you open the review screen, so that needs a connection.

## Run it

Open `index.html` in a browser, or host the file on any static site (GitHub Pages works). To test locally:

```bash
python -m http.server 8000
```

## License

[MIT](LICENSE)
