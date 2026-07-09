# KaizenClick Time Study Tool (v2.0)

KaizenClick is a modern, responsive, client-side web application designed for industrial engineers and lean practitioners to conduct time studies. By replacing stopwatches and clipboards, KaizenClick simplifies recording, sequencing, and calculating standard work combination metrics directly on mobile tablets or desktop screens.

---

## Key Features (v2.0)

### Real-time Capture & Timing
*   **High-Contrast Timer**: Live stopwatch tracking total elapsed study time and the current split time.
*   **One-Tap Splits**: Large, thumb-friendly **SPLIT** button to record the end of a work element. Split times are automatically rounded up to the nearest 15-second increment.
*   **Inline Pause/Resume**: Pause the main timer at any time—either from the control bar or directly inside the description modal—to handle process interruptions.

### Smart Suggestions & Setup
*   **Default Elements (Chips)**: Pre-define standard work steps on the setup screen. Rearrange them via drag-and-drop, or add/remove them dynamically.
*   **Auto-Autocomplete Datalist**: Defined chips are loaded directly into the element description datalist for ultra-fast selection during active capture.

### Robust Persistence & Safeguards
*   **Active Session Recovery**: Automatic state backups to `localStorage`. If you close the browser tab or refresh the page, a prompt allows you to resume your study exactly where you left off.
*   **Double-Safe Confirmation Dialogs**: Custom prompts alert you before ending a capture, discarding data, starting a new session, or deleting data rows.

### Interactive Data Sheet
*   **Drag-and-Drop Sequencing**: Reorder captured elements in real-time. The indices and cumulative times update automatically.
*   **In-Place Editing**: Correct work element names and adjust times directly inside the data sheet by clicking on the cell.
*   **Manual Entry**: Insert missed elements manually during either the active capture phase or the final review phase.

### Automated Lean Metrics
*   **Manpower Calculation**: Automatically calculates the required operator headcount based on the target **TAKT time** and **Total Element Time**.
*   **Excel Export**: Download the entire study with formatted headers, metadata, raw durations, total element time, and total elapsed time using [SheetJS](https://sheetjs.com/).
*   **Standard Work Combination Sheet (Print/PDF)**: Clean CSS styling transforms the screen into a formal lean print template for hardcopy documentation or PDF saving.

---

## Tech Stack

*   **HTML5 & CSS3**: Document structure and customized print stylesheets.
*   **Tailwind CSS**: Utility-first CSS framework for responsive layout design.
*   **JavaScript (Vanilla ES6)**: Application state engine, custom timer precision loops, and drag-and-drop APIs.
*   **SheetJS (XLSX)**: Client-side binary generation for spreadsheet exports.
*   **FontAwesome**: Modern iconography.
*   **Google Fonts**: Inter typography.

---

## Usage Guide

### 1. Study Setup
- Open `index.html` in any modern web browser (mobile tablet recommended).
- Enter the **Operation / Process**, **Operator**, **Department**, **TAKT Time (min)**, and **Analyst**.
- Pre-populate work steps in the **Default Elements** chip list. Click **START STUDY**.

### 2. Live Capture
- Tap **SPLIT** when the operator finishes a work step.
- Fill in the description (uses default elements datalist) and save to log it.
- Tap **PAUSE TIMER** in the modal or **PAUSE** on the bottom bar to handle non-cyclical delays.
- Tap **END** on the bottom bar and confirm to transition to Review Mode.

### 3. Review & Edit
- **Correct description/time**: Double-click or tap on any cell inside the data sheet.
- **Reorder**: Press and drag the grip handles on the left of each row to correct the sequence.
- **Delete**: Click the trash icon to remove a row.
- **Add**: Use the **Add Element** button to manually insert elements.

### 4. Share & Document
- **Export XLSX**: Generate a formatted Excel workbook.
- **Print**: Print a clean Standard Work Combination Sheet, or save it directly to PDF.
- **Start New**: Clear current session data and return to the Setup screen.

---

## Installation & Deployment

No complex installation is necessary:
1. Clone or download the repository.
2. Double-click `index.html` or open it from your browser of choice.
3. For local development or testing, serve using any basic HTTP server:
   ```bash
   # Python 3
   python -m http.server 8000
   ```

---

## License

This project is licensed under the [MIT License](LICENSE).
