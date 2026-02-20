# SZ Project 🚀

<p align="center">
  <img src="https://via.placeholder.com/200x200.png?text=SZ+Project" alt="SZ Project Logo" width="200" height="200">
</p>

<p align="center">
  <strong>Optimasi Performa • Sensitivitas Layar • Hijack Game</strong>
</p>

<p align="center">
  <a href="https://github.com/SZProject/.github/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-GPLv3-blue.svg" alt="License: GPL v3">
  </a>
  <a href="https://github.com/SZProject">
    <img src="https://img.shields.io/badge/Platform-Android-brightgreen.svg" alt="Platform Android">
  </a>
  <a href="https://github.com/SZProject">
    <img src="https://img.shields.io/badge/API-21%2B-brightgreen.svg" alt="Minimum API Level">
  </a>
  <a href="https://github.com/SZProject">
    <img src="https://img.shields.io/badge/Shizuku-Required-orange.svg" alt="Shizuku Required">
  </a>
</p>

---

## 📋 Daftar Isi
- [Tentang Project](#tentang-project)
- [Fitur Utama](#fitur-utama)
- [Screenshot](#screenshot)
- [Persyaratan Sistem](#persyaratan-sistem)
- [Cara Install](#cara-install)
- [Cara Build dari Source](#cara-build-dari-source)
- [Struktur Project](#struktur-project)
- [Kontribusi](#kontribusi)
- [Lisensi](#lisensi)
- [Kontak](#kontak)
- [Disclaimer](#disclaimer)

---

## 🎯 Tentang Project

**SZ Project** adalah organisasi pengembangan yang fokus pada pembuatan aplikasi Android untuk meningkatkan pengalaman pengguna melalui optimalisasi performa sistem. Kami mengembangkan solusi inovatif untuk tweaking performa, peningkatan sensitivitas layar sentuh, dan tools untuk modifikasi game dengan memanfaatkan akses izin **Shizuku**.

Dengan SZ Project, Anda dapat:
- Mengoptimalkan performa perangkat Android Anda
- Meningkatkan responsivitas layar sentuh dan gesture
- Melakukan modifikasi pada game untuk pengalaman bermain yang lebih baik
- Semua tanpa memerlukan akses root!

---

## ✨ Fitur Utama

### ⚙️ Tweaking Performa
- **CPU Governor Tuner** - Atur governor CPU sesuai kebutuhan (performance, powersave, interactive)
- **Memory Optimizer** - Optimasi manajemen RAM untuk multitasking lebih lancar
- **Thermal Control** - Kontrol suhu device untuk mencegah throttling
- **I/O Scheduler** - Atur scheduler I/O untuk akses storage lebih cepat
- **Build.prop Tweaks** - Modifikasi build.prop untuk performa maksimal

### 🖐️ Sensitivitas Layar
- **Touch Response Tuner** - Atur sensitivitas sentuhan layar
- **Swipe Sensitivity** - Tingkatkan akurasi gesture swipe
- **Polling Rate Adjuster** - Sesuaikan polling rate layar sentuh
- **Palm Rejection** - Fitur anti-sentuhan telapak tangan saat gaming
- **Edge Prevention** - Hindari sentuhan tidak sengaja di tepi layar

### 🎮 Hijack Game
- **Game Booster** - Optimasi otomatis saat game dijalankan
- **FPS Unlocker** - Buka batasan FPS di game tertentu
- **Graphics Tweaker** - Modifikasi pengaturan grafis game
- **Input Mapper** - Mapping ulang kontrol game
- **Anti-Cheat Bypass Tools** - Untuk game single player (offline)

### 🔧 Teknologi
- Menggunakan **Shizuku API** untuk akses sistem tanpa root
- **Minimal RAM usage** - Hanya berjalan saat diperlukan
- **User-friendly UI** - Interface sederhana dan mudah dipahami
- **Backup & Restore** - Simpan dan pulihkan konfigurasi Anda

---

## 📸 Screenshot

<p align="center">
  <img src="screenshots/home.jpg" width="200" alt="Home Screen">
  <img src="screenshots/performance.jpg" width="200" alt="Performance Settings">
  <img src="screenshots/touch.jpg" width="200" alt="Touch Sensitivity">
  <img src="screenshots/game.jpg" width="200" alt="Game Hijack">
</p>

*Screenshot akan ditambahkan segera*

---

## 📱 Persyaratan Sistem

| Persyaratan | Minimum | Rekomendasi |
|------------|---------|-------------|
| **Android Version** | Android 5.0 (API 21) | Android 8.0+ (API 26+) |
| **RAM** | 1 GB | 3 GB+ |
| **Storage** | 50 MB free | 100 MB free |
| **Shizuku** | v12.0+ | v13.0+ |
| **Root** | Tidak wajib | Opsional (untuk fitur tambahan) |

**Catatan:** Beberapa fitur mungkin memerlukan Android versi lebih tinggi atau akses root.

---

## 📲 Cara Install

### Metode 1: Install dari Release (Termudah) ✅

1. **Download APK** dari halaman [Releases](https://github.com/SZProject/app/releases)
2. **Install Shizuku** (jika belum punya):
   - Download dari [Play Store](https://play.google.com/store/apps/details?id=moe.shizuku.privileged.api)
   - Atau dari [GitHub Shizuku](https://github.com/RikkaApps/Shizuku)
3. **Aktifkan Shizuku**:
   - Buka aplikasi Shizuku
   - Ikuti petunjuk aktivasi sesuai device Anda (ADB/Wireless debugging)
   - Pastikan status "Shizuku is running"
4. **Install APK SZ Project**:
   - Buka file APK yang sudah didownload
   - Izinkan instalasi dari sumber tidak dikenal jika diminta
   - Klik "Install"
5. **Buka aplikasi** dan berikan izin Shizuku saat diminta

### Metode 2: Install via ADB (Alternatif)

```bash
# Install APK via ADB
adb install app-release.apk

# Grant permissions manually (jika perlu)
adb shell pm grant com.szproject.app android.permission.WRITE_SECURE_SETTINGS
adb shell pm grant com.szproject.app android.permission.READ_LOGS
adb shell pm grant com.szproject.app android.permission.DUMP
```

---

## 🔨 Cara Build dari Source

### Prasyarat

| Tools | Version Minimal | Link Download |
|-------|-----------------|---------------|
| **Android Studio** | Arctic Fox (2020.3.1) | [Download](https://developer.android.com/studio) |
| **JDK** | 11 | [Download](https://adoptium.net/) |
| **Git** | 2.25 | [Download](https://git-scm.com/) |
| **Android SDK** | API 33 | (Include di Android Studio) |
| **Gradle** | 7.0.2 | (Include di project) |

### Langkah-langkah Build

#### 1. Clone Repository
```bash
# Clone dengan HTTPS
git clone https://github.com/SZProject/app.git

# Clone dengan SSH
git clone git@github.com:SZProject/app.git

# Masuk ke direktori
cd app
```

#### 2. Setup Local Properties
```bash
# Linux/Mac
echo "sdk.dir=$HOME/Android/Sdk" > local.properties

# Windows (Command Prompt)
echo sdk.dir=C:\\Users\\%USERNAME%\\AppData\\Local\\Android\\Sdk > local.properties
```

#### 3. Build Debug APK
```bash
# Linux/Mac
chmod +x gradlew
./gradlew clean assembleDebug

# Windows
gradlew.bat clean assembleDebug
```

#### 4. Build Release APK
```bash
# Generate keystore (jika belum punya)
keytool -genkey -v -keystore release.keystore -alias szproject -keyalg RSA -keysize 2048 -validity 10000

# Build release
./gradlew clean assembleRelease
```

#### 5. Lokasi Hasil Build
```
Debug APK: app/build/outputs/apk/debug/app-debug.apk
Release APK: app/build/outputs/apk/release/app-release.apk
```

### Build Variants
```bash
# Build semua variant
./gradlew assemble

# Install langsung ke device
./gradlew installDebug
./gradlew installRelease
```

### Troubleshooting Build

| Error | Solusi |
|-------|--------|
| `SDK location not found` | Buat file local.properties dengan path SDK yang benar |
| `Java home not set` | Install JDK 11 dan set `JAVA_HOME` |
| `Permission denied` | `chmod +x gradlew` di Linux/Mac |
| `Shizuku API not found` | `./gradlew clean` lalu build ulang |

---

## 📁 Struktur Project

```
SZProject/
├── app/                                      # Module aplikasi utama
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/szproject/
│   │   │   │   ├── ui/                       # UI Components
│   │   │   │   ├── core/                      # Core logic
│   │   │   │   ├── tweaks/                    # Performance tweaks
│   │   │   │   ├── touch/                      # Touch sensitivity
│   │   │   │   ├── game/                        # Game hijack
│   │   │   │   └── utils/                       # Utility classes
│   │   │   ├── res/                            # Resources
│   │   │   └── AndroidManifest.xml
│   │   ├── test/                                # Unit tests
│   │   └── androidTest/                         # Instrumentation tests
│   ├── build.gradle                             # App module gradle
│   └── proguard-rules.pro                        # ProGuard rules
├── libraries/                                    # Library modules
│   ├── shizuku-api/                              # Shizuku API wrapper
│   └── common-utils/                             # Shared utilities
├── gradle/wrapper/                                # Gradle wrapper
├── docs/                                          # Documentation
├── .github/                                       # GitHub config
├── .gitignore                                     # Git ignore rules
├── LICENSE                                        # GPL-3.0 License
├── README.md                                      # This file
├── build.gradle                                   # Project gradle
├── gradle.properties                              # Gradle properties
├── gradlew                                        # Gradle wrapper (Linux/Mac)
├── gradlew.bat                                    # Gradle wrapper (Windows)
└── settings.gradle                                # Project settings
```

---

## 🤝 Kontribusi

Kami sangat terbuka untuk kontribusi! Berikut caranya:

### Cara Berkontribusi
1. **Fork repository** ini
2. **Buat branch baru** untuk fitur Anda
   ```bash
   git checkout -b fitur-keren-anda
   ```
3. **Commit perubahan** Anda
   ```bash
   git commit -m "feat: menambahkan fitur baru"
   ```
4. **Push ke branch**
   ```bash
   git push origin fitur-keren-anda
   ```
5. **Buat Pull Request** ke branch `main`

### Pedoman Kontribusi
- ✅ Ikuti coding style yang ada
- ✅ Tambahkan komentar untuk kode kompleks
- ✅ Update dokumentasi jika diperlukan
- ✅ Test di minimal 2 device berbeda

---

## 📄 Lisensi

```
Copyright (C) 2024 SZ Project

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
```

Project ini dilisensikan di bawah **GNU General Public License v3.0**.

---

## 📬 Kontak

| Platform | Link |
|----------|------|
| **GitHub** | [@SZProject](https://github.com/SZProject) |
| **Telegram** | [t.me/szproject](https://t.me/szproject) |
| **Discord** | [SZ Project Community](https://discord.gg/szproject) |
| **Email** | [szproject@email.com](mailto:szproject@email.com) |

### Report Bug / Saran Fitur
- Buat [Issue baru](https://github.com/SZProject/app/issues)

---

## ⚠️ Disclaimer

**Peringatan Penting:**
1. **Penggunaan Aplikasi**
   - Aplikasi ini menggunakan akses Shizuku yang dapat mengubah pengaturan sistem
   - Gunakan dengan bijak dan pahami risiko yang ada
   - Kami tidak bertanggung jawab atas kerusakan yang disebabkan oleh penggunaan yang tidak tepat

2. **Fitur Hijack Game**
   - Hanya untuk game OFFLINE / SINGLE PLAYER
   - Jangan gunakan untuk game online/multiplayer
   - Penggunaan untuk game online dapat mengakibatkan banned account

3. **Kompatibilitas Device**
   - Tidak semua fitur bekerja di semua device
   - Performa dapat bervariasi tergantung device

4. **Data Privacy**
   - Aplikasi ini TIDAK mengumpulkan data pribadi
   - Semua konfigurasi disimpan lokal di device

---

<p align="center">
  Made with ❤️ by SZ Project Team
</p>

<p align="center">
  <a href="#sz-project-">Kembali ke Atas ↑</a>
</p>
