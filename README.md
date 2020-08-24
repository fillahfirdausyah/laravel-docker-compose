# laravel-docker-compose

Alur kerja Docker Compose yang cukup sederhana yang menyiapkan jaringan LEMP (Linux, Nginx, Mysql, PHP) container untuk pengembangan Laravel lokal.


## Penggunaan

Untuk memulai, pastikan Anda memiliki [Docker terinstal] (https://docs.docker.com) di sistem Anda, lalu klon repositori ini.

Selanjutnya, navigasikan di terminal Anda ke direktori tempat Anda mengkloning ini, dan jalankan container untuk server web dengan menjalankan `docker-compose up -d --build`.

Setelah itu selesai, ikuti langkah-langkah dari file [src / README.md] (src / README.md) untuk menambahkan proyek Laravel Anda (atau buat baru yang kosong).

Container akan berjalan di PORT:

- **nginx** - `:8080`
- **mysql** - `:3306`
- **php** - `:9000`

Untuk mengakses NPM pakai command berikut:

- `docker-compose run --rm npm (command npm)`

Untuk mengakses Container php pakai command berikut:

- `docker exec -it php /bin/bash`

Untuk mengakses Composer pakai command berikut:

-  masuk ke Container php
- `composer (command composer)`

Untuk mengakses Artisan pakai command berikut:

-  masuk ke Container php
- `php artisan (command artisan)`
