
# Admin Finder Tool

![ASCII Art Header](https://via.placeholder.com/728x90?text=Admin+Finder+Tool)

Admin Finder adalah alat sederhana berbasis Bash untuk menemukan halaman admin dari suatu situs web dengan melakukan pemindaian terhadap path yang umum digunakan. Skrip ini dilengkapi dengan tampilan warna-warni untuk memberikan pengalaman pengguna yang lebih menarik.

## Fitur
- **Pencarian Path Admin**: Memindai berbagai path admin panel yang umum.
- **Indikasi Warna**: Menampilkan hasil dengan warna yang berbeda:
  - **Hijau**: Path ditemukan (status HTTP 200).
  - **Biru**: Path ditemukan tetapi akses terlarang (status HTTP 403).
  - **Merah**: Path tidak ditemukan.
- **Header Keren**: Tampil dengan header ASCII art yang menarik.

## Instalasi
1. Unduh skrip dengan perintah berikut:
   ```bash
   curl -O https://example.com/admin_finder.sh
   ```
2. Berikan izin eksekusi pada skrip:
   ```bash
   chmod +x admin_finder.sh
   ```

## Penggunaan
1. Jalankan skrip:
   ```bash
   ./admin_finder.sh
   ```
2. Masukkan URL target (contoh: `http://example.com`).
3. Skrip akan memindai dan menampilkan hasil dari path admin yang ditemukan.

## Contoh Output
```plaintext
 █████╗ ██████╗ ███╗   ███╗██╗███╗   ██╗      ███████╗██╗██████╗ ███████╗
██╔══██╗██╔══██╗████╗ ████║██║████╗  ██║      ██╔════╝██║██╔══██╗██╔════╝
███████║██║  ██║██╔████╔██║██║██╔██╗ ██║█████╗███████╗██║██████╔╝█████╗  
██╔══██║██║  ██║██║╚██╔╝██║██║██║╚██╗██║╚════╝╚════██║██║██╔═══╝ ██╔══╝  
██║  ██║██████╔╝██║ ╚═╝ ██║██║██║ ╚████║      ███████║██║██║     ███████╗
╚═╝  ╚═╝╚═════╝ ╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝      ╚══════╝╚═╝╚═╝     ╚══════╝
      Admin Finder Tool by TuguPhantom
=======================================================================
Masukkan URL target (contoh: http://example.com): http://example.com

Scanning for admin panels...
[NOT FOUND] http://example.com/admin
[NOT FOUND] http://example.com/administrator
[FORBIDDEN] http://example.com/login
[FOUND] http://example.com/admin/login
[NOT FOUND] http://example.com/admin/dashboard

Scan selesai!
```

## Catatan
- Pastikan Anda memiliki akses legal untuk memindai situs target.
- Alat ini dirancang untuk tujuan pembelajaran dan pengujian keamanan. Penggunaan ilegal tidak diperkenankan.

## Kontribusi
Kontribusi selalu diterima! Jika Anda memiliki ide untuk meningkatkan skrip ini, jangan ragu untuk membuat **pull request**.

## Lisensi
Skrip ini dirilis di bawah lisensi [MIT License](LICENSE).
