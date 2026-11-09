# Catatan belajar: perpustakaan, RSS, aset, dan pencarian

Catatan awal yang disiapkan dengan bantuan OpenAI Codex untuk dipelajari dan diuji ulang oleh pemilik repository. Belum merupakan bukti pemahaman atau pemakaian oleh pengguna lain.

## Empat masalah

- [Library Loan Dashboard](https://github.com/ZidaneNaufal1/library-loan-dashboard): mencatat buku, anggota, pinjaman dan pengembalian dalam SQLite. Transaksi mencegah peminjaman yang melanggar stok. Server contoh hanya untuk komputer lokal dan data sintetis: tidak ada login atau TLS.
- [RSS Reading Inbox](https://github.com/ZidaneNaufal1/rss-reading-inbox): mengumpulkan artikel dari file RSS/Atom yang dipilih, menyaring duplikat dan menyimpan status di browser. Versi awal belum mengambil feed melalui internet.
- [Digital Asset License Catalog](https://github.com/ZidaneNaufal1/digital-asset-license-catalog): mencatat pembuat, sumber, lisensi dan kredit; metadata adalah masukan pengguna, bukan bukti izin penggunaan.
- [Static Docs Search](https://github.com/ZidaneNaufal1/static-docs-search): membuat indeks dari Markdown lalu mencari teks di browser. Indeks memuat kutipan isi sumber sehingga harus diperiksa sebelum dibagikan.

## Latihan menjelaskan

1. Mengapa pemeriksaan stok dan penyimpanan pinjaman perlu dilakukan dalam satu transaksi?
2. Bagaimana mendeteksi artikel yang sama saat dua file feed diimpor?
3. Mengapa nama lisensi pada katalog tidak cukup untuk membuktikan hak pakai?
4. Apa risiko mengunggah indeks yang dibuat dari dokumen pribadi?

Buka README masing-masing proyek untuk menjalankan contoh dan membaca batasan terbaru. Coba dengan data sintetis terlebih dahulu.
