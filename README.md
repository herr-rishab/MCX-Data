# MCX

Clean, fast, and focused market intelligence for MCX—built in Flutter for mobile and web.

---

## ✨ Highlights
- **Daily Margin**: today + previous day, with Total, Prev Total, and Difference per contract
- **Market Watch**: FUTCOM expiries with consecutive‑expiry LTP spreads
- **Curated universe**: ALUMINI, COPPER, CRUDEOIL, GOLD, LEAD, NATURALGAS, NICKEL, SILVER, ZINC
- **Web‑ready UI**: responsive layout, clean cards, instant filters

---

## 📱 Screens
- Daily Margin
- Market Watch

---

## 🧮 Calculation logic
- **Total** = Initial + ELM + Tender + Delivery + Add L/S + Spec L/S + Daily Vol + Annual Vol  
- **Prev Total** = previous day’s same symbol + expiry (normalized expiry key), same formula  
- **Difference** = Total − Prev Total

---

## 🚀 Quickstart
```bash
flutter pub get
flutter run
```

## 🌐 Build for web
```bash
flutter build web
```

---


## 🔒 Notes
- Data is pulled from MCX endpoints.
- For web, a proxy may be required if CORS blocks requests.

---

## ✅ Status
Stable and hosted at https://datamcx.pages.dev/
