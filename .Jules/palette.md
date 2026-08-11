# Palette's Journal - Critical Learnings

## 2024-10-24 - [Clipboard Toast Accessibility]
**Learning:** Toast notifications triggered by copying content to clipboard need explicit ARIA role="status" and aria-live="polite" attributes to ensure screen readers announce them properly. Rapid copy events can cause toasts to overlap or fail to dismiss correctly if timeouts aren't managed.
**Action:** Always include ARIA attributes on Toast notifications and clear previous timeouts to handle rapid succession of copy actions gracefully.
