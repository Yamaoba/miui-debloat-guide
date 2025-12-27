# 📱 MIUI 14 (Android 12) Debloat Guide

> **Goal:** Safely remove unnecessary MIUI / Google / third‑party bloatware to improve performance, privacy, and battery life.

---

## ⚠️ Disclaimer

* This guide is based on **community experience** (XDA, Reddit, Gists).
* **Do everything at your own risk.**
* Always **backup important data** before debloating.
* Prefer **disable first**, uninstall only if you are confident.

---

## 📌 Device Information

* **Device:** Poco X3 NFC
* **ROM:** MIUI 14
* **Android:** 12

---

## 📚 References / Sources

* XDA Developers – Poco X3 NFC Bloatware Guide
  [https://xdaforums.com/t/guide-uninstall-poco-x3-nfc-bloatware-list.4169497/](https://xdaforums.com/t/guide-uninstall-poco-x3-nfc-bloatware-list.4169497/)
* mcxiaoke MIUI package list
  [https://gist.github.com/mcxiaoke/ade05718f590bcd574b807c4706a00b1](https://gist.github.com/mcxiaoke/ade05718f590bcd574b807c4706a00b1)
* Reddit – Safe to uninstall system apps
  [https://www.reddit.com/r/PocoPhones/comments/jc5rlr/list_of_safe_to_uninstall_system_apps/](https://www.reddit.com/r/PocoPhones/comments/jc5rlr/list_of_safe_to_uninstall_system_apps/)
* Reddit – msa & miui daemon discussion
  [https://www.reddit.com/r/miui/comments/1fa50gi/am_i_need_those_msa_and_miui_daemon_or_should_i/](https://www.reddit.com/r/miui/comments/1fa50gi/am_i_need_those_msa_and_miui_daemon_or_should_i/)

---

## 🧹 1. Apps I Uninstalled (Safe for Daily Use)

> These apps were removed without breaking core system functionality.

### MIUI / Xiaomi Apps

* `com.mi.android.globalminusscreen` — App Vault
* `com.mi.android.globalFileexplorer` — Mi File Manager
* `com.mi.globalbrowser` — Mi Browser
* `com.miui.analytics` — MIUI Analytics *(spyware / telemetry)*
* `com.miui.bugreport` — Bug Report
* `com.miui.hybrid` — Quick Apps *(data mining)*
* `com.miui.hybrid.accessory` — Quick Apps Accessory
* `com.miui.miservice` — Services & Feedback
* `com.miui.yellowpage` — Yellow Pages
* `com.xiaomi.glgm` — GetApps Games
* `com.xiaomi.scanner` — Mi Scanner
* `com.xiaomi.mircs` — MIUI to MIUI Messaging
* `com.xiaomi.mipicks` — GetApps (Xiaomi App Store)
* `com.xiaomi.mi_connect_service` — Xiaomi IoT / Mi Home bridge
* `com.miuix.editor` — Frequent Phrase Service
* `com.miui.videoplayer` — Mi Video
* `com.miui.weather2` — Mi Weather
* `com.miui.calculator` — Mi Calculator
* `com.miui.screenrecorder` — Mi Screen Recorder

### Google Apps

* `com.google.android.feedback` — App / Play Store Feedback
* `com.google.android.apps.subscriptions.red` — Google One
* `com.google.android.projection.gearhead` — Android Auto
* `com.google.android.apps.googleassistant` — Google Assistant
* `com.google.ar.core` — Google Play AR Services

### Third‑Party / Others

* `com.facebook.appmanager` — Facebook
* `com.facebook.services` — Facebook
* `com.facebook.system` — Facebook
* `com.tencent.soter.soterserver` — Chinese payment service *(removed without issues)*
* `org.ifaa.aidl.manager` — Alipay related service

---

## ❓ 2. Apps With Risks / Uncertain Behavior

> These apps may affect system stability, DRM, or battery life.

### ⚠️ **DO NOT UNINSTALL (Recommended)**

* `com.miui.wmsvc`

  * ⚠️ May break **Widevine L1**, cause bootloops or service crashes.

### ⚠️ **Be Careful**

* `com.xiaomi.xmsf` — Xiaomi Service Framework
  ❌ Removing causes errors like:

  * "Battery & performance has stopped"
  * "Xiaomi location has stopped"

* `com.xiaomi.xmsfkeeper` — XMSF log keeper

  * Cannot be disabled
  * Best left installed

* `com.miui.daemon` — MIUI Data Collector

  * Some users report **battery drain when removed**
  * I personally **uninstalled** it

* `com.xiaomi.barrage` — Game pop‑up / bullet notifications (Maybe China ROM feature)

  * Removed, no issues observed

* `com.xiaomi.joyose` — Power / GPU management

  * Conflicting reports:

    * Ads / analytics tracker
    * GPU tuner
    * Removing may delay **calls & SMS**
  * 🔁 **Reinstalled for safety**

---

## 📴 3. Disabled (May Be Useful Later)

* `com.miui.touchassistant` — Quick Ball feature

> Disabled instead of uninstalling so it can be restored easily.

---

## 📝 4. Important Notes

### Mi File Manager

* Package: `com.mi.android.globalFileexplorer`
* Required for **"Choose Package"** option in Xiaomi Package Updater
* Play Store link:
  [https://play.google.com/store/apps/details?id=com.mi.android.globalFileexplorer](https://play.google.com/store/apps/details?id=com.mi.android.globalFileexplorer)

👉 If you don’t use Xiaomi Package Updater, it’s better to use a **third‑party file manager**.

---

## 🔁 5. Recommended Replacement Apps (Optional)

> All replacements below are **user choice** — install only what you need.

### 🌐 Browser

* Removed: `com.android.browser`
* Replacement: **Brave Browser**, **Cromite**

### 🧮 Calculator

* Removed: `com.miui.calculator`
* Replacement: **ClevCalc**

### 📅 Calendar

* Removed: `com.android.calendar`
* Replacement: **Google Calendar**

### 🧭 Compass

* Removed: `com.miui.compass`
* Replacement: **Digital Compass**
  *(or use a real compass 😄)*

### 📤 File Sharing

* Removed: `com.xiaomi.midrop`
* Replacement: **Send Anywhere**

### 🧹 Cleaner

* Removed: `com.miui.cleanmaster`
* Replacement: **SD Maid**

### 📁 File Manager

* Removed: `com.mi.android.globalFileexplorer`
* Replacement: **Solid Explorer**

### 🎬 Video Player

* Removed: `com.miui.videoplayer`
* Replacement: **VLC**, **MX Player**

### 🖼️ Wallpaper

* Removed: `com.miui.miwallpaper`
* Replacement: **Walli**

### 🎵 Music

* Removed: `com.miui.player`
* Replacement: **Spotify**, **YouTube Music**

### 📝 Notes

* Removed: `com.miui.notes`
* Replacement: **Simplenote**

### 🎙️ Recorder

* Removed: `com.android.soundrecorder`
* Replacement: **Smart Recorder**

### 📷 Scanner

* Removed: `com.xiaomi.scanner`
* Replacement: **Binary Eye**

### 🎥 Screen Recorder

* Removed: `com.miui.screenrecorder`
* Replacement: **AZ Screen Recorder**

### ☁️ Weather

* Removed: `com.miui.weather2`
* Replacement: **Today Weather**

### 📞 Caller ID

* Removed: `com.miui.yellowpage`
* Replacement: **Truecaller**
* Only Optional to Install

---

## ✅ Final Notes

* Always debloat **step‑by‑step**, reboot after major changes.
* If something breaks → **reinstall the package immediately**.
* For maximum safety, prefer **disable > uninstall**.

Happy debloating 🚀
