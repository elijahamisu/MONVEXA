# Palette UX & Accessibility Journal 🎨

Critical UX, accessibility, and interaction learnings maintained for the design system.

## 2026-10-24 - Non-disruptive feedback on copy actions
**Learning:** Browser-native alerts disrupt the user flow and block the execution thread on premium interfaces. Integrating a silent visual or floating toast feedback system yields a far more professional and fluid feel. Additionally, icon-only buttons need explicit `aria-label` tags to retain complete screen reader accessibility.
**Action:** Replace `alert()` methods with animated toast notifications or clear inline state indicators on key interactive items, and ensure all icon buttons have clean `aria-label` definitions.
