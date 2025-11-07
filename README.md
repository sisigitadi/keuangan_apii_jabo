# Aplikasi Pencatatan Keuangan APII DPW Jabodetabek

## 📋 Daftar Isi
- [Tentang Aplikasi](#tentang-aplikasi)
- [Fitur Utama](#fitur-utama)
- [Teknologi](#teknologi)
- [Instalasi](#instalasi)
- [Panduan Penggunaan](#panduan-penggunaan)
- [Kredensial Test](#kredensial-test)
- [Struktur Aplikasi](#struktur-aplikasi)
- [Kategori Transaksi](#kategori-transaksi)
- [Responsive Design](#responsive-design)
- [Kontak & Support](#kontak--support)

## 🎯 Tentang Aplikasi

**Aplikasi Pencatatan Keuangan APII DPW Jabodetabek** adalah aplikasi web yang dirancang untuk membantu organisasi Yayasan Apologet Islam Indonesia (APII) Dewan Pimpinan Wilayah Jabodetabek dalam mengelola dan mencatat transaksi keuangan secara terstruktur dan efisien.

Aplikasi ini dibangun menggunakan teknologi web modern (HTML5, CSS3, JavaScript) dan tidak memerlukan server backend, sehingga dapat diakses secara offline dan data disimpan secara lokal di browser.

## ✨ Fitur Utama

### 1. **Autentikasi & Manajemen User**
   - Sistem login dengan username dan password
   - Tiga level akses: Admin, Manager, dan Viewer
   - Manajemen user - tambah/hapus user account
   - Session management dengan localStorage

### 2. **Dashboard Keuangan**
   - Ringkasan aset bersih (Penerimaan - Pengeluaran)
   - Total penerimaan bulanan/periode
   - Total pengeluaran bulanan/periode
   - Daftar 10 transaksi terbaru dengan status income/expense

### 3. **Pencatatan Transaksi**
   - Form input transaksi dengan validasi
   - Pilih tipe: Penerimaan atau Pengeluaran
   - Kategori transaksi yang terstruktur
   - Input tanggal, nominal, dan keterangan
   - Pencatatan automatic user dan timestamp

### 4. **Laporan Keuangan**
   - Ringkasan laporan: Total Penerimaan, Pengeluaran, Surplus/Defisit
   - Perhitungan real-time berdasarkan data transaksi
   - Format mata uang IDR (Indonesian Rupiah)

### 5. **Manajemen User (Admin Only)**
   - Daftar semua user dengan role
   - Tambah user baru dengan role pilihan
   - Hapus user (kecuali admin yang sedang login)
   - Password management

### 6. **Backup & Export Data**
   - Export transaksi ke format JSON
   - Backup otomatis di localStorage browser
   - Restore dari backup saat reload page

### 7. **UI/UX Modern**
   - Design responsive untuk desktop, tablet, mobile
   - Logo APII permanen embedded di header
   - Judul aplikasi 3 baris yang informatif
   - Footer dengan copyright & email contact
   - Theme warna emas yang elegant

## 🛠 Teknologi

- **Frontend:** HTML5, CSS3, JavaScript ES6+
- **Storage:** Browser localStorage API
- **Styling:** CSS Grid, Flexbox, Media Queries
- **Compatibility:** Chrome, Firefox, Safari, Edge (modern browsers)
- **Responsive:** Mobile-first design approach

## 📦 Instalasi

### Syarat Minimal
- Browser modern (Chrome, Firefox, Safari, Edge)
- Internet untuk download file (atau akses file lokal)

### Cara Instalasi

1. **Download file `index.html`**
   - Ekstrak file dari repository

2. **Simpan di folder project Anda:**
   ```
   D:\Projects\APII Jabo\Bendahara\keuangan_apii_jabo\index.html
   ```

3. **Buka di browser:**
   - Klik dua kali file `index.html`
   - Atau buka dengan kanan klik > Open with > Browser

4. **Aplikasi siap digunakan!**
   - Tidak perlu instalasi server atau database

### Upload ke GitHub (Optional)

```bash
# Clone repository
git clone https://github.com/username/keuangan_apii_jabo.git
cd keuangan_apii_jabo

# Tambahkan file
git add index.html logo-apii-jabo.jpg

# Commit
git commit -m "Initial commit: Aplikasi Pencatatan Keuangan APII"

# Push ke repository
git push origin main
```

## 📖 Panduan Penggunaan

### 1. Login

**Halaman Awal:**
- Masukkan username pada field "Username"
- Masukkan password pada field "Password"
- Klik tombol "🔓 Login"

**Fitur Khusus:**
- Test credentials tersedia di bawah form
- Setelah login berhasil, session disimpan sampai logout
- Auto-redirect ke dashboard

### 2. Dashboard

**Tampilan Utama:**
- **Aset Bersih:** Total penerimaan dikurangi pengeluaran
- **Total Penerimaan:** Jumlah semua transaksi penerimaan
- **Total Pengeluaran:** Jumlah semua transaksi pengeluaran

**Transaksi Terbaru:**
- 10 transaksi terbaru ditampilkan
- Warna biru untuk Penerimaan (+)
- Warna merah untuk Pengeluaran (-)
- Admin dapat menghapus transaksi dengan tombol 🗑️

### 3. Input Transaksi (Tab Transaksi)

**Form Input:**
1. Pilih **Tanggal** - default hari ini
2. Masukkan **Nominal** dalam Rupiah (tanpa titik/koma)
3. Pilih **Tipe** - Penerimaan atau Pengeluaran
4. Pilih **Kategori** - sesuai tipe yang dipilih
5. Isi **Keterangan** - detail transaksi
6. Klik **💾 Simpan**

**Validasi:**
- Semua field wajib diisi
- Nominal harus angka positif
- Data disimpan otomatis ke localStorage

### 4. Laporan Keuangan (Tab Laporan)

**Informasi yang Ditampilkan:**
- **Total Penerimaan:** Semua transaksi penerimaan
- **Total Pengeluaran:** Semua transaksi pengeluaran
- **Surplus/Defisit:** Selisih (positif atau negatif)

**Interpretasi:**
- Nilai positif = Surplus (kelebihan penerimaan)
- Nilai negatif = Defisit (kekurangan penerimaan)

### 5. Settings (Tab Settings)

#### A. Users Management
- **Daftar Users:** Semua user dengan role-nya
- **Tambah User:** 
  - Klik tombol "➕ Tambah User"
  - Masukkan username, password, role
  - User otomatis ditambahkan
- **Hapus User:** Admin dapat hapus user lain (not yourself)

#### B. Data Backup
- **Export JSON:** Download semua transaksi dalam format JSON
  - File bernama: `export_YYYY-MM-DD.json`
  - Berisi: transaksi, tanggal export, user yang export
- **Hapus Data:** Menghapus semua transaksi (irreversible!)

## 🔐 Kredensial Test

Gunakan kredensial berikut untuk testing:

| Username | Password | Role | Keterangan |
|----------|----------|------|-----------|
| admin | admin | Admin | Akses penuh, bisa hapus transaksi & user |
| manager | manager | Manager | Akses standar, bisa input transaksi |
| viewer | viewer | Viewer | Akses read-only, hanya lihat data |

**Catatan:**
- Ganti password setelah deployment
- Jangan share kredensial ke pihak yang tidak perlu akses

## 📊 Struktur Aplikasi

### File Utama
- `index.html` - Aplikasi lengkap (single page application)
- `logo-apii-jabo.jpg` - Logo APII (embedded dalam HTML)

### Data Storage
- **Transactions:** Daftar semua transaksi keuangan
- **Users:** Daftar user dengan credentials dan role
- **CurrentUser:** User yang sedang login

Semua data disimpan di `localStorage` browser dengan key:
- `transactions` - array transaksi
- `users` - array users
- `currentUser` - user session

### Navigation Tabs
1. **Dashboard (📊)** - Ringkasan keuangan & transaksi terbaru
2. **Transaksi (➕)** - Input transaksi baru
3. **Laporan (📈)** - Laporan keuangan detail
4. **Settings (⚙️)** - Manajemen user & data

## 💰 Kategori Transaksi

### Penerimaan
- Sumbangan/Donasi
- Hibah/Grant
- Pendapatan Program
- Pendapatan Investasi
- Pendapatan Lainnya

### Pengeluaran
- Program Utama
- Program Pendidikan
- Program Kesehatan
- Program Sosial
- Beban Penggajian
- Beban Administrasi
- Beban Operasional
- Beban Lainnya

## 📱 Responsive Design

Aplikasi dioptimalkan untuk berbagai ukuran layar:

| Device | Breakpoint | Optimasi |
|--------|-----------|----------|
| Desktop | 1200px+ | Layout horizontal optimal, full features |
| Large Tablet | 992-1199px | Layout sedikit compressed, masih nyaman |
| Tablet | 768-991px | 2-column grid, responsive navigation |
| Mobile | 481-767px | 1-column layout, stacked header |
| Small Phone | ≤480px | Minimal layout, touch-friendly buttons |

### Fitur Responsive
- ✅ Logo scaling dinamis (65-90px)
- ✅ Font size adaptif untuk readability
- ✅ Touch-friendly buttons untuk mobile
- ✅ Scrollable tabs untuk navigation
- ✅ Form inputs dengan font 16px (prevent zoom)
- ✅ Flexible grid untuk cards

## 🎨 Design System

### Warna
- **Primary:** #D4AF37 (Gold) - Header, buttons, accents
- **Secondary:** #C9A961 (Dark Gold) - Gradient
- **Income:** #28a745 (Green) - Transaksi penerimaan
- **Expense:** #dc3545 (Red) - Transaksi pengeluaran
- **Background:** Linear gradient #F9F7F4 to #F5F3F1

### Typography
- **Font Family:** Segoe UI, Tahoma, Geneva, Verdana, sans-serif
- **Heading:** Bold, size 1.5em
- **Body:** Regular, size 0.95-1em
- **Small:** Size 0.8-0.85em untuk footer/metadata

### Component
- **Card:** Gradient background, shadow, rounded corners
- **Button:** Gradient, hover effect (translateY -2px)
- **Input:** Border 2px, focus color gold
- **Transaction Item:** Border-left colored, flexbox layout

## 💾 Data Format

### Struktur Transaksi
```json
{
  "id": 1699428000000,
  "date": "2025-11-08",
  "amount": 500000,
  "type": "Penerimaan",
  "category": "Sumbangan/Donasi",
  "description": "Donasi dari Budi Santoso",
  "user": "admin",
  "timestamp": "2025-11-08T04:00:00.000Z"
}
```

### Struktur User
```json
{
  "id": 1,
  "username": "admin",
  "password": "admin",
  "role": "Admin"
}
```

## 🔒 Keamanan

**Catatan Penting:**
- ⚠️ Aplikasi ini untuk internal use only
- ⚠️ Jangan expose ke internet publik tanpa security layer
- ⚠️ Password disimpan plain-text di localStorage (development only)
- ⚠️ Untuk production, implementasikan:
  - Backend server dengan authentication
  - Password hashing (bcrypt, argon2)
  - HTTPS encryption
  - Database untuk persistent storage

## 🚀 Deployment

### Local Use
- Download `index.html` dan simpan di folder
- Buka di browser (file:// protocol)

### Web Server
```bash
# Copy file ke server web
cp index.html /var/www/html/keuangan/

# Akses melalui URL
http://localhost/keuangan/index.html
```

### GitHub Pages (Static Hosting)
```bash
# Push ke GitHub
git push origin main

# Enable GitHub Pages di repository settings
# Akses di: https://username.github.io/keuangan_apii_jabo/
```

## 📞 Kontak & Support

**Developer:** SigitAdi  
**Email:** si.sigitadi@gmail.com  
**Copyright:** © 2025

### Feedback & Bug Report
- Hubungi melalui email di footer aplikasi
- Atau email: si.sigitadi@gmail.com

### Updates & Changelog
- v1.0 (Nov 2025) - Initial release
  - Login & authentication
  - Dashboard & transaction management
  - Financial reports
  - User management
  - Responsive design
  - Footer dengan copyright & contact

## 📄 Lisensi

Aplikasi ini dikembangkan untuk APII DPW Jabodetabek.  
Penggunaan hanya untuk internal organizational use.

---

**Terima kasih telah menggunakan Aplikasi Pencatatan Keuangan APII DPW Jabodetabek!** 🙏