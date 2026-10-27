# Privacy Policy for Structured Mail

**Effective Date:** October 27, 2026

Structured Mail is an independently developed application for direct peer-to-peer communication, file handling, and local information organization. The app is free to use. The Android version may offer optional, one-time developer-support purchases through Google Play Billing; these payments are voluntary and do not unlock app features.

This Privacy Policy explains what information Structured Mail processes, where it is stored, and when it may be disclosed to peers or third-party service providers. It applies to the Android and desktop versions. Sections that apply only to Android are identified accordingly.

---

## 1. Privacy-Focused, Local-First Design

Structured Mail does not require users to create an account with the developer. It does not require a phone number, email address, or password to establish a developer-operated account, and the developer does not operate a centralized user registry or messaging relay for the app.

The app is designed to keep application data on users' devices and to communicate directly with peers where a connection can be established. The developer does not operate an app-usage analytics or advertising service and does not intentionally collect message content through developer-operated infrastructure.

This does not mean that no technical information is processed during communication. A peer, a local-network discovery mechanism, an Internet service provider, or a third-party connectivity service may observe information necessary for networking, as explained below.

## 2. Information Processed and Stored

### Information stored locally

Depending on the features you use, Structured Mail stores information on your device, including:

- Messages and message-related records, saved-peer information, and local communication state.
- The local knowledge graph, including its nodes and relationships.
- Files and attachments that you place in or receive into the app's Warehouse, together with related metadata.
- App settings, peer-trust decisions, identity material, and other secrets needed for the app to operate.

The app uses separate encrypted local databases for message/peer records, mail records, and knowledge-graph data. Warehouse file contents and their authenticated metadata are protected using application-level file encryption. On Android, app secrets are stored using Android Keystore-backed encryption mechanisms; whether the device provides hardware-backed key protection depends on the device. Desktop protection also depends on the platform's facilities and the app's storage configuration.

Some filesystem metadata may remain visible. For example, a Warehouse object's logical filename and ciphertext size may be visible even when its contents and authenticated metadata are encrypted. Data may also be exposed if a device or app session is compromised, if someone has access to an unlocked device, or if you export or copy data outside the app's protected storage.

### Information sent to peers

When you send a message or file, the relevant content is transmitted to the peer you selected or otherwise authorized to communicate with. That peer may store, copy, disclose, or forward the content independently of the developer. Deleting a local copy does not delete copies already received by another peer.

### Information the developer collects

The developer does not operate a service that receives or stores the app's messages, attachments, local knowledge graph, or general usage analytics. Structured Mail does not intentionally send these contents to developer-operated analytics or advertising infrastructure.

## 3. Network Communication and Metadata

Structured Mail can use different communication methods according to the available network and device capabilities:

- **Direct IP communication:** When a direct IP connection can be established, peers communicate without routing message content through a developer-operated messaging relay. IP addresses and port information are required to establish network connections.
- **Local-network discovery:** The app can use multicast DNS (mDNS) to discover peers on the same local network. Discovery information may be visible to devices able to observe traffic on that network.
- **Bluetooth:** When supported and enabled, Bluetooth discovery and communication can be used with nearby peers. Bluetooth Low Energy discovery broadcasts a short-lived rendezvous token; this token is not the app's stable peer identity. Nearby devices may still observe radio-level discovery traffic and other Bluetooth metadata exposed by the platform.
- **STUN connectivity discovery:** When STUN is enabled, the app sends requests to configured STUN server(s) to discover a public network endpoint and/or help assess NAT behavior. The server receives the public IP address and source port used for the request and may observe other network metadata inherent in receiving it. The app's built-in defaults include Google-operated STUN endpoints; Cloudflare is also available as a server option. STUN is used for connectivity discovery, not to carry message or file content.

You may be able to disable STUN in the relevant receiving/network settings. When STUN is disabled, the app does not contact a STUN server for that discovery operation, but peers outside your local network may be harder or impossible to reach.

Network information such as IP addresses, ports, timestamps, and protocol metadata may be visible to the peers you contact, your network operator, and any third-party service contacted for connectivity discovery. The developer does not receive this information through a developer-operated messaging relay or analytics service.

