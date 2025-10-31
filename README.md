✅ Yescrypt Miner iOS Repo

This repository contains Yescrypt miner packages for jailbroken iOS devices. It is designed to work with Cydia, Zebra, or Sileo.

📦 Repo Structure
yescrypt-repo/
 ├── debs/
 │    └── yescryptminer_1.0_iphoneos-arm.deb
 ├── Packages
 ├── Packages.gz
 └── Release


debs/ → contains the .deb package(s)

Packages → metadata for Cydia/Zebra

Packages.gz → compressed metadata

Release → repo information

⚙️ Installation

Add repo URL to Cydia/Zebra:

http://yourdomain.com/yescrypt-repo/


Refresh sources.

Install Yescrypt Miner from the package list.

🔧 Updating the Repo

Add or replace .deb files inside debs/.

Regenerate metadata:

dpkg-scanpackages debs /dev/null > Packages
gzip -c Packages > Packages.gz


Upload all files (debs/, Packages, Packages.gz, Release) to your web host.

⚠️ Notes

Only works on jailbroken iOS devices

Ensure .deb matches your device architecture: iphoneos-arm, arm64, or arm64e

Test on a secondary device before installing

📜 Credits

Maintainer: Your Name <email@example.com>

Repo created for Yescrypt CPU/GPU miner for iOS
