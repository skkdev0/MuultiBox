# 📦 Multi Box Engine & .hpk Ecosystem

<p align="center">
  <img src="https://raw.githubusercontent.com/skkdev0/MuultiBox/refs/heads/main/app_icon.png" alt="Multi Box Icon" width="150" height="150">
</p>

<p align="center">
  <strong>A Revolutionary, Lightweight, and Zero-Footprint Dynamic Application Runner for Android & Beyond.</strong>
</p>

---

## 🚀 Overview

**Multi Box** is a next-generation application environment that breaks traditional Android constraints. It allows users to run modular, standalone applications packed inside a custom **`.hpk` (Hybrid Package)** format. 

With **Backward & Forward Compatibility (supporting Android 5.0 Lollipop up to Android 14+ / API 34+)**, Multi Box bypasses strict system limitations like Scoped Storage and Package Visibility Rules through runtime isolation and efficient application bridging.

---

## 🛠️ The 3 Layers of `.hpk` Support

Multi Box is engineered to handle three distinct types of applications within a single client, giving developers unmatched flexibility:

| App Type | Description | Core Engine |
| :--- | :--- | :--- |
| **🌐 URL Base** | Directly wraps any web application or portal into a native-feeling application experience. | Optimized WebView |
| **💻 HTML/Script Base** | Runs local HTML, CSS, JavaScript, or lightweight scripts locally with full GUI integration. | Local Sandbox Engine |
| **⚡ Dex Base** | Loads and executes compiled Android `.dex` (Dalvik/ART executable) files dynamically at runtime. | Advanced DexClassLoader |

---

## ✨ Key Features

* **True Native Feel:** Installing, running, or uninstalling an `.hpk` file gives the exact same premium user experience as standard Android `.apk` files.
* **Zero Footprint & High Security:** To ensure absolute privacy and storage efficiency, all unpacked execution files are **automatically wiped out** immediately upon application exit (`OnStroke` / `OnExit`).
* **Cross-Platform Vision:** Built with a clean architectural layout, meaning the same `.hpk` package (URL & HTML base) can effortlessly run on a **Windows Host application** in the future with zero code modification.
* **Full Modern Android Support:** Seamlessly handles **Android 11 to 14+ security restrictions**, including dynamic read-only memory alignment for dynamic class loading.

---

## 🏗️ Repository Structure

This repository acts as the central hub for the entire `.hpk` ecosystem:

* `/multi-box-engine/` -> The core Android runtime client application (releases available).
* `/hpk-builder/` -> The official compiler/toolchain used to bundle your websites, scripts, or dex files into `.hpk` packages.
* `/sample-hpk-apps/` -> A collection of lightweight, ready-to-run child `.hpk` applications for testing.

---

## 🛠️ How to Build `.hpk` Packages

We provide a specialized, lightweight compiler called **HPK Builder**. You can use it to package your projects:

1. Open **HPK Builder**.
2. Select your project source (Website URL, Local HTML/Script folder, or Compiled `.dex`).
3. Set your Application ID and Metadata.
4. Click **Compile** to generate your standalone `.hpk` file.
5. Transfer it to your device and open it via **Multi Box**!

---

## 🔒 Security & Data Isolation (Work in Progress)

We are actively refining individual data sandboxing for URL and HTML-based applications to separate cache, cookies, and LocalStorage directories per `.hpk` app, ensuring total isolation from the host APK.

---

## 🤝 Contributing & Support

This project is currently open-source! We welcome developers to test, create innovative `.hpk` child apps, and contribute to the engine.

* **Developer:** Sham Kumar Kshetri
* **Telegram Channel:** [Join Our Official Telegram](https://t.me/multiboxpro) for instant updates, alpha releases, and documentation.

---
<p align="center">🛡️ Built for performance. Optimized for privacy. Engineered for freedom. 🛡️</p>
