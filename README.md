# Tangga Curi Poin

Aplikasi web papan skor dan layar host untuk game show kuis trivia Indonesia (Tim Merah vs Tim Biru). Dibuat satu file HTML tanpa build step, tanpa instalasi package, dan langsung jalan di browser.

Akses langsung: https://reynaldirp.github.io/trivia-apps/

## Cara pakai

Cukup buka `index.html` di browser (Chrome, Edge, Firefox, Safari).

Tidak butuh Node.js, server, atau koneksi internet saat bertanding. Semua styling dan suara sintetis berjalan langsung di browser lewat Tailwind CDN dan Web Audio API.

## Aturan main (reli 4 tangga)

Setiap babak memakai 4 anak tangga petunjuk yang makin lama makin mudah, tapi nilainya turun (400, 300, 200, 100 poin).

Alur giliran berjalan bergantian (ping-pong):
1. **Tangga 1 (400 poin):** Tim pertama punya 15 detik untuk menjawab.
2. **Tangga 2 (300 poin):** Jika tim pertama salah atau pasrah, giliran pindah ke tim lawan dengan petunjuk kedua.
3. **Tangga 3 (200 poin):** Jika tim kedua salah, giliran kembali ke tim pertama dengan petunjuk ketiga.
4. **Tangga 4 (100 poin):** Jika masih salah, kesempatan terakhir diberikan ke tim lawan.
5. **Hangus (0 poin):** Babak hangus jika kedua tim gagal sampai tangga ke-4.

Host bertindak sebagai juri penuh. Peserta menjawab lisan atau pakai bel fisik di panggung, lalu host yang menekan tombol penilaian di layar.

## Tombol pintasan host

Jalankan game tanpa repot klik mouse:

| Tombol | Fungsi |
| --- | --- |
| `1` atau `A` | Jawaban benar untuk Tim Merah |
| `2` atau `B` | Jawaban benar untuk Tim Biru |
| `X` atau `Spasi` | Salah / oper giliran ke lawan dan turun tangga |
| `T` | Mulai atau jeda timer 15 detik |
| `R` | Reset timer ke 15 detik |
| `H` | Buka atau tutup contekan kunci jawaban host |
| `N` | Buka anak tangga berikutnya secara manual |
| `F` | Layar penuh (fullscreen) |
| `←` / `→` | Pindah babak sebelumnya / berikutnya |

## Struktur folder

```text
trivia-apps/
├── index.html        # Satu-satunya file aplikasi (host console & arena)
├── README.md         # Panduan ringkas aplikasi
├── PRODUCT.md        # Spesifikasi produk dan alur kerja
├── DESIGN.md         # Catatan palet warna dan antarmuka
└── screenshots/      # Arsip tangkapan layar antarmuka
```

## Kelola soal

Klik tombol ikon buku/soal di pojok kanan atas layar untuk menambah pertanyaan baru atau ekspor/impor paket soal format JSON. Soal tersimpan otomatis di LocalStorage browser host.
