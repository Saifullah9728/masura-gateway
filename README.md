# 🌐 Masura Dynamic Endpoint Gateway

Official Cryptographic Discovery & Route Resolution Endpoint for **Masura Systems**, **Masura CineControl Pro**, **MASURA DCP Player**, and all MASURA Enterprise Desktop Suites.

## 📌 Active Endpoint Configuration
- **Live Portal URL (`active_portal_url`):** https://ais-pre-zqb5gcscwnuji4fpncpxdv-132219187393.asia-southeast1.run.app
- **Development / Mirror URL:** https://ais-dev-zqb5gcscwnuji4fpncpxdv-132219187393.asia-southeast1.run.app
- **Backup Endpoint:** https://masura.vercel.app
- **Service Status:** Online (Operational · v2.0.0)
- **Integrity Validation:** RSA-4096 `domainRouterSignature` (`SIG-MSR-PEM-A15F5794FCC28024`)
- **Public Key ID:** `v2026.3-RSA4096`

## 🔐 Live Desktop Licensing API Routes
- **License Activation:** `POST /api/license/activate`
- **Periodic Heartbeat Validation:** `POST /api/license/validate`
- **1-PC Free Trial Lock & Verify:** `POST /api/license/trial-verify`
- **Cryptographic UTC Time Authority:** `GET /api/license/time`
- **Gateway Health Status:** `GET /api/health`

---
*Maintained by Masura Systems. Dedicated to Muhammad Ali Saifullah & Most. Sahida Khatun.*
