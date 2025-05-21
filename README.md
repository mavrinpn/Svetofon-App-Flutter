![Svetofon Smart Trainer](https://github.com/mavrinpn/Svetofon-App/raw/main/img/trainer.png)

# Svetofon — Smart Reaction Trainer

**Svetofon** is a modular mobile application built with Flutter for iOS and Android. It is designed to enhance cognitive and motor functions through interactive training using an external smart trainer panel (Bluetooth LE device).

> Previously implemented in Swift as a native iOS app, the new version adopts a cross-platform approach while preserving core functionality and enhancing flexibility and maintainability.

---

## 📱 App Overview

![Svetofon](https://github.com/mavrinpn/Svetofon-App/raw/main/img/Svetofon_AppStore_Screenshots_2.png)

- Fully custom UI design
- Optimized for tablets (iPad and Android Tablet)
- Adaptive layout across screen sizes
- Offline-first architecture with server sync

---

## 🛠️ Tech Stack

The Flutter app is split into two independent modules:

### **🧩 `svetofon_common`**

Reusable module with:
- Core logic and state management (BLoC, Provider, RxDart)
- Navigation (GoRouter)
- Dependency Injection (GetIt)
- PocketBase API client
- Shared models, services, and UI widgets
- SVG, image caching, HTML rendering

### **📲 `svetofon_flutter_app`**

Main application with:
- **Bluetooth LE** integration (`flutter_blue_plus`)
- **Local data storage**: `sqflite`, `shared_preferences`
- **Multimedia**: sound playback (`flutter_soloud`), text-to-speech (`flutter_tts`), vibration
- **File handling**: PDF/XLSX export, sharing/import
- **Camera support**: image picking and cropping
- **UI utilities**: expandable views, custom fonts

---

## 🧠 Architecture

- Modular monorepo structure
- Clean separation of business logic and presentation
- Feature-first file organization
- Offline-first interaction with remote sync fallback
- Custom exercise configuration with JSON-based protocol

---

## 🔐 Authentication Flow

- Persistent token-based offline authentication
- Server sync for backup/restore when available

---

## 📤 Export & Configuration

- User training data can be exported to `.xlsx` or `.pdf`
- Exercise sets can be created and edited via in-app configurator
- Supports export/import of training routines via JSON

---

## 🧩 Backend Stack (Legacy Swift Version)

The previous version of Svetofon was developed natively for iOS and connected to a custom backend:
- **Node.js (Express, Mongoose, Passport)**
- **MongoDB** for user data
- Deployed on VDS with **Nginx proxy**
- API included:
  - Authentication
  - Analytics
  - Backup management

---

## Supports iPad

![Svetofon](https://github.com/mavrinpn/Svetofon-App/raw/main/img/Svetofon_AppStore_Screenshots_3.png)

---

## 📺 Watch on Youtube

[![Svetofon Youtube](https://github.com/mavrinpn/Svetofon-App/raw/main/img/youtube.png)](https://www.youtube.com/watch?v=dg87534pwd8)

---

## 📦 App Store and Google Play

- App published at [App Store](https://apps.apple.com/ru/app/светофон/id1597336312)

![AppStore Link](https://github.com/mavrinpn/Svetofon-App/raw/main/img/AppStore.png)


---

## 📇 Contact

**Author**: [Pavel Mavrin](https://www.linkedin.com/in/pavel-mavrin-developer/)

---
