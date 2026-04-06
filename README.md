# 🛡️ BSS Market Place (bss_bizgroup)
**Core Engine v2.0.8** *A Secure Multi-Tier E-Commerce Ecosystem for Verified Sellers and Buyers.*

---

## 👨‍💻 Developer Information
* **Lead Architect:** Taiwo Fashola
* **Contact:** +234 811 842 8191
* **Platform:** Firebase Cloud + Gemini 3 Flash Logic

---

## 🚀 System Overview
BSS Market Place is a high-integrity trading platform built with a 4-tier security hierarchy. It utilizes real-time Firestore synchronization and automated "Bold ID" advert verification.

### 🔑 Access Tiers & Menus
1. **🔴 Admin Master:** - Seller Verification (Passport/NIN)
   - Subscription Toggles (ON/OFF)
   - Global Transaction & Chat Monitoring
   - System Prompt Management

2. **🟡 Moderator:** - Policy Enforcement & Content Review
   - Dispute Mediation & Conflict Tickets
   - Private Inbox for Support Reports

3. **🟢 Seller Hub:** - Bold ID Advert Posting
   - Stock & Inventory Logic
   - Direct Buyer Negotiation (Private Inbox)
   - Integrity Score Tracking (Target: 5.0 ⭐)

4. **🔵 Buyer Portal:** - Verified Market Search
   - Payment Receipt Upload (Proof of Funds)
   - Delivery Tracking & Arrival Logic
   - Seller Rating & Order Completion

---

## 🛠️ Technical Stack
* **Frontend:** Single Page HTML5/CSS3 (WhatsApp-Style UI)
* **Backend:** Firebase (Authentication & Firestore)
* **Hosting:** Firebase Hosting (Automated via GitHub Actions)
* **Logic:** System Prompt v2.0.8 (bss_bizgroup Isolated)

---

## 📌 Maintenance Notes
- **Database Sync:** Occurs every 30 seconds via Gemini Cloud.
- **Security:** Do not commit `apiKey` directly to public branches (Use Environment Variables or Keep Repo Private).
- **Updates:** Any changes to `index.html` on the `main` branch will auto-deploy to the live site.
