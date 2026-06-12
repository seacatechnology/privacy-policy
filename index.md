# Privacy Policy for Structured Mail

**Effective Date:** June 2026

Structured Mail is built as a commercial, independent application. This service is provided by the developer at a one-time purchase cost and is designed to be used as-is.

This page is used to inform application users and Google Play reviewers regarding our policies with the collection, use, and disclosure of Personal Information.

---

## 1. Core Philosophy: Zero-Tracking & Privacy-focused
Because Structured Mail is a decentralized, peer-to-peer (P2P) application, **the developer does not operate centralized messaging servers, maintain user registries, or intentionally collect message content, user accounts, or usage analytics through developer-operated infrastructure.**

## 2. Information Collection and Use
* **Personal Data:** The application does not require user accounts, names, phone numbers, emails, or passwords.
* **Message & File Content:** All messages, cryptographic keys, and file attachments are stored locally within your device's isolated application directory (`warehouse`). The developer does not operate infrastructure capable of accessing this data
* **Metadata:** Structured Mail does not transmit connection logs, message content, or usage analytics to developer-operated infrastructure.

## 3. Data Encryption and Transmission Security
To guarantee secure direct data transit, the application enforces the following protocols by default:
* Peer-to-peer communication is entirely encrypted in transit using **TCP + TLS** architectures. 
* A localized STUN helper utility is integrated to facilitate network connectivity behind Cone NAT configurations. STUN is used solely to discover network reachability information required for peer-to-peer connectivity. Message content and file data are not transmitted through STUN services.

## 4. Third-Party Services
The application does not integrate any third-party SDKs, advertising frameworks, analytics trackers, or centralized cloud notification services. 

## 5. Android Device Permissions
To protect your digital environment, Structured Mail requests minimal, non-intrusive system capabilities:
* **Internet Permission (`INTERNET`):** Required exclusively to establish the localized socket architectures, UDP listening/knocking hooks, and direct TCP peer-to-peer network routing loops.
* **Storage Access Framework (SAF):** The app utilizes native Android SAF system pickers. This allows you to selectively import or export file attachments without granting the application broad, generic read/write access to your entire device storage.

## 6. Children’s Privacy
These Services do not address anyone under the age of 13. We do not knowingly collect personally identifiable information from anyone because Structured Mail does not require user accounts and does not intentionally collect personal information through developer-operated infrastructure.

## 7. Network Limitations
Structured Mail relies on direct peer-to-peer connectivity. Some network environments, particularly those using Symmetric NAT configurations or restrictive firewalls, may prevent direct connections from being established.

## 8. Peer-to-Peer Communication
Structured Mail is a peer-to-peer application. When you communicate with another peer, network information necessary to establish a direct connection (such as IP addresses and port information) may be visible to participating peers as part of the normal operation of Internet protocols.

The developer does not collect or receive this information through developer-operated infrastructure.

## 9. Changes to This Privacy Policy
We may update our Privacy Policy from time to time. Thus, you are advised to review this page periodically for any changes. Any updates will be pushed transparently to this public repository.

## 10. Contact Us
If you have any questions or suggestions regarding the structural architecture or privacy compliance of Structured Mail, do not hesitate to contact the developer:

* **Developer Name:** [Seacatechnology]
* **Support Email:** [seacatechnology@gmail.com]
