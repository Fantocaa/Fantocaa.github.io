# Goravel + Inertia + React

Memulai aplikasi web baru sering berarti membangun fondasi yang sama sebelum menyentuh kebutuhan produk: proses masuk, halaman terlindungi, pengaturan akun, navigasi, dan dasbor. Saya membuat starter kit sumber terbuka ini agar bagian-bagian tersebut sudah bekerja bersama dalam aplikasi Go dan React sejak awal.

## Masalah utamanya

Halaman login saja belum menjadi fondasi aplikasi yang siap digunakan. Server perlu tahu rute mana yang memerlukan sesi, antarmuka perlu menerima data pengguna dan pesan validasi, dan pengguna perlu tempat untuk mengelola akun. Jika bagian-bagian ini disusun terpisah, setiap proyek baru harus menyambungkannya lagi dari awal.

## Cara saya menyelesaikannya

Saya menggunakan Goravel sebagai backend Go dan Inertia untuk menghubungkan respons server ke halaman React dan TypeScript. Starter kit ini mencakup pendaftaran dan proses masuk, perlindungan rute berbasis sesi, pengaturan profil dan kata sandi, serta data autentikasi dan pesan status yang dibagikan ke antarmuka. Ada juga sidebar responsif, pilihan tema, dan contoh dasbor analitik.

Angka pada dasbor merupakan data contoh untuk menunjukkan tampilan, bukan data dari bisnis tertentu.

## Hasil yang dibangun

Pengembang dapat memulai dari aplikasi dengan alur akun dan administrasi yang sudah terhubung, lalu mengganti layar contoh dengan kebutuhan produk mereka sendiri. [Repositori GitHub publik](https://github.com/Fantocaa/goravel-inertia-react) memuat kode sumber, petunjuk pemasangan, dan lisensinya.
