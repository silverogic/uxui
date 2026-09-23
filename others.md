### The 4 Core Principles (POUR)

> [!NOTE]
> All UI components should satisfy the POUR principles.

1. **Perceivable:** Information and UI components must be presentable to users in ways they can perceive (alt text, captions, color contrast).
2. **Operable:** User interface components and navigation must be operable (keyboard navigation, sufficient touch targets, no seizure-inducing flashes).
3. **Understandable:** Information and the operation of user interface must be understandable (consistent navigation, clear error messages).
4. **Robust:** Content must be robust enough that it can be interpreted reliably by a wide variety of user agents, including assistive technologies.

### Conformance Levels (Level A, AA, AAA)

- **Level A:** Minimum essential requirement (failure blocks access for some users).
- **Level AA:** **Global industry standard** (target level for most legal compliance and enterprise products).
- **Level AAA:** Highest level of accessibility (specialized or niche accessibility applications).

### Visual UI Design

> [!IMPORTANT]
> **Color Contrast Ratios (WCAG 2.1 Level AA)**
> - **Body Text:** At least **4.5 : 1** against background
> - **Large Text (18pt+ or 14pt+ Bold):** At least **3 : 1** against background
> - **UI Components (Buttons, Input Borders, Icons):** At least **3 : 1** against background

- **Multi-modal Signals:** Never rely solely on color to convey status (e.g., pair red error borders with an **alert icon + descriptive text**).
- **Typography & Spacing:** Maintain line height at least `1.5x` font size, and paragraph spacing at least `2x` font size.
- **Text Reflow (200% Zoom):** Ensure layout does not break when users zoom text up to 200%.

### Others

Ensure that elements within the grid do not extend beyond the grid boundaries.

Make sure the combo box design follows the app's theme.

If a toggle switch has four or more options, switch to a combo box.

UI elements performing the same function within a single modal should be consolidated.

Ensure that the table contents do not extend beyond the table boundaries.

Combine visually redundant symbols and text that share the same meaning.
