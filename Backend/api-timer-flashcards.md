# Mengenal API, timer, dan spaced repetition

Catatan belajar yang disiapkan dengan bantuan OpenAI Codex untuk dipelajari pemilik repository; bukan klaim bahwa materi sudah dikuasai.

## API contract
[API Contract Test Kit](https://github.com/ZidaneNaufal1/api-contract-test-kit) memeriksa apakah respons HTTP sesuai harapan: status, header, dan beberapa tipe properti JSON. Contoh: endpoint kesehatan diharapkan mengembalikan status 200 dan properti `ok` bertipe boolean. Jika hasil berbeda, library melaporkan bagian yang tidak cocok. Versi ini hanya GET dan memakai subset schema, bukan validator OpenAPI penuh.

## Timer fokus
[Ruang Fokus](https://github.com/ZidaneNaufal1/accessible-pomodoro-web) menyimpan waktu akhir sesi, sehingga hitungan dapat diperbarui berdasarkan jam saat halaman kembali aktif. Saat dijeda, aplikasi menyimpan sisa waktu. Data berada di browser; menghapus data browser dapat menghilangkan riwayat.

## Kartu pengulangan
[Recall Notes](https://github.com/ZidaneNaufal1/flashcard-spaced-repetition) menjadwalkan kartu berdasarkan penilaian Again, Good, atau Easy. Tanggal menggunakan UTC dan rumusnya sederhana, bukan metode yang sudah dibuktikan secara ilmiah. Backup JSON membantu menyimpan salinan, tetapi import mengganti deck setelah konfirmasi.

## Pertanyaan latihan
1. Apa yang terjadi jika status HTTP benar tetapi tipe JSON salah?
2. Mengapa menyimpan deadline dapat membantu ketika tab tidak aktif?
3. Apa perbedaan Again dan Good dalam penjadwalan kartu?
