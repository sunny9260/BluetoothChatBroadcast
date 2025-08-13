# 📡 Offline Bluetooth Chat with Admin Broadcast

An **offline communication app** for Android that uses **Bluetooth only** — no Wi-Fi, no mobile data, no internet.  
Supports **private 1-to-1 chats** and **admin broadcasts** to all nearby devices.

---

## 🚀 Features
- **📡 Auto-Broadcast** messages without pairing (BLE advertising).
- **🔒 Private Chat** with specific nearby users (Classic Bluetooth sockets).
- **👑 Admin Mode** — First device in the session becomes admin automatically.
- **📱 Fully Offline** — Works anywhere without internet.
- **📜 Real-time Chat UI** with message history.
- **⚡ Low-Power BLE** for efficient broadcasting.
- **🔍 Automatic Device Discovery**.

---

## 🎯 Use Cases
- Disaster zones with no network coverage.
- Group announcements at events, schools, or workplaces.
- Offline chat for trekking, camping, or remote locations.
- Military or tactical communication without network dependency.

---

## 🛠 Tech Stack
- **Language:** Java / Kotlin
- **Framework:** Native Android (API 26+)
- **Bluetooth APIs:** Classic Bluetooth + Bluetooth Low Energy (BLE)
- **Tools:** Android Studio, GitHub Codespaces, Codemagic CI/CD for cloud builds.

---

## ⚙ How It Works
1. **Start App** → Devices begin BLE scanning to detect nearby devices.
2. **Admin Selection** → First device to start becomes admin automatically.
3. **Messaging Options**:
   - **Broadcast Message** → Admin sends to all devices via BLE advertising.
   - **Private Message** → Send directly to one user via Classic Bluetooth sockets.
4. **Chat Interface** → All messages are displayed in real-time.

---

## 📋 Permissions
Add these to `AndroidManifest.xml`:
```xml
<uses-permission android:name="android.permission.BLUETOOTH" />
<uses-permission android:name="android.permission.BLUETOOTH_ADMIN" />
<uses-permission android:name="android.permission.BLUETOOTH_SCAN" />
<uses-permission android:name="android.permission.BLUETOOTH_ADVERTISE" />
<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
