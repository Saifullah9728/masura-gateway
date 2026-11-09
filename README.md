# MASURA Systems — Dynamic Licensing, Auto-Update & Cloud Gateway (`masura-gateway`)

Official dynamic endpoint router, cryptographic signature authority, and software version manifest for the **MASURA** desktop software ecosystem (Windows, macOS, and Linux).

---

## 🌐 Live Production Portal & Cloud Endpoints

- **Official Website & Licensing Portal:** [https://masura.ai.studio](https://masura.ai.studio)
- **Primary Discovery Manifest (`endpoint.json`):** `https://raw.githubusercontent.com/Saifullah9728/masura-gateway/main/endpoint.json`
- **Mirror Gateway Manifest (`api_gateway.json`):** `https://raw.githubusercontent.com/Saifullah9728/masura-gateway/main/api_gateway.json`
- **Direct Cloud Firestore REST Gateway (Layer-2 Failsafe):** `https://firestore.googleapis.com/v1/projects/scientific-rigging-k53bd/databases/ai-studio-9531feab-88e4-44e4-9f9a-e06f64ef4c64/documents`

---

## 🛡️ 4-Layer Connection Ring & 10-Layer Anti-Crack Security

All MASURA desktop applications (compiled to native C/C++ machine binaries via Cython) connect through a 4-layer failsafe architecture:

1. **Layer 1 — Primary Portal API (`https://masura.ai.studio/api/license/*`):**
   - `GET /api/license/time` — Authoritative UTC Network Time
   - `POST /api/license/trial-verify` — 1-Time Per-PC Hardware-Locked Trial Verification
   - `POST /api/license/activate` — Challenge-Response Nonce Activation & AES-256 Engine Seed Release
   - `POST /api/license/unbind` — Online Machine Deactivation (Quota & Cooldown Enforced)
   - `POST /api/license/verify-offline-unbind` — Cryptographic `.msru` Offline Deactivation Receipt Verification
   - `POST /api/license/report-tamper` — Zero-Tolerance Anti-Crack Auto-Revocation
2. **Layer 2 — Direct Google Cloud Firestore REST Gateway (`server: ESF`):**
   - Zero-downtime direct validation against `/licenses/{licenseKey}`, `/trial_machines/{lockId}`, and `/settings/global`.
3. **Layer 3 — Signed GitHub Discovery & Software Update Manifest:**
   - Verified via `domainRouterSignature` (`SIG-MSR-PEM-D0FCA519C24C2DBB`) using each application's embedded `public.pem`.
4. **Layer 4 — Hardware-Bound Encrypted Offline Lease (`license.enc`):**
   - Protected by `HWID-MSR-XXXXXXXX` (Motherboard UUID + CPU Signature + Primary Disk Serial) and monotonic UTC clock-rollback guards.

---

## 📦 Supported Flagship Software Products

| Product ID | Prefix | Software Name | Current Release |
| :--- | :--- | :--- | :--- |
| `cinecontrol-pro` | `CINE` | **MASURA CineControl Pro** | `v4.8.2 Enterprise` |
| `dcp-player` | `DCPP` | **MASURA DCP Player** | `v3.6.0 Studio` |
| `dcp-converter` | `DCPC` | **MASURA DCP Converter** | `v4.2.1 Mastering` |
| `file-server` | `FSERV` | **MASURA File Server** | `v3.9.4 RackCore` |
| `masura-editor` | `EDIT` | **MASURA Editor** | `v2.7.0 Finishing` |
| `media-player` | `MPLAY` | **MASURA Media Player** | `v5.1.0 Ultra` |
| `cinema-playout-server` | `PLAYOUT` | **MASURA Cinema Playout Server** | `v4.5.0 MasterNode` |

---

## 📞 Support & Commercial Licensing

- **Portal:** [https://masura.ai.studio](https://masura.ai.studio)
- **WhatsApp Direct Support:** `+8801303849728`
- **Email:** `hmdasaifullah28@gmail.com`

© 2026 MASURA Systems. All rights reserved.
