# Components & Interaction

## Theme & Component Consistency

- **Theme Alignment:** Ensure combo boxes, spinners, and tooltips follow the application's UI theme.
- **Toggle-to-Combobox Threshold:** If a mutually exclusive toggle switch or segmented control (such as a metric or display-mode selector) has four or more options, switch to a combo box. (Multi-select filter chips and quick-navigation presets may instead use a single-row scrollable bar.)
- **Consolidate Duplicate Controls:** UI elements performing the same function within a single modal should be consolidated.
- **Combine Redundant Symbols & Text:** Merge visually redundant icons, symbols, and labels that convey the exact same meaning.

## Overlays & Interactive Canvases

- **Consistent Overlay Dismissal:** All modals, popovers, and comboboxes should close consistently on both `Escape` key press and outside click.
- **Isolate Events on Interactive Canvases:** Floating UI controls and cards placed over draggable/zoomable 3D canvases or maps must isolate pointer and wheel events so interacting with UI buttons does not accidentally pan or rotate the canvas.
- **Safe Clearance for Floating Controls:** Maintain clear visual spacing (e.g., `16px+`) between floating buttons and adjacent bottom bars, and smoothly reposition floating controls when adjacent bars are hidden in other view modes.
- **Intentional Selection & Cursor Control:** Suppress unintended text selection (`user-select: none`) and caret blinking on interactive chrome (buttons, tabs, and draggable canvases/maps), while preserving normal text selection on readable content (articles, table values, and error messages) as well as normal caret and selection behavior inside `input` and `textarea` elements, and applying `cursor: pointer` to interactive controls.
