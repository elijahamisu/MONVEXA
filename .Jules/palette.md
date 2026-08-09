# Palette's Journal - Critical Learnings

## 2026-03-01 - Premium Clipboard-Copy Experience

**Learning:** Browser-native copy alerts disrupt the premium mobile-first dark-theme user experience. Replacing alert() with an inline, styled floating toast notification maintains the immersive, luxury aesthetic of the app and handles rapid succession copying gracefully.
**Action:** Replace `alert()` inside `dashboard.html` with a custom floating toast that mimics the existing styled toast design in referrals and deposits pages.
