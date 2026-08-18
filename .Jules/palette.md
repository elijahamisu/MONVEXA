# Palette's Journal - Critical UX & Accessibility Learnings

## 2025-05-18 - Non-disruptive feedback for copy actions
**Learning:** Browser native `alert()` popups disrupt user workflow when copying codes or links. Inline visual feedback (icon transition to checkmark) provides clear, accessible acknowledgment without interrupting user focus.
**Action:** Use inline icon state changes or accessible toasts for copy-to-clipboard interactions instead of `alert()`.
