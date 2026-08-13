# Kelas Ngajiku

Landing page statis untuk `kelasngajiku.com`.

## Deploy ke Easypanel dari GitHub

1. Push project ini ke repository GitHub.
2. Buat app baru di Easypanel.
3. Pilih source dari Git repository.
4. Pilih build menggunakan Dockerfile.
5. Set domain ke `kelasngajiku.com`.
6. Deploy.

File yang perlu ada di repository:

- `index.html`
- `assets/`
- `Dockerfile`
- `nginx.conf`
- `robots.txt`
- `.dockerignore`
- `README.md`

Container berjalan di port internal `80`. Jika Easypanel meminta port aplikasi, isi `80`.

Jika sebelumnya pernah membuat redirect manual di menu Redirects, hapus rule yang mengarah ke `/index.html` atau dari `/index.html` ke `/`, lalu deploy ulang.

Konfigurasi Nginx sudah mengarahkan akses `/index.html` kembali ke `/`, jadi URL publik tetap bersih di root domain.

## Deploy manual

1. Buat app baru di Easypanel.
2. Upload project ini.
3. Pilih build menggunakan Dockerfile.
4. Set domain ke `kelasngajiku.com`.
5. Deploy.
