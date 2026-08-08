## 2026-03-01 - [Polished Clipboard Copy Alerts with Accessible Toasts]
**Learning:** Browser native alerts interrupt user focus and degrade a premium investment platform experience. High z-index toasts with `role="status"` and `aria-live="polite"` provide excellent non-disruptive feedback, while managing `clearTimeout` ensures proper behavior on successive rapid clicks.
**Action:** Replace native copy `alert()` prompts with high z-index (3000), accessible status-live toasts equipped with timeout safety across the app.
