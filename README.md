<p align="center">
  <img src="readme-res/kp-readme-header.png" width="80%" alt="KnoxPatch Header" />
</p>

# KnoxPatch (One UI 9 Support Fork)

An [Xposed / LSPosed / Vector](https://github.com/JingMatrix/LSPosed) module to get Samsung Knox-dependent apps and features working again on rooted Samsung Galaxy devices with a tripped Knox warranty bit (`0x1`).

> [!NOTE]
> **One UI 9 Compatibility**: This fork adds active support for **One UI 9.x (Android 17, SEP 180000)** on devices like the Galaxy S23 Ultra and newer, removing the artificial version ceiling present in the upstream release.

---

## 📱 Supported Android & One UI Versions
- Android 9 (One UI 1.x)
- Android 10 (One UI 2.x)
- Android 11 (One UI 3.x)
- Android 12 (One UI 4.x)
- Android 12L (One UI 4.1.1)
- Android 13 (One UI 5.x)
- Android 14 (One UI 6.x)
- Android 15 (One UI 7.x)
- Android 16 (One UI 8.x)
- **Android 17 (One UI 9.x)** *(Supported in this fork)*

---

## ✅ Supported Apps
- ✅ [Auto Blocker](https://www.samsung.com/uk/support/mobile-devices/protect-your-galaxy-device-with-the-new-auto-blocker-feature/)
- ➖ [Galaxy Wearable (Gear Manager)](https://www.samsung.com/us/support/owners/app/galaxy-wearable-watch) ([Enhancer](#knoxpatch-enhancer) required)
- ✅ Samsung Cloud ([FMM](https://www.samsung.com/uk/support/mobile-devices/what-is-find-my-mobile-and-how-can-i-use-it-to-locate-lock-or-wipe-my-device/), [Enhanced data protection](https://www.samsung.com/ae/support/mobile-devices/what-is-the-enhanced-data-protection-function-and-when-can-i-use-it/))
- ✅ [Samsung Flow](https://www.samsung.com/uk/apps/samsung-flow/)
- ✅ [Samsung Health](https://www.samsung.com/uk/apps/samsung-health/)
- ✅ [Samsung Health Monitor](https://www.samsung.com/uk/apps/samsung-health-monitor/)
- ➖ [Samsung TV Plus](https://www.samsungtvplus.com/) ([TrickyStore](https://github.com/5ec1cff/TrickyStore/releases/latest) required)
- ✅ [Secure Folder](https://www.samsungknox.com/en/solutions/personal-apps/secure-folder) ([Enhancer](#knoxpatch-enhancer) might be required)
- ✅ [Secure Wi-Fi](https://www.samsung.com/uk/support/mobile-devices/what-is-the-secure-wifi-feature-and-how-do-i-enable-or-use-it/)
- ✅ [SmartThings](https://www.samsung.com/uk/smartthings/app/)
- ➖ [Smart View](https://www.samsung.com/uk/tvs/tv-buying-guide/what-is-samsung-smart-view/) ([Enhancer](#knoxpatch-enhancer) required)
- ✅ [Private Share](https://www.samsung.com/uk/support/mobile-devices/how-to-keep-your-personal-data-safe-using-private-share/)*
- ❌ [Samsung Pass](https://www.samsung.com/uk/apps/samsung-pass/)
- ❌ [Samsung Wallet (Pay)](https://www.samsung.com/uk/apps/samsung-wallet/)

\* Devices running One UI 5.1 or lower might need [PIF](https://github.com/chiteroman/PlayIntegrityFix/releases/latest) or similar for this feature to work correctly since the integration in Quick Share. 

---

## ⚡ Installation Guide

1. **Install KnoxPatch APK:**  
   Download `KnoxPatch-v0.8.4-OneUI9.apk` from the [Releases](https://github.com/larcencial/KnoxPatch/releases) section and install it.
2. **Enable in LSPosed / Vector:**  
   Open LSPosed (or Vector), go to the **Modules** tab, enable **KnoxPatch**, and ensure **System Framework** and target Samsung apps are checked.
3. **Install KnoxPatch Enhancer (Recommended):**  
   Flash `KnoxPatch-Enhancer-v0.4.zip` in **KernelSU / Magisk** to fix Galaxy Wearable, Smart View, and additional WSM security layers.
4. **Reboot:**  
   Restart your device and enjoy Knox-dependent apps.

---

## 🔧 KnoxPatch Enhancer

KnoxPatch Enhancer is a flashable zip that will take care of the (currently) non-fixable apps/features via the Xposed APIs.

- **Via the [Magisk](https://github.com/topjohnwu/Magisk) / [KernelSU](https://github.com/tiann/KernelSU) app (Fix Galaxy Wearable apps / Smart View):**  
  Download the module zip from [Releases](https://github.com/larcencial/KnoxPatch/releases) and install it from the "Modules" tab. The app will then show an "Enhanced" badge once active:

<p align="center">
  <img loading="lazy" src="readme-res/kp-enhancer.png" width="35%" alt="KnoxPatch Enhancer Badge" />
</p>

---

## 📜 Credits
- [salvogiangri](https://github.com/salvogiangri) (Original KnoxPatch creator)
- [larcencial](https://github.com/larcencial) (One UI 9 maintenance & compatibility)
- Samsung
- [JingMatrix](https://github.com/JingMatrix)
- [YukiHookAPI](https://github.com/fankes/YukiHookAPI)
- [Rikka](https://github.com/RikkaApps)

## 📄 License
GNU General Public License v3.0 - see [LICENSE](LICENSE) for details.
