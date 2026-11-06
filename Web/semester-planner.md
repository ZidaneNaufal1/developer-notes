# Memahami Ruang Semester

Catatan belajar yang disiapkan dengan bantuan OpenAI Codex. Catatan ini adalah bahan latihan, bukan klaim bahwa materi sudah dikuasai.

## Masalah yang diselesaikan

[Semester Planner](https://github.com/ZidaneNaufal1/semester-planner-web) menyatukan jadwal kuliah mingguan dan tenggat tugas. Data disimpan dalam browser, sehingga tidak memerlukan akun.

## Cara kerja

1. Setiap jadwal memiliki hari serta waktu mulai dan selesai. Bentrok terjadi ketika dua jadwal berada pada hari yang sama dan waktunya saling tumpang tindih. Jadwal yang berakhir tepat saat jadwal lain dimulai tidak bentrok.
2. Tugas memiliki tanggal tenggat, status, dan mata kuliah opsional. Daftar dapat disaring berdasarkan status.
3. Cadangan JSON diperiksa sebelum impor mengganti data. Jika data tidak valid atau ada jadwal bentrok, impor ditolak.

## Batas dan hal yang perlu dipahami

Data lokal dapat hilang saat data browser dibersihkan; ekspor cadangan secara berkala. Belum ada kalender bulanan, fitur edit, akun, sinkronisasi, atau notifikasi. Jadwal mengulang setiap minggu tanpa rentang semester. Jangan menyimpan informasi sensitif karena data tidak dienkripsi.

## Latihan

- Mengapa jadwal 08.00–10.00 dan 10.00–11.00 tidak dianggap bentrok?
- Apa yang terjadi jika file cadangan berisi tanggal yang tidak valid?
- Apa risiko menyimpan data hanya pada satu browser?
