# Progress 1: Simple LMS - Docker & Django Foundation

## Langkah-langkah Menjalankan Project

## 1. Clone Repository

- git clone https://github.com/andikaa17/Simple-LMS---Docker-Django.git

## 2. Menjalankan Docker

- docker-compose up -d --build

c:\Users\loq\OneDrive\Pictures\Screenshots\Cuplikan layar 2026-03-27 001514.png

## 3. Cek Container Berjalan atau belum

- docker ps

c:\Users\loq\OneDrive\Pictures\Screenshots\Cuplikan layar 2026-03-27 001752.png

## 4. Mengakses Aplikasi

Buka browser dan akses: http://localhost:8000

c:\Users\loq\OneDrive\Pictures\Screenshots\Cuplikan layar 2026-03-27 101055.png

## 5. Memberhentikan Project

- docker compose down

# Environment Variables

konfigurasi file .env :
c:\Users\loq\OneDrive\Pictures\Screenshots\Cuplikan layar 2026-03-27 102140.png

Keterangan:

- Debug: Pengaturan untuk mengaktifkan fitur debug pada Django, nilai True menandakan aplikasi sedang berjalan di mode development.
- SECRET_KEY: Kunci rahasia yang digunakan Django untuk menjaga keamanan aplikasi, termasuk pengelolaan session dan perlindungan CSRF.
- ALLOWED_HOSTS: Konfigurasi yang menentukan daftar host atau domain yang diperbolehkan mengakses aplikasi.
- DATABASE_URL: URL konfigurasi koneksi ke database PostgreSQL yang mencakup username & password (postgres), hostname (database), port (5432), dan nama database (lms_db).
- REDIS_URL: URL yang digunakan untuk menghubungkan aplikasi ke server Redis.
