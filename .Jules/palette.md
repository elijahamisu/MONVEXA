# Palette UX/Accessibility Journal

## 2025-02-14 - Accessible Floating Toast Copy Notifications
**Learning:** Browser-native alert dialogs are abrasive and disrupt screen readers and user flows. Replacing copy-to-clipboard alerts with floating toast notifications containing `role="status"` and `aria-live="polite"` improves overall accessibility, visual feedback, and user retention. When implementing copy indicators, z-index must be set to `3000` (above modal overlays) and consecutive clicks must be handled using `clearTimeout(toastTimeout)` to prevent rapid successions from closing the notification prematurely.
**Action:** Always include a custom toast display function with `clearTimeout` reset, high z-index, and appropriate ARIA attributes for clipboard copy and status actions on standalone pages.
