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
