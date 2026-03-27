# Progress 1: Simple LMS - Docker & Django Foundation

## Langkah-langkah Menjalankan Project

## 1. Clone Repository

- git clone https://github.com/andikaa17/Simple-LMS---Docker-Django.git

## 2. Menjalankan Docker

- docker-compose up -d --build
  
<img width="1904" height="759" alt="Cuplikan layar 2026-03-27 001514" src="https://github.com/user-attachments/assets/ae800433-db06-4967-b484-e7aedf9cc066" />


## 3. Cek Container Berjalan atau belum

- docker ps
  
<img width="1884" height="297" alt="Cuplikan layar 2026-03-27 001752" src="https://github.com/user-attachments/assets/76587563-bf0d-45ca-aa2e-3010ff6d1aa9" />


## 4. Mengakses Aplikasi

Buka browser dan akses: http://localhost:8000

<img width="1918" height="1037" alt="Cuplikan layar 2026-03-27 101055" src="https://github.com/user-attachments/assets/921e00e6-ab16-4baa-8bbe-52214b3d182a" />


## 5. Memberhentikan Project

- docker compose down

<img width="1906" height="197" alt="Cuplikan layar 2026-03-27 001944" src="https://github.com/user-attachments/assets/a705abd3-a16b-4273-96af-44a3adbd7d70" />


# Environment Variables

konfigurasi file .env :

<img width="942" height="152" alt="Cuplikan layar 2026-03-27 102140" src="https://github.com/user-attachments/assets/6d69b42e-3068-468b-bf34-ede590bf5494" />

Keterangan:

- Debug: Pengaturan untuk mengaktifkan fitur debug pada Django, nilai True menandakan aplikasi sedang berjalan di mode development.
- SECRET_KEY: Kunci rahasia yang digunakan Django untuk menjaga keamanan aplikasi, termasuk pengelolaan session dan perlindungan CSRF.
- ALLOWED_HOSTS: Konfigurasi yang menentukan daftar host atau domain yang diperbolehkan mengakses aplikasi.
- DATABASE_URL: URL konfigurasi koneksi ke database PostgreSQL yang mencakup username & password (postgres), hostname (database), port (5432), dan nama database (lms_db).
- REDIS_URL: URL yang digunakan untuk menghubungkan aplikasi ke server Redis.
