# Palette's Journal

Critical UX/accessibility learnings for the EASYPIE design system are maintained here.

## 2026-10-24 - Premium Non-Disruptive Clipboard Copy Notifications & Accessibility
**Learning:** Replacing blocking, thread-disruptive browser-native `alert()` dialogs with lightweight, floating CSS toast notifications significantly enhances the premium, luxury feel of the application. To ensure full accessibility and robustness, any copy toast must have `role="status"` and `aria-live="polite"` attributes, set a high `z-index` (e.g., 3000) to float above standard overlay components, and handle rapid succession copying by resetting previous transitions via `clearTimeout()`. Icon-only buttons (such as notification icons, logout buttons, and copy buttons) must also have explicit `aria-label` tags to maintain keyboard/screen-reader accessibility.
**Action:** Replace all native copy-confirm dialogs with custom accessible floating toasts, always use `clearTimeout` for rapid click handling, and add `aria-label` to all icon-only elements.
