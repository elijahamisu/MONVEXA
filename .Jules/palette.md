# Palette UX Journal

This journal tracks critical UX/accessibility learnings for the EASYPIE platform.

## 2024-08-13 - [Non-Disruptive Copy Feedback & Icon accessibility]
**Learning:** Browser-native alert dialogs are highly disruptive, breaking premium visual flows. Replacing them with accessible floating toasts (`role="status"`, `aria-live="polite"`, high `z-index: 3000`) and properly managing rapid successive clicks via `clearTimeout` elevates user interaction immensely. Additionally, interactive header icon-only buttons need precise `aria-label`s to be screen-reader compliant.
**Action:** Always replace `alert()` with a robust custom toast and add standard `aria-label` attributes on icon-only header/navigation elements.
