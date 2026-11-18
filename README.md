# 🥔 kentangOS 1.0

**kentangOS** adalah distribusi Linux mandiri (*independent distribution*) yang dibangun dari fondasi **Linux From Scratch (LFS)** dengan fokus pada stabilitas, efisiensi sumber daya, dan keamanan sistem. Sistem operasi ini dirancang agar tetap ringan dijalankan pada perangkat keras berspesifikasi rendah (*low-end*), sekaligus memberikan kontrol penuh atas arsitektur sistem di baliknya.

---

## ✨ Fitur Utama

* **Arsitektur Mandiri (LFS-Based):** Dirakit langsung dari bawah tanpa *bloatware* bawaan distro komersial.
* **Custom Vanilla Kernel:** Menggunakan kode sumber murni dari [kernel.org](https://kernel.org) versi **6.18.63-kentangos** yang dikonfigurasi dan dikompilasi secara khusus untuk efisiensi *driver* dan kecepatan *booting*.
* **Keamanan Bawaan (AppArmor Enabled):** Mendukung *Mandatory Access Control* (MAC) melalui AppArmor yang terintegrasi langsung pada tingkat kernel.
* **Antarmuka Ringan:** Menggunakan lingkungan desktop **XFCE4** yang responsif dan hemat penggunaan memori.
* **Manajemen Paket Terintegrasi:** Mengadopsi ekosistem manajemen paket `apt` / `dpkg` untuk kemudahan instalasi perangkat lunak.

---

## 💻 Spesifikasi Minimum Sistem (Versi 1.0)

Untuk menjalankan **kentangOS 1.0** beserta lingkungan desktop XFCE4 secara lancar, pastikan perangkat memenuhi spesifikasi berikut:

| Komponen | Spesifikasi Minimum |
| :--- | :--- |
| **Arsitektur Prosesor** | x86_64 (64-bit) |
| **Memori (RAM)** | **Minimal 3 GB** (direkomendasikan untuk kelancaran multitasking) |
| **Penyimpanan** | Minimal 15 GB ruang kosong (untuk instalasi sistem) |
| **Firmware / Boot** | UEFI atau Legacy BIOS (GRUB2) |

---

## 🛠️ Informasi Teknis Sistem

* **Nama Distribusi:** kentangOS 1.0 (Codename: `Kentang`)
* **Versi Kernel:** `6.18.63-kentangos` (Vanilla LTS)
* **Init System:** `systemd`
* **Desktop Environment:** XFCE4
* **Lisensi:** GNU General Public License v3.0 (GPL-3.0)

---

## 📂 Struktur Repositori

* `kernel/` — Berisi file konfigurasi kernel (`.config`) dan skrip bantu kompilasi untuk membangun ulang kernel `6.18.63-kentangos`.
* `docs/` — Catatan teknis pengembangan, panduan konfigurasi sistem, dan dokumentasi *hardening* keamanan.
* `LICENSE` — Dokumen lisensi resmi GPL-3.0.

---

## 🚀 Roadmap Pengembangan

- [x] Membangun fondasi sistem berbasis Linux From Scratch (LFS)
- [x] Kompilasi *vanilla kernel* mandiri (`6.18.63-kentangos`) dengan dukungan AppArmor
- [x] Konfigurasi identitas sistem mandiri (`/etc/os-release` & GRUB)
- [ ] Unggah file konfigurasi `.config` kernel ke repositori
- [ ] Pembuatan *Live ISO Installer* (`squashfs` + GRUB) untuk distribusi publik
- [ ] Penerapan profil *security hardening* tingkat lanjut secara bawaan

---

## 🤝 Kontribusi & Pelaporan Bug

Proyek ini dikembangkan secara terbuka. Jika menemukan *bug*, kendala kompatibilitas perangkat keras, atau ingin memberikan saran pengembangan, silakan buka tiket baru melalui halaman [**Issues**](https://github.com).

---
os ini di kembangkan murni untuk iseng namun gw berfikir ingin seriusin mulai sekarang btw mungkin bug tak dapat ku perbaiki
dengan cepat karna aku masih bersekolah di bangku smp jadi yaa mohon di maklumi tapi tiap minggu gw pasti bacain jika ada bug report

*Dikembangkan secara independen sejak Januari 2026 oleh Rajo kentangOS...*
