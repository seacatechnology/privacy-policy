# Privacy Policy for Structured Mail

**Effective Date:** June 2026

Structured Mail is built as a commercial, independent application. This service is provided by the developer at a one-time purchase cost and is designed to be used as-is.

This page is used to inform application users and Google Play reviewers regarding our policies with the collection, use, and disclosure of Personal Information.

---

## 1. Core Philosophy: Zero-Tracking & Absolute Privacy
Because Structured Mail is a decentralized, peer-to-peer (P2P) application, **the developer does not operate centralized servers, does not maintain user registries, and does not collect, track, store, or harvest any personal data, usage metrics, or message content.**

Your data belongs entirely to you. Communication happens directly between your device and your peer endpoints.

## 2. Information Collection and Use
* **Personal Data:** The application does not require user accounts, names, phone numbers, emails, or passwords. Therefore, no personal identity tracking is possible.
* **Message & File Content:** All messages, cryptographic keys, and file attachments are stored locally within your device's isolated application directory (`warehouse`). The developer has zero access to this data.
* **Metadata:** No connection tracking metadata or logs are transmitted to the developer or any third party.

## 3. Data Encryption and Transmission Security
To guarantee secure direct data transit, the application enforces the following protocols by default:
* Peer-to-peer communication is entirely encrypted in transit using **TCP + TLS** architectures. 
* A localized STUN helper utility is integrated to facilitate network connectivity behind Cone NAT configurations. No data payload is exposed during this lookup process. 

## 4. Android Device Permissions
To protect your digital environment, Structured Mail requests minimal, non-intrusive system capabilities:
* **Internet Permission (`INTERNET`):** Required exclusively to establish the localized socket architectures, UDP listening/knocking hooks, and direct TCP peer-to-peer network routing loops.
* **Storage Access Framework (SAF):** The app utilizes native Android SAF system pickers. This allows you to selectively import or export file attachments without granting the application broad, generic read/write access to your entire device storage.

## 5. Third-Party Services
The application does not integrate any third-party SDKs, advertising frameworks, analytics trackers, or centralized cloud notification services. 

## 6. Children’s Privacy
These Services do not address anyone under the age of 13. We do not knowingly collect personally identifiable information from anyone because the application does not collect any data from any user whatsoever.

## 7. Changes to This Privacy Policy
We may update our Privacy Policy from time to time. Thus, you are advised to review this page periodically for any changes. Any updates will be pushed transparently to this public repository.

## 8. Contact Us
If you have any questions or suggestions regarding the structural architecture or privacy compliance of Structured Mail, do not hesitate to contact the developer:

* **Developer Name:** [Seacatechnology]
* **Support Email:** [seacatechnology@gmail.com]
