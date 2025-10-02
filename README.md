# 🛠️ Fix: JK BMS Bluetooth "Make a Pair Failure!" Error  

## 📌 Issue  
Many JK BMS users (esp. 60A/100A all-in-one boards with **integrated Bluetooth**) hit this problem:  

- First connection works fine.  
- Later attempts on a new phone (or after reinstalling the app) always show:  




This happens because the BMS **binds to the first phone/app installation** and won’t accept new pairings until reset. Since these models have no detachable Bluetooth dongle, normal tricks (forget device, reinstall app, toggle BT) don’t work.  

---

## ✅ Solution: Reset via JK BMS *Company* App  

### ⚠️ Prerequisites
- Password must still be the **default** (`123456`).  
- Device name doesn’t matter.  
- Willingness to install a **shady Chinese “JK-BMS Company” app** (different from the Play Store JK BMS app).  

*(This app is clunky, half-translated, and not recommended for daily use — but it exposes the hidden “Factory Reset” option.)*  

---

### 🔧 Steps
1. **Install the JK BMS Company app** (APK can be found via JK docs / forums / vendors).  
2. **Open the app → connect to your BMS**.  
   - Ignore any weird UI or broken status screens.  
3. **Slide to the “Settings” tab/column**.  
4. Scroll down and tap **Factory Reset**.  
5. Confirm reset → BMS will reboot.  

---

## 🎉 Result
- Bluetooth binding is cleared.  
- You can now reconnect using the **regular JK-BMS app** (the proper one from Play Store).  
- “Make a pair failure!” is gone.  

---

## 🧾 Notes
- If you’ve ever changed the default password, you’ll need to set it back before reset works.  
- Factory reset doesn’t erase your cell calibration or pack settings — it just resets comms.  
- If you’d rather avoid the Company app, you can also do this via **RS485 + PC software**, but the APK is the fastest way.  

---

## 💡 TL;DR
JK BMS integrated BT locks to the first phone. To fix “Make a pair failure!”, install the **JK-BMS Company app**, connect, go to **Settings → Factory Reset**, and you’re good.  

---

## 📷 Example Error Screen  

![Make a pair failure](INSERT-IMAGE-LINK-HERE)
