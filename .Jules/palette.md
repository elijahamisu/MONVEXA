# Palette's UX Journal

## 2024-11-20 - Non-disruptive copy actions and screen reader support
**Learning:** Browser native popups (such as alert()) are highly disruptive to user experience on premium platforms. Replacing them with custom floating toast notifications with proper role="status" and aria-live="polite" attributes makes copying actions non-disruptive and fully accessible to screen reader users. Additionally, clearing previous timeouts ensures rapid successive clicks are handled correctly.
**Action:** Replace all native alert-based copy actions with accessible styled toasts that use role="status" and aria-live="polite", keeping z-index high (such as 3000) to clear overlay elements, and clear previous timeouts to handle rapid clicks.
