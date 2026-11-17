# Platform Acara Multi-Tenant

Operator platform melayani beberapa penyelenggara acara. Masing-masing penyelenggara membutuhkan tempat untuk mengelola acara dan tamunya, sementara operator perlu membuat dan mengatur ruang kerja yang terpisah. Jika dua tanggung jawab itu dicampur dalam satu ruang data, kepemilikan tiap catatan menjadi sulit dibedakan.

## Masalah utamanya

Tantangannya adalah memisahkan pekerjaan operator platform dari pekerjaan harian penyelenggara. Saat organisasi baru bergabung, mereka membutuhkan ruang kerja yang siap dipakai, bukan sekadar akun. Setelah itu, setiap permintaan aplikasi harus masuk ke data organisasi yang tepat.

## Cara saya menyelesaikannya

Saya memisahkan data pusat untuk organisasi dan akses dari data acara serta tamu milik tiap organisasi. Subdomain menentukan konteks penyelenggara, lalu basis data PostgreSQL tersendiri menyimpan data operasionalnya. Proses pembuatan organisasi juga menyiapkan basis data, migrasi, serta peran dan menu awal agar ruang kerja langsung dapat digunakan.

Laravel menangani proses penyiapan organisasi dan permintaan aplikasi; React dan Inertia menyajikan antarmukanya. Redis mendukung sesi, cache, dan pekerjaan antrean. Semua itu mengikuti keputusan yang sama: administrasi platform terpusat, pekerjaan tiap penyelenggara terpisah.

## Hasil yang dibangun

Operator dapat mengelola organisasi tanpa mencampur data acaranya ke ruang administrasi bersama. Setiap penyelenggara bekerja dengan acara dan tamu miliknya melalui subdomain sendiri.

Ini proyek privat. Data klien, konfigurasi internal, dan kode sumber tidak dipublikasikan di sini. [Diskusikan proyek serupa](mailto:fantocaa17@gmail.com).
