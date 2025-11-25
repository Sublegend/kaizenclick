# KaizenClick Time Study Tool

KaizenClick is a modern, web-based time study application designed to help industrial engineers and process analysts capture, analyze, and optimize process times with ease. Built with a focus on usability and mobile responsiveness, it replaces traditional stopwatch-and-clipboard methods with a digital, touch-friendly interface.

## Features

*   **Study Setup**: Quickly define operation details, operator, department, and takt time.
*   **Digital Stopwatch**: Large, high-contrast timer display with millisecond precision.
*   **Split/Lap Recording**: "Tap to Capture" interface optimized for touchscreens to record element times without looking away from the process. **Note: Split times are automatically rounded up to the nearest 15 seconds.**
*   **Review & Edit**: Drag-and-drop interface to reorder elements, edit descriptions, and adjust times.
*   **Data Export**: Export study data directly to Excel (.xlsx) for further analysis.
*   **Print-Ready Reports**: Generates a clean "Standard Work Combination Sheet" layout for printing or saving as PDF.
*   **Local Storage**: Automatically saves study metadata to the browser's local storage for quick reuse.

## Technologies Used

*   **HTML5 & CSS3**: Core structure and styling.
*   **Tailwind CSS**: Utility-first CSS framework for rapid, responsive UI design.
*   **JavaScript (ES6+)**: Application logic, timer precision, and state management.
*   **SheetJS (xlsx)**: Client-side Excel export functionality.
*   **FontAwesome**: Iconography.

## Usage Guide

1.  **Setup**: Open the app and fill in the study details (Operation, Operator, etc.). Click **START STUDY**.
2.  **Timing**:
    *   The timer starts immediately.
    *   Tap the large **SPLIT** button to record the end of an element and start the next one.
    *   Use **PAUSE** if the process is interrupted.
    *   Click **END STUDY** when finished.
3.  **Review**:
    *   The app switches to the Review View.
    *   **Edit**: Click on any description or time to edit it.
    *   **Reorder**: Drag rows using the handle on the left to correct the sequence.
    *   **Add Elements**: Insert missed elements manually.
4.  **Export/Print**: Use the buttons at the bottom to **Export XLSX** or **Print** the report.

## Installation

No installation required! Just open `index.html` in any modern web browser.

## License

[MIT](LICENSE)
