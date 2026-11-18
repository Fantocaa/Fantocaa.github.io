# Pengelola Jendela React

Ada aplikasi yang menuntut orang membuka beberapa bagian pekerjaan sekaligus: berpindah antar panel, membandingkan informasi, lalu kembali ke susunan layar yang sudah mereka atur. Tata letak halaman biasa tidak memberi ruang kerja seperti itu. Komponen sumber terbuka ini memungkinkan aplikasi React menggunakan jendela yang dapat dipindahkan tanpa membangun ulang seluruh perilakunya.

## Masalah utamanya

Menggeser panel hanya salah satu bagiannya. Ukuran jendela perlu batas yang masuk akal, jendela yang bertumpuk perlu urutan yang jelas, dan pengguna perlu melihat posisi tujuan sebelum jendela ditata otomatis. Saat jendela diminimalkan, pekerjaannya harus tetap mudah ditemukan. Semua perilaku itu juga perlu selaras setelah halaman dimuat ulang atau dipakai di layar lebih kecil.

## Cara saya menyelesaikannya

Saya memisahkan perilaku jendela dari isi yang dimasukkan aplikasi ke dalamnya. Komponen ini menangani pemindahan dan perubahan ukuran, penataan ke layar penuh, setengah, atau seperempat layar, serta pratinjau sebelum jendela ditempatkan. Jendela yang diminimalkan masuk ke dock yang bisa diurutkan. Aksi papan ketik dan gestur geser di ponsel memberi cara pengoperasian lain, sementara penyimpanan lokal mempertahankan susunan ruang kerja.

React dan Zustand mendukung komponen serta keadaan ruang kerjanya. Nilai utamanya adalah pengalaman mengatur pekerjaan yang bisa dipakai ulang oleh aplikasi lain.

## Hasil yang dibangun

Pengembang dapat memasukkan layar aplikasinya sendiri ke dalam jendela, lalu memberi pengguna ruang kerja yang bisa mereka atur dan buka kembali. [Repositori GitHub publik](https://github.com/Fantocaa/winmgr) memuat komponen dan petunjuk integrasinya.
