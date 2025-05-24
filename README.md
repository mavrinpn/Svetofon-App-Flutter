![Svetofon Smart Trainer](https://github.com/mavrinpn/Svetofon-App-Flutter/raw/main/img/Svetoton_cover.jpeg)

# Svetofon — Smart Reaction Trainer

## 🛠️ Tech Stack

- 🧩 Mobile Frontend: Flutter/Dart
- 🧩 Backend: PocketBase
- 🧩 Admin and Statistics Dashboard: Flutter Web

## 📦 Supported Platforms and Store Links

- ✅ iOS (iPhone + iPad): [App Store](https://apps.apple.com/en/app/svetofon/id6737197083)
- ✅ Android: [Google Play]()
- ✅ Huawei (with no Google Services): [APK]

**Svetofon** is a modular mobile application built with Flutter for iOS and Android. It is designed to enhance cognitive and motor functions through interactive training using an external smart trainer panel (Bluetooth LE device).

> Previously implemented in [Swift as a native iOS app](https://github.com/mavrinpn/Svetofon-App-Swift), the new version adopts a cross-platform approach while preserving core functionality and enhancing flexibility and maintainability.

---

## 📱 App Overview

![Svetofon](https://github.com/mavrinpn/Svetofon-App-Flutter/raw/main/img/Svetofon3_iPhone.png)

**Svetofon** is a mobile app designed to assess and improve **reaction speed**, **coordination**, and **cognitive skills** using a Bluetooth-connected smart trainer panel.

The app combines physical and mental exercises to stimulate both the **central** and **peripheral nervous systems**. It’s suitable for use in rehabilitation, sports performance, and mental training programs.

The main screen features a categorized catalog of exercises with clear text instructions and flexible difficulty levels.

---

### 🔐 Key Capabilities

- Measures **reaction times** with near real-time latency (under 10ms)
- Exports training results to **XLSX** and **PDF** formats
- Supports export/import of **File Cabinet cards** and **Favorite exercises** using a proprietary JSON-based format
- Fully functional in **offline mode** with **auto-sync** when Internet connection is available
- Exercise and module catalog with **group-based access control**
- Full **multilingual support**, including UI localization and **voice guidance** during exercises
- **Multichannel Audio and vibration feedback** for interactive training sessions
- Backup and **restore of the local user database**, including rollback capabilities
- Custom exercise configuration with JSON-based protocol

---

## 🧠 Architecture and Libs

The Flutter app is split into two independent modules:

### **🧩 `svetofon_common`**

Reusable module with:
- Core logic and state management (BLoC, Provider, RxDart)
- Navigation (GoRouter)
- Dependency Injection (GetIt)
- PocketBase API client
- Shared models, services, and UI widgets
- SVG, image caching, HTML rendering
- and other

### **📲 `svetofon_flutter_app`**

Main application with:
- **Bluetooth LE** integration (`flutter_blue_plus`)
- **Local data storage**: `sqflite`, `shared_preferences`
- **Multimedia**: sound playback (`flutter_soloud`), text-to-speech (`flutter_tts`), vibration
- **File handling**: PDF/XLSX export (`pdf`, `excel`), sharing/import (`share_plus`, `open_file`, `receive_sharing_intent`)
- **UI utilities**: expandable views, custom fonts and layout params

---

## 🧩 Features

- Fully custom UI design
- Optimized for tablets (iPad and Android Tablet)
- Adaptive layout across screen sizes
- Offline-first architecture with server sync
- Modular monorepo structure
- Clean separation of business logic and presentation
- Feature-first file organization
- **Remote configuration** of app settings, themes, icons, and UI elements from the server
- Custom server-based **Translation Management System** with pluralization support
- **Intelligent version control**: ensures exercises are only available if supported by the current app version

![Svetofon iPad](https://github.com/mavrinpn/Svetofon-App-Flutter/raw/main/img/Svetofon3_iPad.png)

---

## 📤 Export Data

- User training data can be exported to `.xlsx` or `.pdf`
- Result files contains custom tables, charts, graphs and descriptions

![Svetofon PDF Protocol](https://github.com/mavrinpn/Svetofon-App-Flutter/raw/main/img/protocol.png)

---

## 📺 Watch on Youtube

[![Svetofon Youtube](https://github.com/mavrinpn/Svetofon-App-Flutter/raw/main/img/youtube.png)](https://www.youtube.com/watch?v=dg87534pwd8)

---

## 📇 Contact

**Author**: Pavel Mavrin  
[LinkedIn](https://www.linkedin.com/in/mavrinpn/)
[Telegram](https://t.me/mavrinpn)

---
