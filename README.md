# 🌟 Yescrypt Miner iOS Repo

Welcome to the **Yescrypt Miner repository** for jailbroken iOS devices!  
Compatible with **Cydia** and **Zebra**.

---

## 🚀 Quick Add

[![Add Yescrypt Miner Repo](https://img.shields.io/badge/Add-Yescrypt_Miner_Repo-blue?style=for-the-badge)](cydia://url/https://github.com/nahrvic/Yescrypt-Miner-iOS-Repo)  
[![Add Yescrypt Miner Repo](https://img.shields.io/badge/Add-Yescrypt_Miner_Repo-purple?style=for-the-badge)](zbra://url/https://github.com/nahrvic/Yescrypt-Miner-iOS-Repo)

---

## 📁 Repo Structure

```
Yescrypt-Miner-iOS-Repo/
 ├── debs/
 │    └── yescryptminer_1.0_iphoneos-arm.deb
 ├── Packages
 ├── Packages.gz
 ├── Release
 └── README.md
```

- `debs/` → contains `.deb` packages  
- `Packages` → metadata for Cydia/Zebra  
- `Packages.gz` → compressed metadata  
- `Release` → repo info  
- `README.md` → this file

---

## ⚙️ Installation Instructions

1. Open **Cydia** or **Zebra** on your jailbroken iPhone  
2. Go to **Sources → Edit → Add**  
3. Paste your repo URL:

```
https://github.com/nahrvic/Yescrypt-Miner-iOS-Repo
```

4. Refresh sources  
5. Install **Yescrypt Miner** from the list

---

## 🔧 Updating the Repo

1. Add or replace `.deb` files inside `debs/`  
2. Regenerate metadata:

```bash
cd yescrypt-repo
dpkg-scanpackages debs /dev/null > Packages
gzip -c Packages > Packages.gz
```

3. Commit and push **all files** to GitHub

---

## ⚠️ Notes

- Only works on **jailbroken iOS devices**  
- `.deb` must match device architecture: `iphoneos-arm`, `arm64`, or `arm64e`  
- Test on a secondary device before installing

---

## 📜 Credits

- Maintainer: **Your Name** `<email@example.com>`  
- Repository created for **Yescrypt CPU/GPU miner for iOS**