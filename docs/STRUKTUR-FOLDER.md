# 📂 Struktur Folder - Kursus HTML Anak SD

```text
materi-HTML/
│
├── 📄 index.html                 🏠 Halaman utama (hub semua pertemuan)
├── 🧪 playground.html            Editor Coba-Coba (offline, untuk semua pertemuan)
├── 📋 README.md                  Dokumentasi utama
│
├── 📁 assets/
│     ├── kursus.css              Gaya bersama: warna, huruf, nav, kotak, tabel, tombol
│     └── slides.css              Tema slide reveal.js (dipakai bersama kursus.css)
│
├── 📁 pertemuan-1/materi/        🚀 Dasar HTML (ada kode akses)
├── 📁 pertemuan-2/materi/        🎨 Gambar & Warna
├── 📁 pertemuan-3/materi/        🔗 Link & Navigasi
├── 📁 pertemuan-4/materi/        🎯 Mini Project & Presentasi
├── 📁 pertemuan-5/materi/        📋 List & Tabel
├── 📁 pertemuan-6/materi/        📦 Kotak & Tombol
│     ├── index.html              ⭐ Presentasi (slide reveal.js)
│     ├── template-siswa.html     ✍️ Template tugas siswa
│     └── cheat-sheet.html        📝 Referensi cepat
│
├── 📁 docs/
│     ├── PANDUAN-INSTRUKTUR.md   Cara mengajar tiap pertemuan
│     ├── STRUKTUR-FOLDER.md      File ini
│     ├── FITUR-IMPROVEMENTS.md   Catatan fitur (Pertemuan 1)
│     └── OPTIMASI-LAPTOP.md      Catatan ukuran layar (Pertemuan 1)
│
└── 📁 reference/
      └── KURSUS HTML ANAK SD.pdf Silabus asli
```

Setiap folder `pertemuan-N/materi/` berisi 3 file yang sama polanya: `index.html`, `template-siswa.html`, dan `cheat-sheet.html`.

## 📌 Deskripsi File

### 🎯 Untuk Instruktur

- **index.html (root)**: pintu masuk; berisi kartu tiap pertemuan dan tombol Editor Coba-Coba.
- **pertemuan-N/materi/index.html**: slide presentasi. Navigasi pakai SPASI / panah, ESC untuk overview.
  Hanya Pertemuan 1 yang memakai kode akses (`html2025`).

### 👨‍🎓 Untuk Siswa

- **template-siswa.html**: instruksi tugas, kerangka kode, checklist debug, dan penilaian diri.
- **cheat-sheet.html**: tabel tag, contoh kode, dan troubleshooting.
- **playground.html**: tempat mengetik HTML dan langsung melihat hasilnya, tanpa Notepad dan tanpa internet.

### 📚 Dokumentasi

- **README.md**: ringkasan materi dan outcome tiap pertemuan.
- **docs/PANDUAN-INSTRUKTUR.md**: rundown, tips mengajar, troubleshooting, dan penilaian.

## 🔗 Aturan Navigasi Antar File

- Semua link memakai path relatif, jadi folder bisa dipindah atau disalin ke flashdisk tanpa rusak.
- Dari dalam `pertemuan-N/materi/`, kembali ke root memakai `../../`.
- Setiap halaman punya nav-bar ke Beranda, file lain di pertemuan yang sama, serta pertemuan sebelum/sesudahnya.

## ➕ Menambah Pertemuan Baru

1. Salin folder pertemuan terakhir, ganti nomornya (mis. `pertemuan-7`).
2. Ganti isi slide, template, dan cheat sheet. Tambahkan warna sampul baru di `assets/kursus.css`
   (`[data-pertemuan="7"] { --aksen: ...; }`) dan pasang `data-pertemuan="7"` di `<body>`.
3. Tambahkan baris baru di daftar pertemuan `index.html` (root).
4. Tambahkan link "Pertemuan berikutnya →" di nav-bar ketiga file pertemuan sebelumnya.
5. Perbarui `README.md` dan dokumen ini.

## 🌐 Kebutuhan Internet

- Semua slide presentasi (Pertemuan 1-6) memuat reveal.js dari CDN, jadi **perlu internet** saat dibuka.
- Template, cheat sheet, dan `playground.html` bisa dipakai **tanpa internet** (huruf otomatis diganti huruf sistem).
