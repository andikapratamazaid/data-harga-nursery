# Data Harga Bibit & Input Nursery — Cikopo

Dataset terbuka berisi patokan harga bibit durian dan input nursery untuk
keperluan costing proyek Nursery Durian Cikopo, lengkap dengan dashboard
tampilan di `index.html`.

## Isi Repository

- `data/harga_bibit_durian.csv` — harga bibit durian (Black Thorn sambung
  pucuk, lokal dari biji) dari riset pasar, asumsi RAB, dan asumsi model HPP.
- `data/harga_input_nursery.csv` — harga input: kohe kambing, dolomit,
  NPK 15-15-15 +TE, dan pipa HDPE dari riset marketplace dan quotation vendor.
- `index.html` — dashboard statis yang menampilkan kedua dataset sebagai
  tabel (datanya tertanam di halaman, sama persis dengan isi CSV).

## Kolom Data

`tanggal` (tanggal riset/penawaran), `item`, `jenis` atau `spek`,
`min` dan `max` (rupiah), `satuan`, `jenis_harga`, `sumber`, `catatan`.

## Jenis Harga (penting)

- **Riset pasar / Riset marketplace**: harga listing saat riset (Oktober
  2026). Bukan penawaran resmi; bisa berubah atau hilang.
- **Quotation vendor**: dari surat penawaran tertulis vendor, dengan nomor
  dokumen tercantum di kolom sumber.
- **Estimasi pembanding**: perkiraan dari kelas produk yang sama, dipakai
  hanya bila harga resmi tidak dipajang publik.
- **Asumsi RAB / Asumsi model**: angka perencanaan internal, bukan harga pasar.

Selalu minta quotation terbaru sebelum memakai angka ini untuk keputusan
pembelian.

## Cara Memperbarui

Tambahkan baris baru di file CSV dengan tanggal riset terbaru (jangan menimpa
baris lama, supaya riwayat harga terlihat), lalu sesuaikan data tertanam di
`index.html` agar dashboard tetap sama dengan CSV.

## Sumber

Riset pasar Oktober 2026 untuk proyek Nursery Durian Cikopo (dokumen proyek
Durian Farm Cikopo; listing Tokopedia/Shopee tanggal 22–23 Oktober 2026) dan
quotation PT Solusi Inti Bersama (27 Oktober 2026) serta CV Panca Wira
Wisesa (27 Oktober 2026).
