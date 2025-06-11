# 📚 Libralystic – Library Management System (Admin Only)

**Libralystic** adalah aplikasi *Library Management System (LMS)* berbasis desktop yang dirancang khusus untuk **admin** perpustakaan dalam membantu proses digitalisasi pengelolaan koleksi dan transaksi. Aplikasi ini mencakup pendataan buku, pencatatan peminjaman dan pengembalian, hingga pencetakan laporan, semuanya dikendalikan melalui antarmuka admin yang intuitif dan efisien.

> ⚠️ **Catatan**: Aplikasi ini ditujukan hanya untuk penggunaan oleh **administrator** perpustakaan. Tidak ada fitur login/panel khusus untuk pengguna umum atau anggota.

---

## 🎯 Tujuan Aplikasi

Libralystic bertujuan untuk:
- Memberikan sistem manajemen perpustakaan yang terpusat bagi admin.
- Mempermudah pencatatan dan pelacakan transaksi.
- Mendukung pelaporan berbasis data secara real-time.
---

## 🧩 Fitur Utama

Aplikasi Libralystic terbagi dalam tiga bagian utama:

### 1️⃣ Halaman Data (Admin-Only)
Menu ini berfungsi untuk mengatur seluruh data utama perpustakaan, terdiri dari:
- **Dashboard** – Menampilkan ringkasan peminjaman, jumlah anggota, dan koleksi buku.
- **Anggota** – Menambahkan dan mengelola data pengguna atau peminjam.
- **Daftar Buku** – Mengelola koleksi buku perpustakaan.
- **Kategori** – Mengatur kategori buku (fiksi, non-fiksi, referensi, agama, dll.).
- **Penerbit** – Mendata dan mengelola informasi penerbit buku.

### 2️⃣ **Transaksi**
Menu ini mencatat aktivitas peminjaman dan pengembalian buku:
- **Peminjaman** – Mencatat transaksi peminjaman berdasarkan anggota dan buku.
- **Pengembalian** – Mencatat pengembalian buku serta menghitung keterlambatan jika ada.

### 3️⃣ **Laporan**
Menu ini menyajikan rekap riwayat peminjaman:
- **Laporan Peminjaman** – Menampilkan seluruh riwayat peminjaman yang dapat dicetak sebagai dokumen laporan (PDF/Print).

---

## 🎨 Fokus Desain UI

Desain UI difokuskan pada kemudahan penggunaan oleh admin:
- Layout menggunakan **AbsoluteLayout** untuk fleksibilitas desain.
- Antarmuka ringan dengan tema **FlatLaf**.
- Dukungan ikon modern dari **Flaticon** dan **Icon8**.
- Menampilkan data dalam bentuk **panel interaktif**, bukan hanya tabel.
---

## 🛠️ Tools & Requirement

| Kebutuhan          | Digunakan Untuk                                    |
|--------------------|----------------------------------------------------|
| 💻 NetBeans        | Pengembangan kode program (JavaScript, JavaSwing) |
| 🧩 Laragon         | Local server (Apache, MySQL)                      |
| 🗃️ MySQL Workbench | Desain & manajemen database visual                |
| 🧮 SQLyog Community| Manajemen database berbasis GUI                   |
| 🎨 Flaticon        | Sumber ikon untuk antarmuka                       |
| 🎨 Icon8           | Tambahan ikon dan elemen visual                   |
| ☕ JDK 23 (Default)| Versi Java yang digunakan untuk kompilasi         |

---

## 📦 Library yang Digunakan

Berikut adalah *external libraries* yang digunakan dalam aplikasi:

| Library                      | Kegunaan                                 |
|------------------------------|------------------------------------------|
| `datachooser.jar`            | Komponen pemilihan tanggal               |
| `mysql-connector-j-9.3.0.jar`| Koneksi database MySQL dari Java         |
| `AbsoluteLayout.jar`         | Manajemen layout manual di UI            |
| `flatlaf-3.2.1.jar`          | Tampilan tema modern untuk desktop       |

> 📁 Semua file `.jar` sudah dimasukkan ke folder **Libraries** di dalam proyek NetBeans.

---

## 📁 Struktur Direktori Proyek

📂 Libralystic/
├── 📁 src/
│ ├── 📁 Config/
│ │ └── Koneksi.java
│ ├── 📁 Icon/
│ ├── 📁 Main/
│ │ ├── Dashboard.java
│ │ ├── DaftarBuku.java
│ │ ├── MenuItem.java
│ │ ├── MenuUtama.java
│ │ ├── Peminjaman.java
│ │ ├── SignUp.java
│ │ └── panelAnggota.java
│ ├── 📁 View/
│ │ ├── FormLogin.java
│ │ ├── MenuBuku.java
│ │ ├── MenuDashboard.java
│ │ ├── MenuKategori.java
│ │ ├── MenuPeminjaman.java
│ │ ├── MenuPenerbit.java
│ │ └── MenuPengembalian.java
├── 📁 img/
├── 📁 Test Packages/
├── 📁 Libraries/
│ ├── datechooser.jar
│ ├── mysql-connector-j-9.3.0.jar
│ ├── AbsoluteLayout.jar
│ ├── flatlaf-3.2.1.jar
│ └── JDK 23 (Default)
