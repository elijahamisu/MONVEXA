## 2024-05-18 - Replacing Blocking Alerts with Accessible Status Toasts
**Learning:** Standard browser `alert()` popups disrupt user workflow and block execution. Replacing them with floating toast notifications (`role="status"`, `aria-live="polite"`) delivers a smooth feedback mechanism while keeping the page screen-reader accessible.
**Action:** Always prefer accessible inline or floating toast notifications with proper timeout clearing over browser-native modal alerts when confirming user actions like clipboard copying.
