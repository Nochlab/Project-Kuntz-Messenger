# 📡 Kuntz Messenger

> **Decentralized, serverless offline messaging for Bochrim.** Forked from the open-source Knit framework.

<img width="2000" height="2000" alt="Kuntz icon NEW" src="https://github.com/user-attachments/assets/d929e632-d27a-4011-afd0-9a68ea451c4e" />

---

### 📖 Overview

**Kuntz** is a serverless, peer-to-peer messaging application engineered specifically to give bochrim a smooth, direct way to stay in touch completely off-the-grid. 

Because it routes communications directly device-to-device, you can text without cellular service, active data plans, or recurring bills. Chat on the fly using local Bluetooth mesh networks or hop onto nearby Wi-Fi configurations to exchange messages across larger campus areas without needing a traditional mobile carrier.

---

### 🔥 Key Advantages for Bochrim

Kuntz is built from the ground up for a reliable, completely independent texting experience without contract restrictions or web filters:

* **No SIM or Cell Service Needed**  
  Breathe new life into offline hardware. Kuntz runs flawlessly on old smartphones with the SIM cards pulled out, iPods, or any baseline Android device.
* **Dual-Mode Local Connectivity**  
  Seamlessly adapt to your environment. The app switches automatically to **Bluetooth Mesh** when you are walking down the street and hooks onto standard **Local Wi-Fi** loops indoors.
* **Zero Internet Traps**  
  Because text packets never touch the open web, there are no algorithmic feeds, tracking pixels, built-in browsers, or online distractions to worry about. It simply routes messages.
* **Complete Infrastructure Privacy**  
  No cellular phone numbers, registered emails, or centralized account databases track your connections. You remain fully off-grid.

---

### 📡 How It Works: Mesh Networking Explained

Traditional chat clients fail the moment a cell tower drops or an internet gateway closes. Kuntz keeps conversations active by forming dynamic pathways over existing on-board device radios.

#### 1. Bluetooth Low Energy (BLE) Mesh
When completely separated from local routers or hardware infrastructure, Kuntz leverages BLE radios to construct an independent neighborhood mesh.
* **The "Hop" Network:** If you text a friend blocks away, your message securely bounces through the devices of other close-range Kuntz users until it lands safely on his screen.
* **Total Intermediary Privacy:** Middle-relay users never have access to your data. Private DMs and group chats are entirely end-to-end encrypted, passing transparently through background system processes.

#### 2. Wi-Fi Local & Multi-Hop Channels
The framework expands past pure Bluetooth limits by utilizing local Wi-Fi frequencies for extended reach.
* **Local Wi-Fi Direct:** Connect directly peer-to-peer inside the same building without configuring or authenticating through an external internet router.
* **Standard Campus Wi-Fi:** When an active Wi-Fi access point is present, Kuntz utilizes it as an expansive transmission bridge to blast your messages across massive structural distances or entire campus complexes instantly.

---

### 🔒 Security & Interception Realities

Because Kuntz transmits data over a public broadcasting medium (radio waves), it is physically possible for anyone with a standard packet sniffer within range to capture your traffic. However, the protocol architecture protects your content based on the chat type:

* **Private Rooms & DMs (End-to-End Encrypted):** Uses Google Tink HPKE (wrapped in X25519) and AES-256-GCM. An outside interceptor or background relay node will only see encrypted gibberish. The text, images, and delivery receipts are protected.
* **Public "Nearby" Room (Plaintext):** Designed as an open digital megaphone. Messages sent in this room are **unencrypted** so any device can join the conversation. **Do not share sensitive information in the Nearby room, as anyone sniffing the network can read it.**
* **Metadata & Identity Protection:** While text payloads remain locked in private chats, a sophisticated interceptor can track *when* messages are sent and *how large* they are. Always scan your friends' physical QR codes to complete key verification and block Man-in-the-Middle tracking.

---

### 📊 Client Feature Comparison

| Capabilities & Requirements | 📡 Kuntz Messenger | 💬 Standard Chat Applications |
| :--- | :---: | :---: |
| **Requires Active SIM Card** | ❌ No |  Yes |
| **Requires Monthly Service Plan** | ❌ No |  Yes |
| **Operates over Offline Wi-Fi Direct** |  Yes | ❌ No |
| **Routes via Multi-Device Bluetooth Mesh** |  Yes | ❌ No |

---

### 🛠️ Quick Setup Guide

1. **Sideload the Application**  
   Grab the latest `.apk` package file directly from a friend via SD Card, local USB storage, or peer-to-peer sharing.
2. **Activate Hardware Radios**  
   Ensure both your system **Bluetooth** and **Wi-Fi** settings are toggled on.
3. **Exchange Identity Keys**  
   Pair securely with your friends by scanning their local public ID key directly on-screen, and you are ready to message.
