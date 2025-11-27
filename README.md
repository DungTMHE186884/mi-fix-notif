# mi-fix-notif

## 📌 Introduction
This script is designed to **fix delayed or missing notifications** on Xiaomi devices running MIUI/HyperOS.  
The main issue comes from **MIUI Optimization**, **PowerKeeper**, and Android’s **Doze Mode**, which aggressively restrict background activity and cause apps like messaging, email, or banking apps to miss push notifications.

The script will:
- Disable MIUI Optimization.
- Optionally disable Android Doze Mode.
- Add important apps to the **whitelist** so they are not killed in the background.
- Reset PowerKeeper to apply changes immediately.

---

## ⚙️ Requirements
- Xiaomi/MIUI/HyperOS device with **USB Debugging** enabled.
- A computer with **ADB** installed.
- USB connection between phone and computer.

---

## 🛠 How to Use
1. Clone or download the script to your computer.
2. Connect your Xiaomi device via USB.
3. Verify the connection:
   ```sh
   adb devices
If your device appears, continue.
4. Run the script:
   ```sh
   adb shell sh /path/to/fix-notification.sh
