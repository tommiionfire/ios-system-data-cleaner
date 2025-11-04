# 🧹 iOS System Data Cleaner (Date Trick Automation)

> A simple, repeatable method to force iOS to permanently clear “System Data” (caches) using the **Date Trick** — without revalidation or cache reappearance.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-iOS-lightgrey.svg)](#)
[![Status](https://img.shields.io/badge/status-stable-green.svg)](#)

---

## 📖 Overview

If you’ve ever noticed **“System Data”** on iOS consuming tens of gigabytes, you’re not alone.  
Apple’s background process `maintenanced` is responsible for cache management — but often fails to permanently remove temporary files even after triggering the so-called *date trick*.

This guide details a **reliable, repeatable, and safe method** to fully trigger and complete the cache expunging process — making the reduction in “System Data” **immediate and permanent** (until caches rebuild naturally over time).

---

## ⚠️ Disclaimer

- **Use at your own risk.** This method interacts with system maintenance processes in iOS.
- **Do not perform frequently.** Caches improve performance. Only use when System Data exceeds **25 GB** or device storage is critically low.
- **Backup important data first.**
- **Set iMessage to “Forever” before beginning** — otherwise old messages may be deleted.

---

## 🧭 Step-by-Step Instructions

### 1️⃣ Preparation

1. Check current *System Data* usage:  
   **Settings → General → iPhone Storage → System Data**
2. Close all running apps.
3. Go to:  
   **Settings → Messages → Keep Messages → Forever**  
   ✅ *Critical: prevents message loss.*
4. Enable **Airplane Mode** and disable both **Wi-Fi** and **Bluetooth.**  
   *(Prevents iCloud sync or Apple Watch interference.)*

---

### 2️⃣ Trigger Maintenance Process

1. Open **Settings → General → Date & Time.**
2. Disable *Set Automatically.*
3. Manually set the date **1 year into the future**.
4. Wait **60 seconds** while keeping the phone awake.
5. Check *System Data* usage — it should drop significantly.  
   *(If not visible, relaunch Settings and check again.)*

---

### 3️⃣ Finalize & Lock the Change

1. Now, change the date to **3 months in the future** from the real date.  
   (This is roughly **9 months earlier** than the previous setting.)
2. Wait another **60 seconds.**
3. Check *System Data* again — it should remain the same or slightly lower.
4. Re-enable **Set Automatically.**
5. Turn **Airplane Mode** off.

---

## ✅ Done!

You’ve now successfully triggered and completed iOS’s internal cleanup process (`maintenanced`).  
Your *System Data* should be permanently reduced until iOS naturally rebuilds necessary caches.

---

## 🧩 Optional Cleanup Tips

- Delete and reinstall **Instagram** and **Discord** — these apps are known for hiding large caches within System Data.
- Reboot your device after completion for best results.

---

## 🧠 Why It Works

iOS’s `maintenanced` process is time-based. By jumping the date far into the future, you **force** a scheduled maintenance cycle.  
The *double date change* ensures the cleanup process completes before revalidation occurs — effectively locking in the freed storage.

---

## 📅 Changelog

| Version | Date       | Description                      |
|----------|------------|----------------------------------|
| 1.0.0    | 2025-11-04 | Initial documented method release |

---

## 🪪 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 💬 Feedback

Found a variation that works better?  
Open an issue or share your findings in the [Discussions](../../discussions) tab.

---

> “It’s absolutely ridiculous this process is even necessary — Apple should fix this once and for all.”  
> — *iOS community consensus since iOS 12.*
