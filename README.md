# papan-investigasi

# 赤い糸 Akai Ito — Papan Investigasi Digital

**Papan gabus detektif, dalam browser.** Kelola kasus, tempel bukti, dan hubungkan petunjuk dengan benang merah di kanvas interaktif yang bisa di-*pan* dan *zoom* — semuanya berjalan 100% di sisi klien, tanpa server dan tanpa akun.

> *"Setiap kasus adalah papan investigasi tersendiri — kumpulkan bukti, hubungkan benang merah."*

![Lisensi MIT](https://img.shields.io/badge/lisensi-MIT-a91e22) ![Tanpa dependensi build](https://img.shields.io/badge/build-tidak%20diperlukan-c9b98d) ![Single file](https://img.shields.io/badge/single--file-HTML-2a2318)

---

## ✨ Fitur

- **Manajemen kasus** — buat banyak kasus, masing-masing dengan tanggal mulai, batas waktu, status, dan progres tenggat waktu visual.
- **Papan bukti interaktif** — tempel data sebagai *pin* di kanvas bebas, geser (drag), *pan* & *zoom*, cari, dan filter.
- **8 jenis data**: Dokumen, Foto, Audio, Video, Catatan, Orang, Tempat, dan Lainnya — masing-masing dengan ikon dan warna sendiri.
- **Benang merah (koneksi)** — hubungkan dua data dengan garis, beri label hubungan (mis. "mengenal", "ditemukan di").
- **Lampiran file** — seret & lepas foto, audio, video, atau dokumen langsung ke sebuah data.
- **Berkas Kesimpulan Kasus** — formulir kronologi, lokasi, pelaku, saksi, alibi, motif, dan bukti kunci untuk menutup kasus, lengkap dengan animasi perayaan "解決 / CASE SOLVED".
- **Mode terang & gelap**, tema bertema washi/kertas tua ala arsip detektif Jepang.
- **Cadangkan / pulihkan data** ke berkas `.json`, plus opsi atur ulang total.
- **Tanpa build step** — satu berkas HTML, buka langsung di peramban.

## 🚀 Menjalankan

Tidak perlu instalasi atau build. Cukup buka `index.html` di peramban modern (Chrome, Firefox, Edge, Safari terbaru):

```bash
git clone https://github.com/<username>/akai-ito.git
cd akai-ito
open index.html   # atau: xdg-open index.html / start index.html
```

Atau jalankan server statis sederhana bila ingin mengakses via `http://localhost`:

```bash
npx serve .
# atau
python3 -m http.server 8000
```

Bisa juga langsung dihosting gratis lewat **GitHub Pages** — aktifkan Pages pada branch `main` dan buka `index.html` sebagai halaman utama.

## 🗄️ Penyimpanan Data

Seluruh data (kasus, data/bukti, hubungan, lampiran) disimpan di **`localStorage`** peramban milikmu sendiri — tidak dikirim ke server mana pun. Karena itu:

- Data bersifat lokal per-peramban/per-perangkat.
- Gunakan tombol **Cadangkan (backup)** secara berkala untuk mengekspor seluruh data ke berkas `.json`.
- Gunakan **Pulihkan (restore)** untuk memuat kembali cadangan tersebut, termasuk saat pindah perangkat.

## 🛠️ Teknologi

- HTML, CSS, dan JavaScript murni (vanilla), + [jQuery](https://jquery.com/) untuk manipulasi DOM.
- Font [Shippori Mincho](https://fonts.google.com/specimen/Shippori+Mincho), [Zen Kaku Gothic New](https://fonts.google.com/specimen/Zen+Kaku+Gothic+New), dan [Zen Old Mincho](https://fonts.google.com/specimen/Zen+Old+Mincho) dari Google Fonts.
- Tidak ada framework, bundler, atau dependensi backend — satu berkas `index.html` mandiri.

## 📂 Struktur Repositori

```
.
├── index.html   # Seluruh aplikasi (markup, gaya, logika)
├── README.md
└── LICENSE
```

## 🤝 Kontribusi

Kontribusi, laporan bug, dan ide fitur dipersilakan lewat *Issues* atau *Pull Request*. Beberapa ide pengembangan lanjutan:

- Ekspor papan sebagai gambar (PNG/PDF).
- Multi-bahasa (saat ini antarmuka berbahasa Indonesia).
- Sinkronisasi opsional lewat penyimpanan cloud.

## 📄 Lisensi

Proyek ini dirilis di bawah [Lisensi MIT](LICENSE) — bebas digunakan, dimodifikasi, dan didistribusikan.

---

<sub>Dibuat dengan 🧵 untuk siapa pun yang suka menyusun potongan puzzle sebuah kasus.</sub>
