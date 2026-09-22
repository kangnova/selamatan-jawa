# Selamatan Jawa

Kalkulator jadwal selamatan tradisi Jawa — hitung kapan Nelung Dina (3), Mitung Dina (7), Matang Puluh (40), Nyatus (100), Mendhak 1 & 2 tahun, sampai Nyewu (1000 hari) jatuh, lengkap dengan hari dan pasaran (weton).

A single-file web app to calculate Javanese death-commemoration (*selamatan*) schedules — 3, 7, 40, 100 days, 1 & 2 years, and 1000 days (*nyewu*) — including the Javanese day and *pasaran* (*weton*).

## Demo Langsung

Coba langsung di: https://selamatan-jawa.vercel.app

## Fitur

- Masukkan tanggal wafat, langsung dapat daftar lengkap 7 tahap selamatan beserta tanggal Masehi, hari, pasaran, weton, dan neptu.
- Pilihan waktu wafat: siang/sebelum maghrib atau malam/sesudah maghrib (yang sesudah maghrib otomatis geser ke hari berikutnya).
- Koreksi pasaran manual (opsional) bila hasil otomatis berbeda dengan keyakinan keluarga.
- Pilihan hitungan 1 tahun: tradisional Jawa/Hijriah (354 hari) atau Masehi (365 hari).
- Penanda status tiap tahap: sudah lewat / hari ini / akan datang.
- Catatan "malam sebelumnya" — karena acara lazim digelar malam sebelum tanggal jatuh.
- Tombol salin jadwal (teks) dan cetak.
- Sepenuhnya berjalan di perangkat (client-side), tanpa server, tanpa data diunggah.

## Cara Pakai

1. Buka `index.html` di browser.
2. Isi tanggal wafat (otomatis terisi hari ini).
3. Atur waktu wafat dan pilihan lain sesuai kebutuhan.
4. Tekan "Hitung Jadwal".

## Cara Kerja Hitungan

Kalender Jawa menggabungkan dua siklus: hari 7-harian (Senin–Minggu) dan pasaran 5-harian (Legi, Pahing, Pon, Wage, Kliwon). Kombinasi keduanya disebut *weton*, yang berulang setiap 35 hari (*selapan*).

Setiap tahap selamatan memakai rumus baku (hari ke-N, pasaran ke-M):

| Selamatan | Hari ke- | Rumus |
| --- | --- | --- |
| Nelung Dina | 3 | LUSARLU |
| Mitung Dina | 7 | TUSARO |
| Matang Puluh | 40 | MASARMA |
| Nyatus Dina | 100 | ROSARMA |
| Mendhak Pisan | 354 | PATSARPA |
| Mendhak Pindho | 708 | ROSARPAT |
| Nyewu | 1000 | NEMSARMA |

Acuan (*anchor*) pasaran: 17 Agustus 1945 = Jumat Legi.

Aturan pokok: hari wafat dihitung sebagai hari ke-1 (inklusif); wafat sesudah maghrib dihitung masuk hari berikutnya; satu tahun dihitung 354 hari (tahun Jawa/Hijriah) pada mode tradisional.

## Teknologi

HTML + CSS + JavaScript murni dalam satu file. Tanpa framework, tanpa dependensi, tanpa build.

## Menjalankan / Deploy

- Lokal: buka `index.html` langsung di browser.
- Hosting gratis: GitHub Pages (Settings → Pages → pilih branch `main`), Netlify, atau Vercel.

## Lisensi

[MIT](LICENSE)

## Catatan

Hasil perhitungan mengikuti tradisi Jawa dan bersifat budaya — sarana doa bersama untuk almarhum, bukan ramalan.
