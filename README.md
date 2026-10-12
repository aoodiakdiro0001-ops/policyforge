# 🛡️ PolicyForge — CSP & CORS Auditor + Generator (MIT)

Deep-audit browser protection policies and generate hardened replacements.
UI in EN/TR/AR. Static single file + README.

## Tools

- **🔍 CSP Audit:** 12 directives graded (default/script/object/base/
  ancestors/form/style/img/connect/font/media/worker) — wildcards,
  unsafe-inline/eval, data:/blob:, http: flagged with fixes. Auto-fetch
  (proxy-visible) + manual paste.
- **🌐 CORS Audit:** detects `*` + credentials (critical), null origin,
  missing Vary, over-broad methods, long preflight cache. Paste server
  config or observed values (browsers hide live CORS headers — stated openly).
- **⚙️ Generator:** 4 answers → strict CSP + nginx/Apache/Express(helmet)
  snippets, report-uri optional.
- **🕵️ Leak Scanner:** proxy-fetched HTML → third-party domains × CSP
  cross-check (blocked vs needs-allowlist).
- **💎 Change Alerts $6/mo:** hash-based header-change detection on watched
  sites + browser alerts; Pro = Telegram (backend required) + payment box.

## Money & contact

- `CONFIG.ads` footer slot.
- Donate + Pro payments: BTC + USDT-TRC20 + IBANs.
- 📧 baranavisat@gmail.com · 📞 +90 531 326 37 22 · WhatsApp

## Run

```bash
cd policyforge
python3 -m http.server 8080
```

## License

MIT. Verify critical configs in staging first.
