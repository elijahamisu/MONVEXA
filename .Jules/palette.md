## 2025-02-20 - Non-disruptive copy feedback and accessible toast announcements
**Learning:** Browser-native alert dialogs disrupt user interaction flow when copying referral codes or IDs. Providing an in-page toast notification with `role="status"` and `aria-live="polite"` improves keyboard/screen reader announcements while preserving smooth visual experience.
**Action:** Always replace `alert()` calls on user copy actions with floating toast feedback elements equipped with polite live region accessibility attributes.
