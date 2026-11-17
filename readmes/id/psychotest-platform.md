# Platform Psikotes Rekrutmen

Tim rekrutmen perlu mengundang pelamar mengikuti tes dan kemudian meninjau hasilnya. Pelamar membutuhkan alur tes yang jelas, sedangkan orang yang mengelola soal dan laporan membutuhkan ruang kerja terlindungi. Keduanya berada dalam proses yang sama, tetapi tidak semestinya memiliki akses yang sama.

## Masalah utamanya

Mengirim tautan tes baru menyelesaikan langkah undangan. Soal masih perlu dikelompokkan, pelamar perlu melewati tiap bagian tes, dan hasilnya harus kembali dalam bentuk yang dapat ditinjau perekrut atau dibagikan kepada pihak yang berwenang.

## Cara saya menyelesaikannya

Saya membangun alur admin untuk membuat tautan tes per pelamar, mengelola soal dan bagian tes, serta meninjau data pengerjaan. Pelamar memakai tautan publik untuk memulai bagian tes dan mengirim jawaban tanpa masuk ke ruang admin. Hasilnya tersedia sebagai laporan terperinci dan laporan keterampilan, dapat diakses melalui tautan laporan yang dikendalikan serta diekspor ke PDF.

Backend Laravel menghubungkan tes, pengiriman jawaban, dan pembuatan laporan. React, TypeScript, dan Inertia menyajikan antarmuka bagi kedua pihak. Peran, izin, dan catatan audit mendukung pekerjaan admin yang dilindungi.

## Hasil yang dibangun

Perekrut memiliki alur dari menyiapkan asesmen hingga membaca hasilnya. Pelamar mendapat jalur pengerjaan terpisah sehingga tidak perlu memasuki area administrasi.

Ini proyek privat `module-psychotest`. Data pelamar, materi tes, dan kode sumber tidak dipublikasikan di sini. [Diskusikan proyek serupa](mailto:fantocaa17@gmail.com).
