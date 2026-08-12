# Palette UX / Accessibility Journal - EASYPIE

## 2025-02-23 - Custom Toast Copy-Notifications and Modals
**Learning:** Browser-native alerts for copy-to-clipboard actions are disruptive and unpolished. Replacing them with custom floating toasts greatly improves micro-UX.
- To handle rapid consecutive clicks safely without flickering or premature hiding, always clear the previous timeout ID using `clearTimeout(toastTimeout)`.
- Custom floating toasts need a very high `z-index` (such as 3000) so they safely render on top of modal backdrop overlays (which typically use `z-index: 2000`).
- Including `role="status"` and `aria-live="polite"` makes the toast notifications fully accessible to screen readers automatically.
- Icon-only buttons (like clipboard copy buttons) always require an explicit `aria-label` to provide the necessary semantic context for non-visual users.
**Action:** Apply these accessible toast and button standards to all dynamic copying/status-reporting UI elements across the application pages.
