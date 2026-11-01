# Memahami Job Queue Simulator

Catatan pendamping yang disiapkan dengan bantuan OpenAI Codex untuk dipelajari dan ditinjau pemilik repository. Catatan ini tidak menyatakan bahwa materi sudah dikuasai.

## Masalah yang disimulasikan

Antrean pekerjaan menata urutan tugas. Dalam [job-queue-simulator](https://github.com/ZidaneNaufal1/job-queue-simulator), tugas hanya data contoh: simulator tidak mengirim email atau menjalankan proses sungguhan.

## Konsep inti

- **FIFO:** tugas yang siap lebih dulu diproses lebih dulu; urutan input menjadi pemecah seri.
- **Priority:** tugas dengan prioritas efektif tertinggi dipilih. Nilai bertambah saat menunggu (aging), untuk membantu tugas prioritas rendah mendapat kesempatan.
- **Retry:** kegagalan bisa dicoba lagi setelah jeda. Batas jumlah percobaan mencegah simulasi terus berulang.
- **Dead-letter:** tugas yang tetap gagal setelah batas percobaan ditandai untuk ditinjau.
- **Tick:** satuan waktu simulasi; setiap percobaan memakan satu tick. Tick bukan detik nyata.

## Contoh yang dapat dicoba

Pada salinan proyek, jalankan `npm test` dan `npm run demo`. Skenario contoh menghasilkan dua pekerjaan selesai dan satu dead-letter. Buka `examples/scenario.json`, salin isinya ke file baru, ubah `failures` atau `maxAttempts`, lalu jalankan `node cli.js nama-file.json` untuk membandingkan hasil.

## Pertanyaan latihan

1. Apa perbedaan FIFO dan priority saat dua tugas sama-sama siap?
2. Apa yang terjadi jika `maxAttempts` dikurangi menjadi satu?
3. Mengapa simulasi ini belum cukup menjadi sistem antrean produksi?

Batas penting: hanya satu worker, tidak ada jaringan, penyimpanan permanen, atau jaminan delivery. Aging di sini tidak membuktikan fairness pada sistem terdistribusi nyata.
