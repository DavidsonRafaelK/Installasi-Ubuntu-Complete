##  Daftar Isi

[**Home**](#home) 

##  Mengenal Ubuntu

* [**Apa itu Ubuntu?**](#apa-itu-ubuntu)
* [**Mengapa Memilih Ubuntu?**](#mengapa-memilih-ubuntu)
* [**Mengapa Repo Ini?**](#mengapa-repo-ini)

##  Persiapan Instalasi

* [**Persyaratan dan Alat**](#persyaratan-dan-alat)
    * [**Perangkat Keras yang Kompatibel**](#perangkat-keras-yang-kompatibel)
    * [**Cadangkan Data Anda**](#cadangkan-data-anda)
    * [**Unduh Ubuntu ISO**](#unduh-ubuntu-iso)
    * [**Buat USB Bootable**](#buat-usb-bootable)
        * [**Buat USB Bootable dengan Etcher**](#buat-usb-bootable-dengan-etcher)
            * [**Unduh Etcher**](#unduh-etcher)
            * [**Instal Etcher**](#instal-etcher)
            * [**Siapkan USB Drive**](#siapkan-usb-drive)
            * [**Buat USB Bootable dengan Etcher**](#buat-usb-bootable-dengan-etcher)
            * [**Boot dari USB Drive**](#boot-dari-usb-drive)
            * [**Ringkasan Langkah**](#ringkasan-langkah)
    * [**Akses BIOS/UEFI**](#akses-biosuefi)
    * [**Koneksi Internet**](#koneksi-internet)
    * [**Rencanakan Partisi (jika Dual Booting)**](#rencanakan-partisi-jika-dual-booting)
    * [**Langkah-langkah Persiapan USB Ubuntu**](#langkah-langkah-persiapan-usb-ubuntu)
    * [**Daftar Periksa**](#daftar-periksa)
* [**Memecahkan Masalah Kesalahan Umum**](#memecahkan-masalah-kesalahan-umum)
    * [**Masalah Boot Order**](#masalah-boot-order)
    * [**Instalasi Macet atau Gagal Dimulai**](#instalasi-macet-atau-gagal-dimulai)
    * [**Kesalahan Partisi**](#kesalahan-partisi)
        * [**Gunakan GParted**](#gunakan-gparted)
    * [**Masalah Konektivitas Jaringan**](#masalah-konektivitas-jaringan)
    * [**Instalasi GRUB Gagal**](#instalasi-grub-gagal)
        * [**Langkah-langkah Troubleshooting GRUB**](#langkah-langkah-troubleshooting-grub)
    * [**Ringkasan Kesalahan Umum dan Solusi**](#ringkasan-kesalahan-umum-dan-solusi)

##  Instalasi Ubuntu

* [**Instal Ubuntu Desktop dan Atur Partisi Manual**](#instal-ubuntu-desktop-dan-atur-partisi-manual)
    * [**Boot dari USB Drive**](#boot-dari-usb-drive)
    * [**Mulai Instalasi Ubuntu**](#mulai-instalasi-ubuntu)
    * [**Siapkan Disk (Partisi Manual)**](#siapkan-disk-partisi-manual)
        * [**Buat Partisi Root (/)**](#buat-partisi-root)
        * [**Buat Partisi Swap**](#buat-partisi-swap)
        * [**Buat Partisi Home (/home)**](#buat-partisi-home-home)
    * [**Selesaikan Instalasi**](#selesaikan-instalasi)
    * [**Proses Instalasi**](#proses-instalasi)
    * [**Selesaikan**](#selesaikan)
    * [**Ringkasan Partisi Manual**](#ringkasan-partisi-manual)
    * [**Penjelasan Singkat Partisi**](#penjelasan-singkat-partisi)
* [**Pengaturan Awal dan Konfigurasi**](#pengaturan-awal-dan-konfigurasi)
    * [**Instal Perangkat Lunak Esensial**](#instal-perangkat-lunak-esensial)
    * [**Konfigurasi Desktop Environment**](#konfigurasi-desktop-environment)
        * [**Personalisasi Tampilan**](#personalisasi-tampilan)
        * [**Atur Dock**](#atur-dock)
    * [**Hubungkan ke Internet**](#hubungkan-ke-internet)
        * [**Wi-Fi**](#wi-fi)
        * [**Ethernet**](#ethernet)
    * [**Atur Printer Anda**](#atur-printer-anda)
    * [**Buat Pengguna Tambahan**](#buat-pengguna-tambahan)
    * [**Atur Backup dan Recovery**](#atur-backup-dan-recovery)
* [**Dual Booting dengan Windows**](#dual-booting-dengan-windows)
    * [**Buat Partisi Terpisah untuk Ubuntu**](#buat-partisi-terpisah-untuk-ubuntu)
        * [**Gunakan Windows Disk Management**](#gunakan-windows-disk-management)
    * [**Instal Ubuntu**](#instal-ubuntu)
        * [**Ikuti Panduan Instalasi**](#ikuti-panduan-instalasi)
    * [**Pilihan Boot**](#pilihan-boot)
        * [**Konfigurasi GRUB**](#konfigurasi-grub)
* [**Instalasi Ubuntu Server**](#instalasi-ubuntu-server)
    * [**Unduh Ubuntu Server ISO**](#unduh-ubuntu-server-iso)
        * [**Kunjungi Situs Web Ubuntu**](#kunjungi-situs-web-ubuntu)
    * [**Buat USB Bootable**](#buat-usb-bootable)
        * [**Gunakan Etcher atau Alat Lain**](#gunakan-etcher-atau-alat-lain)
    * [**Boot dari USB Drive**](#boot-dari-usb-drive)
        * [**Ikuti Langkah-langkah Booting**](#ikuti-langkah-langkah-booting)
    * [**Konfigurasi Pengaturan Server**](#konfigurasi-pengaturan-server)
        * [**Ikuti Panduan Instalasi**](#ikuti-panduan-instalasi)
        * [**Contoh Konfigurasi Server**](#contoh-konfigurasi-server)
            * [**Server Web dengan Apache**](#server-web-dengan-apache)
            * [**Server Database dengan MySQL**](#server-database-dengan-mysql)
            * [**Server Email dengan Postfix**](#server-email-dengan-postfix)
* [**Instalasi pada Platform Lain**](#instalasi-pada-platform-lain)
    * [**Instalasi pada Mesin Virtual**](#instalasi-pada-mesin-virtual)
        * [**Instalasi dengan VirtualBox**](#instalasi-dengan-virtualbox)
            * [**Unduh dan Instal VirtualBox**](#unduh-dan-instal-virtualbox)
            * [**Buat Mesin Virtual Baru**](#buat-mesin-virtual-baru)
            * [**Pilih Gambar Ubuntu**](#pilih-gambar-ubuntu)
            * [**Mulai Mesin Virtual**](#mulai-mesin-virtual)
            * [**Konfigurasi Tambahan (opsional)**](#konfigurasi-tambahan-opsional)
        * [**Instalasi dengan VMware Workstation**](#instalasi-dengan-vmware-workstation)
            * [**Unduh dan Instal VMware Workstation**](#unduh-dan-instal-vmware-workstation)
            * [**Buat Mesin Virtual Baru**](#buat-mesin-virtual-baru)
            * [**Pilih Gambar Ubuntu**](#pilih-gambar-ubuntu)
            * [**Mulai Mesin Virtual**](#mulai-mesin-virtual)
            * [**Ikuti Panduan Instalasi**](#ikuti-panduan-instalasi)
            * [**Tips untuk Instalasi dengan VMware Workstation**](#tips-untuk-instalasi-dengan-vmware-workstation)
            * [**Setelah Instalasi**](#setelah-instalasi)
            * [**Kesimpulan**](#kesimpulan)
    * [**Instalasi pada Raspberry Pi**](#instalasi-pada-raspberry-pi)
        * [**Unduh Gambar Raspberry Pi OS**](#unduh-gambar-raspberry-pi-os)
        * [**Buat Image SD Card**](#buat-image-sd-card)
        * [**Boot Raspberry Pi**](#boot-raspberry-pi)

##  Penggunaan Ubuntu

* [**Terminal dan Command Line**](#terminal-dan-command-line)
    * [**Perintah Dasar Terminal**](#perintah-dasar-terminal)
* [**Software Manager**](#software-manager)
    * [**Menggunakan GNOME Software**](#menggunakan-gnome-software)
* [**Apt-get Package Manager**](#apt-get-package-manager)
    * [**Dasar-dasar Apt-get**](#dasar-dasar-apt-get)
* [**Integrasi Git**](#integrasi-git)
    * [**Kloning Repositori**](#kloning-repositori)
        * [**Gunakan Git Clone**](#gunakan-git-clone)
    * [**Membuat Perubahan dan Kontribusi**](#membuat-perubahan-dan-kontribusi)
        * [**Buat Cabang Baru**](#buat-cabang-baru)
        * [**Commit Perubahan**](#commit-perubahan)
    * [**Melacak Perubahan dan Pembaruan**](#melacak-perubahan-dan-pembaruan)
        * [**Pull Perubahan Terbaru**](#pull-perubahan-terbaru)
        * [**Push Perubahan**](#push-perubahan)
* [**Upgrade Ubuntu**](#upgrade-ubuntu)
    * [**Langkah-langkah Upgrade**](#langkah-langkah-upgrade)
        * [**Perbarui Daftar Paket**](#perbarui-daftar-paket)
        * [**Tingkatkan Semua Paket**](#tingkatkan-semua-paket)
        * [**Mulai Ulang Sistem**](#mulai-ulang-sistem)
    * [**Solusi untuk Masalah Upgrade**](#solusi-untuk-masalah-upgrade)
        * [**Bersihkan Cache Paket**](#bersihkan-cache-paket)
        * [**Gunakan Mode Recovery**](#gunakan-mode-recovery)
            * [**Langkah-langkah Memasuki Mode Recovery**](#langkah-langkah-memasuki-mode-recovery)

##  Sumber Daya dan Dukungan

* [**Komunitas Ubuntu**](#komunitas-ubuntu)
* [**Mendapatkan Bantuan dan Dukungan**](#mendapatkan-bantuan-dan-dukungan)

---

## Apa itu Ubuntu?

**Ubuntu** adalah distribusi Linux yang populer dan ramah pengguna yang dikenal karena stabilitasnya, kemudahan penggunaannya, dan dukungan komunitas yang kuat.

## Mengapa Memilih Ubuntu?

### Ramah Pengguna

Ubuntu dirancang dengan kesederhanaan sebagai prioritas. Antarmuka pengguna grafisnya (GUI) intuitif dan mudah dinavigasi, menjadikannya pilihan yang sangat baik bagi mereka yang baru mengenal Linux.

### Stabilitas dan Keamanan

Ubuntu dikenal karena stabilitas dan keamanannya. Pembaruan rutin dan fokus pada keamanan memastikan bahwa sistem Anda tetap aman dan andal.

### Dukungan Komunitas

Ubuntu memiliki komunitas yang besar dan aktif. Ini berarti Anda dapat dengan mudah menemukan bantuan, tutorial, dan forum untuk membantu Anda dengan masalah atau pertanyaan apa pun yang mungkin Anda miliki.

### Ketersediaan Perangkat Lunak

Ubuntu menawarkan repositori besar perangkat lunak gratis dan sumber terbuka. Selain itu, ia mendukung aplikasi populer dan alat pengembangan, menjadikannya cocok untuk berbagai kebutuhan, mulai dari penggunaan kasual hingga pengembangan profesional.

### Kustomisasi

Ubuntu sangat dapat dikustomisasi. Anda dapat menyesuaikan sistem agar sesuai dengan preferensi Anda, mulai dari lingkungan desktop hingga perangkat lunak yang Anda gunakan.

## Mengapa Repo Ini?

Saya membuat repositori ini untuk memberikan panduan yang jelas dan langkah demi langkah untuk menginstal Ubuntu. Sebagai seseorang yang telah mengalami tantangan beralih dari sistem operasi lain ke Linux, saya memahami pentingnya tutorial yang mudah dipahami dan detail. Panduan ini bertujuan untuk membantu Anda dengan percaya diri menginstal dan mulai menggunakan Ubuntu, terlepas dari latar belakang teknis Anda.

---

## Persyaratan dan Alat

### Perangkat Keras yang Kompatibel

- **Prosesor**: Prosesor dual-core 2 GHz atau lebih baik.
- **Memori (RAM)**: Setidaknya 4 GB (8 GB direkomendasikan untuk kinerja yang lebih baik).
- **Penyimpanan**: Minimal 25 GB ruang hard drive kosong.
- **Kartu Grafis**: VGA yang mampu menampilkan resolusi layar 1024x768.
- **Port USB**: Untuk membuat USB bootable.

### Cadangkan Data Anda

Sebelum melanjutkan dengan instalasi, pastikan Anda mencadangkan semua data penting. Menginstal sistem operasi baru berpotensi menyebabkan kehilangan data jika tidak dilakukan dengan benar.

### Unduh Ubuntu ISO

- Kunjungi [situs web resmi Ubuntu](https://ubuntu.com/download) dan unduh file ISO Ubuntu terbaru.

### Buat USB Bootable

Untuk menginstal Ubuntu, Anda perlu membuat USB bootable. Anda dapat menggunakan alat seperti:
- **Rufus** (untuk Windows)
- **Etcher** (tersedia untuk Windows, macOS, dan Linux)
- **UNetbootin** (tersedia untuk Windows, macOS, dan Linux)

#### Buat USB Bootable dengan Etcher

##### Unduh Etcher

1. Kunjungi [situs web Etcher](https://www.balena.io/etcher/).
2. Unduh versi yang sesuai untuk sistem operasi Anda (Windows, macOS, atau Linux).

##### Instal Etcher

1. **Windows**:
   - Jalankan file `.exe` yang diunduh dan ikuti petunjuk instalasi.
2. **macOS**:
   - Buka file `.dmg` yang diunduh dan seret Etcher ke folder Aplikasi.
3. **Linux**:
   - Ekstrak file `.zip` yang diunduh dan jalankan file Etcher AppImage.

##### Siapkan USB Drive

1. Masukkan USB drive (setidaknya 4 GB) ke komputer Anda. Pastikan tidak ada data penting di dalamnya, karena akan diformat selama proses ini.

##### Buat USB Bootable dengan Etcher

1. Buka Etcher.

2. **Pilih Gambar**:
   - Klik tombol "Flash from file".
   - Telusuri dan pilih file ISO Ubuntu yang diunduh.

3. **Pilih Target**:
   - Klik tombol "Select target".
   - Pilih USB drive Anda dari daftar drive yang tersedia.

4. **Flash**:
   - Klik tombol "Flash!".
   - Etcher akan mulai membuat USB bootable. Proses ini mungkin memakan waktu beberapa menit.

5. **Validasi**:
   - Setelah flashing, Etcher akan memvalidasi USB drive untuk memastikan prosesnya berhasil.

##### Boot dari USB Drive

1. Nyalakan kembali komputer Anda.
2. Akses pengaturan BIOS/UEFI dengan menekan tombol yang sesuai selama startup (biasanya `F2`, `F12`, `Esc`, atau `Del`).
3. Ubah urutan boot untuk memprioritaskan boot dari USB drive.
4. Simpan perubahan dan keluar dari pengaturan BIOS/UEFI.
5. Komputer Anda sekarang seharusnya boot dari USB drive, dan Anda akan melihat layar instalasi Ubuntu.

##### Ringkasan Langkah

1. Unduh dan instal Etcher.
2. Siapkan USB drive.
3. Unduh Ubuntu ISO.
4. Gunakan Etcher untuk membuat USB bootable.
5. Boot dari USB drive untuk memulai proses instalasi Ubuntu.

### Akses BIOS/UEFI

- Anda perlu mengakses pengaturan BIOS atau UEFI komputer Anda untuk mengubah urutan boot, sehingga sistem Anda dapat boot dari USB drive.

### Koneksi Internet

- Koneksi internet aktif direkomendasikan selama instalasi untuk mengunduh pembaruan dan perangkat lunak tambahan.

### Rencanakan Partisi (jika Dual Booting)

- Jika Anda berencana untuk melakukan dual booting Ubuntu bersama sistem operasi lain (seperti Windows), rencanakan partisi Anda dengan tepat. Pastikan Anda memiliki cukup ruang kosong di hard drive Anda.

### Langkah-langkah Persiapan USB Ubuntu

1. **Unduh dan Instal Rufus (Windows) atau Etcher (Windows, macOS, Linux)**:
   - Untuk Rufus: Unduh dari [situs web Rufus](https://rufus.ie/).
   - Untuk Etcher: Unduh dari [situs web Etcher](https://www.balena.io/etcher/).

2. **Buat USB Bootable**:
   - Buka Rufus atau Etcher.
   - Pilih file ISO Ubuntu yang Anda unduh.
   - Pilih USB drive yang ingin Anda buat bootable.
   - Mulai proses dan tunggu hingga selesai.

### Daftar Periksa

- [ ] Perangkat keras yang kompatibel sudah siap.
- [ ] Data telah dicadangkan.
- [ ] Ubuntu ISO telah diunduh.
- [ ] USB bootable telah dibuat.
- [ ] Koneksi internet tersedia.
- [ ] Pengaturan BIOS/UEFI dapat diakses.
- [ ] Rencana partisi sudah siap (jika dual booting).

---

## Memecahkan Masalah Kesalahan Umum

### Masalah Boot Order

#### **Gejala:**
- Komputer tidak boot dari USB drive dan malah boot ke sistem operasi yang ada.

#### **Penyebab Kemungkinan:**
- Urutan boot di BIOS/UEFI tidak diatur untuk memprioritaskan USB drive.
- USB drive tidak dikenali sebagai perangkat bootable.

#### **Solusi:**
1. **Periksa Urutan Boot**:
   - Nyalakan kembali komputer dan masuk ke pengaturan BIOS/UEFI dengan menekan tombol yang sesuai (`F2`, `F12`, `Esc`, `Del`, dll.).
   - Pastikan USB drive diatur sebagai opsi boot pertama.
   - Simpan perubahan dan keluar.

2. **Periksa USB Drive**:
   - Verifikasi bahwa USB drive terhubung dengan benar.
   - Coba port USB yang berbeda.

3. **Buat Ulang USB Bootable**:
   - Jika USB drive masih tidak dikenali, buat ulang USB bootable menggunakan Etcher, pastikan prosesnya selesai tanpa kesalahan.

### Instalasi Macet atau Gagal Dimulai

#### **Gejala:**
- Proses instalasi macet atau gagal dimulai setelah memilih "Install Ubuntu".

#### **Penyebab Kemungkinan:**
- Perangkat keras yang tidak kompatibel.
- File ISO yang rusak atau pembuatan USB bootable yang tidak lengkap.
- Sumber daya sistem yang tidak mencukupi.

#### **Solusi:**
1. **Periksa Persyaratan Sistem**:
   - Pastikan komputer Anda memenuhi persyaratan sistem minimum untuk Ubuntu.

2. **Verifikasi Integritas ISO**:
   - Bandingkan checksum file ISO yang diunduh dengan yang disediakan di halaman unduhan Ubuntu untuk memastikan tidak rusak.

3. **Coba Opsi Boot yang Berbeda**:
   - Di layar boot awal, tekan `Esc` atau `Shift` untuk mengakses menu GRUB.
   - Coba boot dengan opsi yang berbeda, seperti mode "Safe Graphics".

### Kesalahan Partisi

#### **Gejala:**
- Kesalahan atau peringatan terkait partisi disk selama proses instalasi.

#### **Penyebab Kemungkinan:**
- Partisi yang ada tidak dikenali atau konflik dengan partisi yang ada.
- Ruang yang tidak cukup di disk target.

#### **Solusi:**
1. **Partisi Manual**:
   - Pilih "Something else" selama proses instalasi untuk mengelola partisi secara manual.
   - Pastikan ada cukup ruang kosong untuk partisi baru.
   - Buat partisi untuk root (`/`), swap, dan secara opsional `/home`.

2. **Periksa Kesehatan Disk**:
   - Gunakan alat seperti `GParted` untuk memeriksa kesehatan disk dan memperbaiki masalah apa pun sebelum melanjutkan dengan instalasi.

#### **Gunakan GParted**

- **Instal GParted:**
    ```bash
    sudo apt install gparted
    ```

- **Jalankan GParted:**
    - Cari "GParted" di menu aplikasi.
    - Gunakan GParted untuk membuat, menghapus, mengubah ukuran, dan memformat partisi.

### Masalah Konektivitas Jaringan

#### **Gejala:**
- Tidak dapat terhubung ke internet selama proses instalasi.

#### **Penyebab Kemungkinan:**
- Driver untuk kartu jaringan hilang.
- Konfigurasi jaringan yang tidak benar.

#### **Solusi:**
1. **Gunakan Koneksi Kabel**:
   - Jika memungkinkan, gunakan koneksi Ethernet kabel selama instalasi.

2. **Instal Driver Pihak Ketiga**:
   - Selama instalasi, pilih opsi untuk menginstal perangkat lunak dan driver pihak ketiga.

3. **Konfigurasi Manual**:
   - Jika menggunakan Wi-Fi, masukkan detail jaringan secara manual (SSID, kata sandi).

### Instalasi GRUB Gagal

#### **Gejala:**
- Pesan kesalahan yang menyatakan "Grub installation failed" selama proses instalasi.

#### **Penyebab Kemungkinan:**
- Perangkat instalasi yang dipilih untuk GRUB tidak benar.
- Konflik dengan boot loader yang ada.

#### **Solusi:**
1. **Instalasi GRUB Manual**:
   - Boot ke sesi live dan buka terminal.
   - Mount partisi root dari sistem yang terinstal:
     ```bash
     sudo mount /dev/sdX1 /mnt
     sudo mount /dev/sdX2 /mnt/boot/efi
     ```
   - Ganti `/dev/sdX1` dan `/dev/sdX2` dengan pengidentifikasi partisi yang sesuai.
   - Instal GRUB secara manual:
     ```bash
     sudo grub-install --boot-directory=/mnt/boot /dev/sdX
     sudo update-grub
     ```

2. **Periksa Mode Boot**:
   - Pastikan BIOS/UEFI diatur ke mode yang benar (UEFI atau Legacy) yang sesuai dengan mode instalasi Ubuntu.

#### **Langkah-langkah Troubleshooting GRUB**

1. **Periksa Log Instalasi:** Lihat log instalasi untuk petunjuk lebih lanjut tentang kesalahan yang terjadi.
2. **Gunakan Perintah `boot-repair`:** Jalankan perintah `boot-repair` dari sesi live untuk memperbaiki masalah boot yang umum.
3. **Buat Ulang USB Bootable:** Buat ulang USB bootable dan coba instalasi lagi.
4. **Pastikan Partisi Boot Terpasang dengan Benar:** Pastikan partisi boot (biasanya `/boot` atau `/boot/efi`) terpasang dengan benar selama proses instalasi GRUB.
5. **Nonaktifkan Secure Boot:** Nonaktifkan Secure Boot di pengaturan BIOS/UEFI jika diaktifkan.
6. **Reset BIOS/UEFI ke Pengaturan Default:** Reset pengaturan BIOS/UEFI ke pengaturan default dan coba instalasi lagi.

### Ringkasan Kesalahan Umum dan Solusi

1. **Masalah Boot Order**:
   - Sesuaikan pengaturan BIOS/UEFI, verifikasi koneksi USB, buat ulang USB bootable jika perlu.

2. **Instalasi Macet atau Gagal Dimulai**:
   - Verifikasi persyaratan sistem, periksa integritas ISO, coba opsi boot yang berbeda.

3. **Kesalahan Partisi**:
   - Gunakan partisi manual, periksa kesehatan disk dengan `GParted`.

4. **Masalah Konektivitas Jaringan**:
   - Gunakan koneksi kabel, instal driver pihak ketiga, konfigurasi jaringan secara manual.

5. **Instalasi GRUB Gagal**:
   - Instal GRUB secara manual, pastikan mode boot yang benar di BIOS/UEFI, dan ikuti langkah-langkah troubleshooting GRUB.

---

## Instal Ubuntu Desktop dan Atur Partisi Manual

### Boot dari USB Drive

1. **Masukkan USB Bootable**:
   - Masukkan USB bootable yang Anda buat sebelumnya ke komputer Anda.

2. **Akses Pengaturan BIOS/UEFI**:
   - Nyalakan kembali komputer Anda dan masuk ke pengaturan BIOS/UEFI dengan menekan tombol yang sesuai (`F2`, `F12`, `Esc`, `Del`, dll.) selama startup.

3. **Ubah Urutan Boot**:
   - Atur USB drive sebagai opsi boot pertama.
   - Simpan perubahan dan keluar dari pengaturan BIOS/UEFI.

4. **Boot dari USB**:
   - Komputer Anda sekarang seharusnya boot dari USB drive, dan Anda akan melihat layar selamat datang Ubuntu.

### Mulai Instalasi Ubuntu

1. **Pilih Bahasa**:
   - Pilih bahasa yang Anda inginkan dan klik "Install Ubuntu".

2. **Tata Letak Keyboard**:
   - Pilih tata letak keyboard Anda dan klik "Continue".

3. **Pembaruan dan Perangkat Lunak Lainnya**:
   - Pilih apakah Anda ingin menginstal perangkat lunak pihak ketiga untuk perangkat keras grafis dan Wi-Fi, Flash, MP3, dan media lainnya. Disarankan untuk mencentang opsi ini untuk kompatibilitas yang lebih baik.
   - Klik "Continue".

### Siapkan Disk (Partisi Manual)

1. **Jenis Instalasi**:
   - Pilih "Something else" untuk mengatur partisi secara manual dan klik "Continue".

2. **Partisi Manual**:
   - Anda akan melihat daftar partisi Anda saat ini. Jika Anda memiliki OS yang ada, Anda mungkin perlu menghapus atau mengubah ukuran partisi untuk membuat ruang untuk Ubuntu. Pastikan Anda telah mencadangkan data Anda sebelum melakukan perubahan.

3. **Membuat Partisi**:
   - **Ruang Kosong**:
     - Pilih ruang kosong atau partisi yang ingin Anda gunakan untuk instalasi Ubuntu dan klik tombol "+" untuk membuat partisi baru.

#### **Membuat Partisi Root (/)**
- **Titik Gunung**: `/`
- **Ukuran**: Setidaknya 25 GB (direkomendasikan: 50 GB atau lebih, tergantung kebutuhan Anda).
- **Jenis untuk partisi baru**: Primer.
- **Lokasi untuk partisi baru**: Awal ruang ini.
- **Gunakan sebagai**: Sistem file pencatatan Ext4.
- Klik "OK".

#### **Membuat Partisi Swap**
- **Titik Gunung**: Area swap.
- **Ukuran**: Umumnya, harus sama dengan atau dua kali ukuran RAM Anda (misalnya, 8 GB RAM -> 8-16 GB swap).
- **Jenis untuk partisi baru**: Primer.
- **Lokasi untuk partisi baru**: Awal ruang ini.
- **Gunakan sebagai**: Area swap.
- Klik "OK".

#### **Membuat Partisi Home (/home)**
- **Titik Gunung**: `/home`
- **Ukuran**: Alokasikan ruang yang tersisa untuk `/home` untuk menyimpan file pengguna.
- **Jenis untuk partisi baru**: Primer.
- **Lokasi untuk partisi baru**: Awal ruang ini.
- **Gunakan sebagai**: Sistem file pencatatan Ext4.
- Klik "OK".

### Selesaikan Instalasi

1. **Perangkat untuk Instalasi Bootloader**:
   - Pastikan perangkat yang benar dipilih (biasanya disk yang sama di mana Anda membuat partisi root).

2. **Tinjau dan Instal**:
   - Tinjau pengaturan partisi Anda untuk memastikan semuanya benar.
   - Klik "Install Now" dan konfirmasi perubahan.

3. **Zona Waktu**:
   - Pilih zona waktu Anda dan klik "Continue".

4. **Pengaturan Pengguna**:
   - Masukkan nama Anda, nama komputer, nama pengguna, dan kata sandi.
   - Pilih apakah Anda ingin masuk secara otomatis atau memerlukan kata sandi untuk masuk.
   - Klik "Continue".

### Proses Instalasi

- Proses instalasi sekarang akan dimulai. Ini mungkin memakan waktu, jadi bersabarlah.

### Selesaikan

1. **Nyalakan Kembali Komputer Anda**:
   - Setelah instalasi selesai, Anda akan diminta untuk menyalakan kembali komputer Anda. Lepaskan USB drive saat diminta.

2. **Boot Pertama**:
   - Komputer Anda sekarang seharusnya boot ke Ubuntu. Masuk dengan nama pengguna dan kata sandi yang Anda buat selama pengaturan.

### Ringkasan Partisi Manual

- **Partisi Root (`/`)**:
  - Ukuran: Setidaknya 25 GB (direkomendasikan: 50 GB atau lebih).
  - Sistem File: Ext4.
  - Titik Gunung: `/`.

- **Partisi Swap**:
  - Ukuran: Sama dengan atau dua kali ukuran RAM Anda.
  - Sistem File: Area swap.

- **Partisi Home (`/home`)**:
  - Ukuran: Ruang yang tersisa.
  - Sistem File: Ext4.
  - Titik Gunung: `/home`.

### Penjelasan Singkat Partisi

- **Partisi Root (`/`)**:
  - Ini adalah tempat file sistem operasi dan aplikasi disimpan.

- **Partisi Swap**:
  - Digunakan sebagai memori virtual ketika RAM penuh. Ini membantu meningkatkan kinerja dan stabilitas sistem.

- **Partisi Home (`/home`)**:
  - Ini adalah tempat file pribadi Anda, pengaturan, dan data khusus pengguna disimpan. Memiliki partisi `/home` yang terpisah membuatnya lebih mudah untuk menginstal ulang OS tanpa kehilangan data pribadi.

---

## Pengaturan Awal dan Konfigurasi

Setelah menginstal Ubuntu, Anda perlu melakukan beberapa tugas pengaturan awal dan konfigurasi:

### Instal Perangkat Lunak Esensial

- **Software Center**: Manajer perangkat lunak default Ubuntu, memberikan akses ke berbagai aplikasi. Gunakan ini untuk menginstal:
    - Browser web (Firefox, Chrome)
    - Paket office (LibreOffice, WPS Office)
    - Pemutar multimedia (VLC, MPV)
    - Editor teks (Gedit, Nano)
    - Emulator terminal (GNOME Terminal, Konsole)
- **Command Line**: Anda dapat menginstal perangkat lunak menggunakan command line:
    ```bash
    sudo apt update
    sudo apt install firefox libreoffice vlc gedit
    ```

### Konfigurasi Desktop Environment

- **GNOME**: Lingkungan desktop default untuk Ubuntu. Anda dapat menyesuaikan tampilan, menambahkan ekstensi, dan mengelola pengaturan.
- **Lingkungan Desktop Lainnya**: Pertimbangkan untuk menjelajahi alternatif seperti KDE, XFCE, atau MATE, tergantung pada preferensi Anda dan sumber daya sistem.

#### **Personalisasi Tampilan**

- Buka "Settings" (Pengaturan) > "Appearance" (Tampilan).
- Pilih tema, latar belakang, dan gaya ikon sesuai keinginan Anda.

#### **Atur Dock**

- Di pengaturan "Dock", sesuaikan ukuran, posisi, dan perilaku Dock.

### Hubungkan ke Internet

- **Wi-Fi**:
  - Klik ikon jaringan di panel atas.
  - Pilih jaringan Wi-Fi Anda dan masukkan kata sandi jika diperlukan.

- **Ethernet**:
  - Sambungkan kabel Ethernet ke komputer Anda. Koneksi akan otomatis terdeteksi.

### Atur Printer Anda

- **Pengaturan Printer**:
  - Buka "Settings" (Pengaturan) > "Printers" (Printer).
  - Klik "Add Printer" (Tambah Printer) dan ikuti petunjuk untuk menambahkan printer Anda.

### Buat Pengguna Tambahan

- **Tambah Pengguna**:
  - Buka "Settings" (Pengaturan) > "Users" (Pengguna).
  - Klik "Add User" (Tambah Pengguna) dan masukkan informasi pengguna baru.

### Atur Backup dan Recovery

- **Pengaturan Backup**:
  - Buka "Settings" (Pengaturan) > "Backup" (Cadangan).
  - Pilih lokasi penyimpanan dan jadwal untuk backup otomatis.
  - Gunakan alat seperti `Deja Dup` untuk memudahkan proses backup.

---

## Sumber Daya dan Dukungan

### Komunitas Ubuntu

- **Forum Ubuntu**:
  - [Ubuntu Forums](https://ubuntuforums.org/): Forum resmi komunitas Ubuntu.
  - [Ask Ubuntu](https://askubuntu.com/): Situs tanya jawab untuk pengguna Ubuntu.

### Mendapatkan Bantuan dan Dukungan

- **Dokumentasi Resmi**:
  - [Ubuntu Documentation](https://help.ubuntu.com/): Dokumentasi resmi Ubuntu.
  
- **Bantuan Online**:
  - Bergabung dengan komunitas Ubuntu di platform sosial seperti Reddit, Discord, dan Telegram.

### Terminal dan Command Line

- **Dasar-dasar Terminal**:
  - Buka terminal dengan menekan `Ctrl+Alt+T`.
  - Gunakan perintah dasar seperti `ls`, `cd`, `cp`, `mv`, `rm` untuk navigasi dan manipulasi file.

#### **Perintah Dasar Terminal**

- **`ls`**: Menampilkan daftar file dan direktori.
- **`cd`**: Mengubah direktori.
- **`mkdir`**: Membuat direktori baru.
- **`cp`**: Menyalin file.
- **`mv`**: Memindahkan file atau direktori.
- **`rm`**: Menghapus file atau direktori.
- **`sudo`**: Memberikan hak akses root untuk menjalankan perintah.
- **`apt`**: Manajer paket untuk menginstal, menghapus, dan memperbarui perangkat lunak.

### Software Manager

- **Menggunakan GNOME Software**:
  - Buka "Ubuntu Software" dari menu aplikasi.
  - Telusuri, instal, dan perbarui aplikasi dengan mudah.

### Apt-get Package Manager

- **Dasar-dasar Apt-get**:
  - Perbarui daftar paket:
    ```bash
    sudo apt update
    ```
  - Tingkatkan semua paket terinstal:
    ```bash
    sudo apt upgrade
    ```
  - Instal paket baru:
    ```bash
    sudo apt install package_name
    ```

### Mesin Virtual

- **Instalasi VirtualBox**:
  - Instal VirtualBox dari Ubuntu Software atau dengan perintah berikut:
    ```bash
    sudo apt install virtualbox
    ```
  - Gunakan VirtualBox untuk menjalankan sistem operasi lain di dalam Ubuntu.

#### **Unduh dan Instal VirtualBox**

- Kunjungi situs web VirtualBox ([https://www.virtualbox.org/](https://www.virtualbox.org/)) dan unduh versi yang sesuai untuk sistem operasi Anda.
- Jalankan file instalasi dan ikuti petunjuk di layar.

#### **Buat Mesin Virtual Baru**

- Buka VirtualBox dan klik tombol "New".
- Berikan nama untuk mesin virtual Anda.
- Pilih jenis sistem operasi yang ingin Anda jalankan (dalam kasus ini, Ubuntu).
- Tentukan jumlah RAM yang ingin Anda alokasikan ke mesin virtual.
- Pilih hard disk untuk mesin virtual, Anda dapat membuat hard disk virtual baru atau menggunakan hard disk yang sudah ada.

1. **Pilih hard disk untuk mesin virtual Anda**:
   - **Buat hard disk virtual baru**:
     - Pilih "Create a virtual hard disk now".
     - Klik "Create".
   - **Pilih jenis file hard disk**:
     - Pilih "VDI (VirtualBox Disk Image)" dan klik "Next".
   - **Pilih jenis penyimpanan di hard disk fisik**:
     - Pilih antara "Dynamically allocated" atau "Fixed size" (dynamically allocated akan memperluas ukuran hard disk sesuai kebutuhan, sedangkan fixed size akan mengalokasikan ukuran penuh segera).
     - Klik "Next".
   - **Tentukan ukuran hard disk**:
     - Pilih ukuran untuk hard disk virtual Anda. Direkomendasikan minimal 25 GB.
     - Klik "Create".

2. **Konfigurasi tambahan (opsional)**:
   - Setelah mesin virtual dibuat, Anda dapat mengkonfigurasi pengaturan tambahan dengan memilih mesin virtual dan mengklik "Settings".
   - Beberapa pengaturan penting termasuk:
     - **System**: Atur alokasi RAM, jumlah CPU, dan urutan boot.
     - **Display**: Atur memori video dan akselerasi grafis.
     - **Storage**: Pastikan file ISO Ubuntu ditambahkan sebagai optical drive di controller IDE atau SATA.
     - **Network**: Pilih jenis jaringan (NAT, Bridged, Host-only, dll.).

3. **Mulai mesin virtual**:
   - Pilih mesin virtual baru Anda dari daftar dan klik "Start".
   - Pilih file ISO Ubuntu yang sudah Anda unduh sebelumnya sebagai sumber instalasi jika diminta.
   - Ikuti panduan instalasi Ubuntu seperti biasanya.


#### **Pilih Gambar Ubuntu**

- Pada jendela pengaturan mesin virtual, pilih "Settings" > "Storage".
- Klik ikon "Empty" dan pilih "Choose existing disk".
- Pilih file ISO Ubuntu yang Anda unduh sebelumnya.

#### **Mulai Mesin Virtual**

- Setelah pengaturan selesai, klik tombol "Start" untuk memulai mesin virtual Ubuntu.

### Instalasi dengan VMware Workstation

- **Unduh dan Instal VMware Workstation**:
  - Unduh dan instal VMware Workstation dari [https://www.vmware.com/products/workstation/workstation-pro.html](https://www.vmware.com/products/workstation/workstation-pro.html).

#### **Buat Mesin Virtual Baru**

- Buka VMware Workstation dan klik tombol "Create a New Virtual Machine".
- Pilih "Custom (advanced)" dan klik "Next".
- Pilih "I will install the operating system later" dan klik "Next".
- Pilih "Linux" sebagai sistem operasi dan "Ubuntu" sebagai versi.
- Tentukan lokasi penyimpanan untuk mesin virtual Anda.
- Pilih ukuran hard disk dan klik "Next".
- Pilih "Create a virtual disk now" dan klik "Next".
- Pilih "Store virtual disk as a single file" dan klik "Next".
- Konfigurasikan ukuran hard disk dan klik "Finish".

#### **Pilih Gambar Ubuntu**

- Pada jendela pengaturan mesin virtual, pilih "Settings" > "Hardware" > "Hard Disk".
- Pilih "Use an existing disk" dan klik "Browse".
- Pilih file ISO Ubuntu yang Anda unduh sebelumnya.

## Instalasi pada Mesin Virtual (VMware Workstation) (Lanjutan)

#### **Mulai Mesin Virtual**

- Setelah pengaturan selesai, klik tombol "Power On This Virtual Machine" untuk memulai mesin virtual Ubuntu.

### Instalasi pada Raspberry Pi

#### **Unduh Gambar Raspberry Pi OS**

- Kunjungi situs web resmi Raspberry Pi ([https://www.raspberrypi.org/software/](https://www.raspberrypi.org/software/)).
- Unduh gambar Raspberry Pi OS terbaru yang kompatibel dengan model Raspberry Pi Anda.

#### **Buat Image SD Card**

- Gunakan alat seperti Etcher atau Rufus untuk membuat image SD card dari file gambar Raspberry Pi OS yang diunduh.
- Pastikan SD card yang Anda gunakan memiliki kapasitas yang cukup untuk gambar Raspberry Pi OS.

#### **Boot Raspberry Pi**

- Masukkan SD card ke slot SD card di Raspberry Pi.
- Hubungkan keyboard, mouse, dan monitor ke Raspberry Pi.
- Hubungkan Raspberry Pi ke sumber daya (adapter daya).
- Raspberry Pi akan boot dan Anda akan melihat layar desktop Raspberry Pi OS.

##  Penggunaan Ubuntu

### Terminal dan Command Line

- **Dasar-dasar Terminal**:
  - Buka terminal dengan menekan `Ctrl+Alt+T`.
  - Gunakan perintah dasar seperti `ls`, `cd`, `cp`, `mv`, `rm` untuk navigasi dan manipulasi file.

#### **Perintah Dasar Terminal**

- **`ls`**: Menampilkan daftar file dan direktori.
- **`cd`**: Mengubah direktori.
- **`mkdir`**: Membuat direktori baru.
- **`cp`**: Menyalin file.
- **`mv`**: Memindahkan file atau direktori.
- **`rm`**: Menghapus file atau direktori.
- **`sudo`**: Memberikan hak akses root untuk menjalankan perintah.
- **`apt`**: Manajer paket untuk menginstal, menghapus, dan memperbarui perangkat lunak.

### Software Manager

- **Menggunakan GNOME Software**:
  - Buka "Ubuntu Software" dari menu aplikasi.
  - Telusuri, instal, dan perbarui aplikasi dengan mudah.

### Apt-get Package Manager

- **Dasar-dasar Apt-get**:
  - Perbarui daftar paket:
    ```bash
    sudo apt update
    ```
  - Tingkatkan semua paket terinstal:
    ```bash
    sudo apt upgrade
    ```
  - Instal paket baru:
    ```bash
    sudo apt install package_name
    ```

### Integrasi Git

#### **Kloning Repositori**

##### **Gunakan Git Clone**

- Instal Git jika belum terinstal:
    ```bash
    sudo apt install git
    ```
- Klon repositori:
    ```bash
    git clone repository_url
    ```

#### **Membuat Perubahan dan Kontribusi**

##### **Buat Cabang Baru**

- Buat cabang baru untuk perubahan Anda:
    ```bash
    git checkout -b branch_name
    ```

##### **Commit Perubahan**

- Commit perubahan Anda:
    ```bash
    git add .
    git commit -m "Pesan commit"
    ```

#### **Melacak Perubahan dan Pembaruan**

##### **Pull Perubahan Terbaru**

- Tarik perubahan terbaru dari cabang utama:
    ```bash
    git pull origin main
    ```

##### **Push Perubahan**

- Dorong perubahan Anda ke repositori:
    ```bash
    git push origin branch_name
    ```

### Upgrade Ubuntu

#### **Langkah-langkah Upgrade**

##### **Perbarui Daftar Paket**

- Perbarui daftar paket yang tersedia:
    ```bash
    sudo apt update
    ```

##### **Tingkatkan Semua Paket**

- Tingkatkan semua paket yang terinstal ke versi terbaru:
    ```bash
    sudo apt upgrade
    ```

##### **Mulai Ulang Sistem**

- Setelah upgrade selesai, mulai ulang sistem Anda.

#### **Solusi untuk Masalah Upgrade**

##### **Bersihkan Cache Paket**

- Jika upgrade gagal, bersihkan cache paket:
    ```bash
    sudo apt clean
    ```

##### **Gunakan Mode Recovery**

- Jika upgrade masih gagal, gunakan mode recovery untuk memperbaiki masalah:
    - Nyalakan kembali komputer dan tekan tombol yang sesuai untuk masuk ke mode recovery (biasanya F2, F8, atau Esc).
    - Pilih opsi untuk memperbaiki sistem.

###### **Langkah-langkah Memasuki Mode Recovery**

1. Nyalakan kembali komputer Anda.
2. Tekan tombol yang sesuai selama proses booting untuk mengakses menu boot. Tombol ini bisa bervariasi tergantung pada motherboard Anda, tetapi tombol umum adalah F2, F8, Esc, atau Del.
3. Pilih opsi untuk masuk ke mode "Recovery Mode" atau "Advanced Options".
4. Pilih opsi untuk memperbaiki sistem atau menjalankan mode pemulihan.
5. Ikuti petunjuk di layar untuk memperbaiki masalah yang terjadi selama proses upgrade.

##  Instalasi Ubuntu Server

### Unduh Ubuntu Server ISO

#### **Kunjungi Situs Web Ubuntu**

- Unduh file ISO Ubuntu Server dari [halaman unduhan Ubuntu](https://ubuntu.com/download/server).

### Buat USB Bootable

#### **Gunakan Etcher atau Alat Lain**

- Buat USB bootable menggunakan Etcher, seperti yang dijelaskan sebelumnya.

### Boot dari USB Drive

#### **Ikuti Langkah-langkah Booting**

- Boot dari USB drive dan pilih opsi untuk menginstal Ubuntu Server.

### Konfigurasi Pengaturan Server

#### **Ikuti Panduan Instalasi**

- Ikuti petunjuk pada layar untuk mengkonfigurasi pengaturan server, termasuk pengaturan jaringan, pengguna, dan paket tambahan yang diperlukan.

#### **Contoh Konfigurasi Server**

##### **Server Web dengan Apache**

1. **Instal Apache:**
   ```bash
   sudo apt install apache2
   ```
2. **Konfigurasi Apache:**
   - Edit file konfigurasi Apache:
     ```bash
     sudo nano /etc/apache2/sites-available/000-default.conf
     ```
   - Ubah pengaturan sesuai kebutuhan.
3. **Mulai Apache:**
   ```bash
   sudo systemctl restart apache2
   ```

##### **Server Database dengan MySQL**

1. **Instal MySQL:**
   ```bash
   sudo apt install mysql-server
   ```
2. **Konfigurasi MySQL:**
   - Jalankan perintah berikut untuk masuk ke shell MySQL:
     ```bash
     mysql -u root -p
     ```
   - Masukkan kata sandi yang Anda buat selama instalasi.
   - Buat database baru:
     ```sql
     CREATE DATABASE database_name;
     ```
   - Buat pengguna baru dan berikan hak akses ke database:
     ```sql
     CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';
     GRANT ALL PRIVILEGES ON database_name.* TO 'username'@'localhost';
     FLUSH PRIVILEGES;
     ```

##### **Server Email dengan Postfix**

1. **Instal Postfix:**
   ```bash
   sudo apt install postfix
   ```
2. **Konfigurasi Postfix:**
   - Pilih opsi "Internet Site" selama instalasi Postfix.
   - Masukkan nama domain atau alamat email Anda.
3. **Konfigurasi Server Email:**
   - Edit file konfigurasi Postfix untuk menyesuaikan pengaturan server email Anda.

###  Instalasi pada Platform Lain

#### **Instalasi pada Mesin Virtual**

##### **Instalasi dengan VirtualBox**

###### **Unduh dan Instal VirtualBox**

- Kunjungi situs web VirtualBox ([https://www.virtualbox.org/](https://www.virtualbox.org/)) dan unduh versi yang sesuai untuk sistem operasi Anda.
- Jalankan file instalasi dan ikuti petunjuk di layar.

###### **Buat Mesin Virtual Baru**

- Buka VirtualBox dan klik tombol "New".
- Berikan nama untuk mesin virtual Anda.
- Pilih jenis sistem operasi yang ingin Anda jalankan (dalam kasus ini, Ubuntu).
- Tentukan jumlah RAM yang ingin Anda alokasikan ke mesin virtual.
- Pilih hard disk untuk mesin virtual, Anda dapat membuat hard disk virtual baru atau menggunakan hard disk yang sudah ada.

1. **Pilih hard disk untuk mesin virtual Anda**:
   - **Buat hard disk virtual baru**:
     - Pilih "Create a virtual hard disk now".
     - Klik "Create".
   - **Pilih jenis file hard disk**:
     - Pilih "VDI (VirtualBox Disk Image)" dan klik "Next".
   - **Pilih jenis penyimpanan di hard disk fisik**:
     - Pilih antara "Dynamically allocated" atau "Fixed size" (dynamically allocated akan memperluas ukuran hard disk sesuai kebutuhan, sedangkan fixed size akan mengalokasikan ukuran penuh segera).
     - Klik "Next".
   - **Tentukan ukuran hard disk**:
     - Pilih ukuran untuk hard disk virtual Anda. Direkomendasikan minimal 25 GB.
     - Klik "Create".

2. **Konfigurasi tambahan (opsional)**:
   - Setelah mesin virtual dibuat, Anda dapat mengkonfigurasi pengaturan tambahan dengan memilih mesin virtual dan mengklik "Settings".
   - Beberapa pengaturan penting termasuk:
     - **System**: Atur alokasi RAM, jumlah CPU, dan urutan boot.
     - **Display**: Atur memori video dan akselerasi grafis.
     - **Storage**: Pastikan file ISO Ubuntu ditambahkan sebagai optical drive di controller IDE atau SATA.
     - **Network**: Pilih jenis jaringan (NAT, Bridged, Host-only, dll.).

3. **Mulai mesin virtual**:
   - Pilih mesin virtual baru Anda dari daftar dan klik "Start".
   - Pilih file ISO Ubuntu yang sudah Anda unduh sebelumnya sebagai sumber instalasi jika diminta.
   - Ikuti panduan instalasi Ubuntu seperti biasanya.

###### **Pilih Gambar Ubuntu**

- Pada jendela pengaturan mesin virtual, pilih "Settings" > "Storage".
- Klik ikon "Empty" dan pilih "Choose existing disk".
- Pilih file ISO Ubuntu yang Anda unduh sebelumnya.

###### **Mulai Mesin Virtual**

- Setelah pengaturan selesai, klik tombol "Start" untuk memulai mesin virtual Ubuntu.

##### **Instalasi dengan VMware Workstation**

###### **Unduh dan Instal VMware Workstation**

- Unduh dan instal VMware Workstation dari [https://www.vmware.com/products/workstation/workstation-pro.html](https://www.vmware.com/products/workstation/workstation-pro.html).

###### **Buat Mesin Virtual Baru**

- Buka VMware Workstation dan klik tombol "Create a New Virtual Machine".
- Pilih "Custom (advanced)" dan klik "Next".
- Pilih "I will install the operating system later" dan klik "Next".
- Pilih "Linux" sebagai sistem operasi dan "Ubuntu" sebagai versi.
- Tentukan lokasi penyimpanan untuk mesin virtual Anda.
- Pilih ukuran hard disk dan klik "Next".
- Pilih "Create a virtual disk now" dan klik "Next".
- Pilih "Store virtual disk as a single file" dan klik "Next".
- Konfigurasikan ukuran hard disk dan klik "Finish".

###### **Pilih Gambar Ubuntu**

- Pada jendela pengaturan mesin virtual, pilih "Settings" > "Hardware" > "Hard Disk".
- Pilih "Use an existing disk" dan klik "Browse".
- Pilih file ISO Ubuntu yang Anda unduh sebelumnya.

###### **Mulai Mesin Virtual**

- Setelah pengaturan selesai, klik tombol "Power On This Virtual Machine" untuk memulai mesin virtual Ubuntu.

#### **Instalasi pada Raspberry Pi**

##### **Unduh Gambar Raspberry Pi OS**

- Kunjungi situs web resmi Raspberry Pi ([https://www.raspberrypi.org/software/](https://www.raspberrypi.org/software/)).
- Unduh gambar Raspberry Pi OS terbaru yang kompatibel dengan model Raspberry Pi Anda.

##### **Buat Image SD Card**

- Gunakan alat seperti Etcher atau Rufus untuk membuat image SD card dari file gambar Raspberry Pi OS yang diunduh.
- Pastikan SD card yang Anda gunakan memiliki kapasitas yang cukup untuk gambar Raspberry Pi OS.

##### **Boot Raspberry Pi**

- Masukkan SD card ke slot SD card di Raspberry Pi.
- Hubungkan keyboard, mouse, dan monitor ke Raspberry Pi.
- Hubungkan Raspberry Pi ke sumber daya (adapter daya).
- Raspberry Pi akan boot dan Anda akan melihat layar desktop Raspberry Pi OS.

##  Sumber Daya dan Dukungan

### Komunitas Ubuntu

- **Forum Ubuntu**:
  - [Ubuntu Forums](https://ubuntuforums.org/): Forum resmi komunitas Ubuntu.
  - [Ask Ubuntu](https://askubuntu.com/): Situs tanya jawab untuk pengguna Ubuntu.

### Mendapatkan Bantuan dan Dukungan

- **Dokumentasi Resmi**:
  - [Ubuntu Documentation](https://help.ubuntu.com/): Dokumentasi resmi Ubuntu.
  
- **Bantuan Online**:
  - Bergabung dengan komunitas Ubuntu di platform sosial seperti Reddit, Discord, dan Telegram.

---
