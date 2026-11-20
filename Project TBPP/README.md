# Media Pembelajaran Interaktif: Perdagangan Internasional

Website media pembelajaran interaktif bertema **Perdagangan Internasional (International Trade)** dengan desain minimalis, modern, bersih, dan kaya fitur interaktivitas serta gamifikasi.

---

## 📁 Struktur Website & Halaman

Website ini dibangun menggunakan konsep Single Page Application (SPA) modular murni (HTML5, Tailwind CSS via CDN, Lucide Icons, dan Vanilla JavaScript) tanpa dependensi berat, sehingga **dapat langsung dibuka di browser apa pun hanya dengan double-click pada file `index.html`**.

### 1. 🏠 Home (Beranda)
- **Hero Banner Minimalis & Elegan:** Judul inspiratif, subjudul penjelasan, dan tombol Call-To-Action (CTA) langsung menuju materi atau kuis.
- **Kartu Cuplikan Topik:** Tiga kartu pintasan cepat menuju Konsep & Teori, Video/Simulasi, dan Evaluasi Game.
- **Peta Alur Belajar (Roadmap):** Panduan 4 tahap belajar mandiri yang sistematis untuk siswa/mahasiswa.

### 2. 📚 Materi (Interaktif & Multimedia)
Dilengkapi dengan navigasi sub-tab yang responsif dan tidak membosankan:
- **Sub-Tab 1: Konsep & Faktor:**
  - Pengertian Perdagangan Internasional, Ekspor, dan Impor.
  - Tabel komparasi interaktif: Perbedaan transaksi dalam negeri vs. luar negeri.
  - Kartu faktor pendorong vs. faktor penghambat dengan indikator visual.
- **Sub-Tab 2: Teori & Kebijakan Proteksi:**
  - Perbandingan Teori Keunggulan Mutlak (Adam Smith) & Teori Keunggulan Komparatif (David Ricardo).
  - 6 Kartu instrumen kebijakan: Tarif/Bea Masuk, Kuota Impor, Subsidi Ekspor, Dumping, Larangan Impor, dan Diskriminasi Harga.
- **Sub-Tab 3: Devisa & Sistem Pembayaran:**
  - Sumber dan fungsi cadangan devisa serta mata uang kuat (*hard currency*).
  - Instrumen pembayaran internasional: Letter of Credit (L/C), Cash in Advance, Open Account, dan Kompensasi Pribadi.
- **Sub-Tab 4: Video & Simulator Interaktif:**
  - Pemutar video YouTube responsif (bisa diganti dengan link video pembelajaran Anda sendiri).
  - **Simulator Interaktif Spesialisasi:** Siswa dapat memilih komoditas untuk melihat hasil efisiensi perdagangan secara langsung.

### 3. 🎮 Evaluasi (2 Mode Game Interaktif)
- **Mode 1: Kuis Interaktif (Ala Quizizz / Kahoot):**
  - Timer mundur per soal (20 detik).
  - Skor dinamis (poin dasar + bonus sisa waktu + combo multiplier).
  - Sistem **Streak Combo** (🔥 Combo x2, x3, dst).
  - Efek suara sintetis browser (*Web Audio API* - tidak perlu file MP3 eksternal, bebas error CORS).
  - Tombol pilihan bernuansa Quizizz dengan feedback langsung dan pembahasan detail setiap soal.
  - Layar hasil akhir lengkap dengan Akurasi %, Skor Akhir, dan Rekor Streak.
- **Mode 2: Game Mencocokkan Pasangan (Match & Connect):**
  - Menguji pemahaman konsep istilah ekonomi (Kolom A: Istilah, Kolom B: Definisi acak).
  - Mekanisme klik untuk memasangkan kartu.
  - Animasi visual: kartu hijau saat benar dan getar merah (*shake animation*) saat salah.
  - Notifikasi selebrasi saat semua istilah berhasil dipasangkan.

### 4. 👤 Profil Penyusun
- Foto profil avatar elegan dengan badge terverifikasi.
- Nama lengkap dan peran/gelar pengembang.
- Kartu metadata institusi, target sasaran pengguna, dan tahun rilis.
- Tautan kontak (Email, Instagram/Medsos).
- Kutipan/pesan motivasi pembelajaran ekonomi global.

---

## 🚀 Cara Menjalankan Website

1. Masuk ke folder: `c:\Users\Dragon\Documents\Project TBPP`
2. **Double-click file `index.html`** untuk membukanya langsung di Google Chrome, Microsoft Edge, Mozilla Firefox, atau browser favorit Anda.
3. Tidak memerlukan instalasi server lokal (Node.js/XAMPP/dll), semua fitur interaktif langsung aktif!

---

## 🛠️ Panduan Kustomisasi Sederhana

- **Mengganti Soal Kuis:** Buka `index.html`, cari variabel `const quizData = [...]` di bagian JavaScript, lalu sesuaikan pertanyaan, pilihan jawaban, kunci jawaban (`correct: true`), dan penjelasannya.
- **Mengganti Istilah Game Cocokkan:** Cari variabel `const matchingPairs = [...]` di `index.html` untuk menambah atau mengganti istilah ekonomi.
- **Mengganti Video Edukasi:** Ganti URL embed pada tag `<iframe>` di bagian materi video (`https://www.youtube-nocookie.com/embed/...`).
- **Mengganti Identitas Penyusun:** Edit teks nama, foto avatar (`src="..."`), dan institusi pada bagian `<section id="section-profil">`.
