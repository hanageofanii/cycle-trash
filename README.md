Berikut adalah langkah-langkah untuk menginstall aplikasi ini:

1. Pastikan bahwa anda sudah menginstall Laravel Versi 8 di perangkat anda
2. Clone repository ini lalu masuk ke folder project cycle-trash
3. Buka terminal atau command line anda, lalu masukkan perintah
    composer install
    npm install
4. Setelah menginstall dependensi yang dibutuhkan, copy file .env.example ke file .env pada root folder project
5. Buka file .env lalu sesuaikan konfigurasi database anda sebagai berikut
    DB_DATABASE=****
    // sesuaikan sendiri username dan password database anda
6. Masukkan perintah php artisan key:generate ke terminal anda
7. Masukkan perintah composer dump-autoload
8. Buka file vendor/crocodicstudio/crudbooster/src/database/seeds/CBSeeder.php lalu masukkan kode berikut pada baris pertama setelah tag php:
    namespace Database\Seeders;
9. Install dependensi CrudBooster dengan memasukkan perintah
   php artisan crudbooster:install
10. Setelah dependesi CrudBooster terinstall, hapus database cycle-trash dan buat lagi dengan nama yang sama tanpa menambahkan tabel apapun ke dalam database

11. Impor file database cycle-trash.sql yang telah kami sediakan ke database yang baru saja anda buat

12.. Jalankan perintah php artisan serve

13. Buka link http://localhost:8000/. Jika tampilan web sudah terlihat maka anda sudah berhasil menginstall aplikasi cycle-trash!
