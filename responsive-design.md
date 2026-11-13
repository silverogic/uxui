# Responsive Design

## Layout & Viewport

- **Preserve Breathing Room on Mobile:** In narrow mobile environments, reduce padding and save horizontal cell space to provide a sense of openness.
- **Fallback for Long Brand/Logo Titles:** If a logo title is too long and gets cut off, ensure at least the icon is displayed cleanly.
- **Compress Secondary & Floating Controls:** On narrow mobile viewports, compress secondary or floating controls by hiding redundant icons or secondary labels (e.g., showing text-only `2D`/`3D` pills) to maximize canvas and content visibility.
- **Differentiate Density by Viewport:** Show only core markers/labels on mobile and reserve denser auxiliary markers (`desktopOnly`) for wider desktop screens to prevent label overlap.
- **Single-Row Horizontal Scroll for Filter/Preset Bars:** Keep multi-select filter chips and quick-navigation preset bars on a single horizontally scrollable row (`overflow-x-auto`) on mobile instead of wrapping into multiple lines; when hiding the scrollbar, preserve visual overflow cues (such as edge fade or partially visible chips) and ensure keyboard focus scrolls items into view.
- **Tokenize Fixed Header & Dock Heights:** Manage fixed header, search dock, and table header heights with CSS variables so `scroll-padding-top` adapts accurately across breakpoints; on very short viewports or 200% text zoom, allow secondary search docks to unstick or compact so data rows remain readable.

## Responsive Tables

- **Prevent Table Clipping:** Ensure that tables are not cut off horizontally or vertically.
- **Keep Fixed Dock Visible:** Make the table's fixed dock (header/search bar) clearly visible while scrolling.
- **Position Data Rows Below the Dock:** Ensure that data rows and anchor-scrolled rows are always positioned cleanly below the fixed dock.
- **Sticky Leading Columns:** When table content exceeds the horizontal screen width, designate the first two columns as sticky columns and allow horizontal swipe/scroll for the remaining columns.