## 4. Encryption and Security Limitations

Structured Mail uses encryption and peer-authentication mechanisms appropriate to the transport in use. IP-based connections use TCP/TLS, and Bluetooth communication uses the app's authenticated encrypted session mechanisms. Local databases and Warehouse objects are encrypted at rest as described above.

These protections reduce exposure but cannot guarantee security in every circumstance. Security can be affected by compromised or unlocked devices, malicious peers, operating-system vulnerabilities, network conditions, user exports, or the recipient's subsequent handling of received data. Direct connectivity may also fail because of NAT behavior, firewalls, device capabilities, or network restrictions. Structured Mail does not provide guaranteed delivery while a peer is offline or unreachable and does not use other peers to relay traffic as a mesh network.

### Android screen-capture protection

On Android, protection against screenshots and screen capture is enabled by default for the app window. You can change this setting in the app's Security tab. This is a mitigation, not a guarantee: it cannot prevent someone from photographing the screen with another device or protect against every operating-system or device compromise.

## 5. Third-Party Services and Payments

Structured Mail does not intentionally integrate advertising or usage-analytics functionality. However, some features use platform services or contact third-party services as described here:

- **STUN providers:** When STUN is enabled, configured providers receive the network information described in Section 3. Their processing is governed by their own policies and terms.
- **Google Play Billing (Android only):** The Android app uses Google Play Billing to offer optional one-time support purchases. Google processes these transactions under Google's applicable terms and privacy policy. The app receives purchase details and status needed to display the available support options and process a completed purchase. The developer does not operate a separate payment-processing server for these purchases.
- **Operating-system services:** File selection and import/export use platform-provided mechanisms, including Android's Storage Access Framework (SAF). Bluetooth and local-network functions also depend on operating-system APIs and permissions.

This list describes the known service integrations relevant to the app's functionality; it does not replace the privacy policies of Google, STUN providers, the operating system, or any other service you choose to use.

## 6. Android Permissions

The Android version requests permissions for the following purposes, as applicable to the Android version and features you use:

- **Internet (`INTERNET`):** Establish direct network connections and perform connectivity discovery.
- **Bluetooth scan, advertise, and connect:** Discover nearby peers and communicate over supported Bluetooth transports.
- **Network and Wi-Fi state/configuration:** Inspect network availability and support local-network communication and connectivity features, including supported hotspot handoffs.
- **Nearby Wi-Fi devices:** Support local-network and nearby Wi-Fi operations on Android versions that require this permission.
- **Legacy location permissions on Android 12L and earlier:** The manifest limits the legacy location permissions to API level 32 and below for compatibility with older Android behavior and nearby-device discovery. Structured Mail does not use these permissions to provide a location-history or location-tracking service.
- **Storage Access Framework (SAF):** Let you select particular files for import or export without requesting broad access to all files on the device.

Android controls when permissions are granted or denied. Some features will not work if the relevant permission is denied or the device does not support the required capability.

## 7. Data Retention and Deletion

Application data is generally retained locally until you delete it using available app controls or remove the relevant app data through the operating system. Exact deletion behavior depends on the platform and the type of data. The developer cannot remotely erase data stored only on your device.

Copies you have sent to peers, exported to another location, or otherwise copied outside the app's private storage are outside the developer's control. Deleting a local copy does not delete a recipient's copy. If you use a third-party service, its retention practices are governed by that service's policies.

## 8. Children's Privacy

Structured Mail is not designed or directed at children under 13. It does not require a developer-operated user account, and the developer does not operate an app backend intended to collect children's personal information. Network communication and third-party services may nevertheless process technical information as described in this policy. If you have a concern about information associated with a child, contact the developer using the details below.

## 9. Changes to This Privacy Policy

This Privacy Policy may be updated when the app's functionality, integrations, or applicable requirements change. The latest version will be published at this page in the public repository. The effective date above indicates when this version took effect. Please review this page periodically.

## 10. Contact Us

For questions about this Privacy Policy or Structured Mail's data-handling practices, contact the developer:

- **Developer:** Seacatechnology
- **Support email:** seacatechnology@gmail.com
