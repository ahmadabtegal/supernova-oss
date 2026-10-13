# Monitoring Perizinan Berusaha OSS — DPMPTSP Kota Tegal

Paket frontend untuk hosting melalui GitHub Pages. Logo dan favicon sudah dipisahkan dari HTML ke folder `assets/`.

## Struktur berkas

```text
monitoring-oss-github-pages/
├── index.html
├── README.md
└── assets/
    ├── favicon.png
    ├── logo-kota-tegal.png
    ├── logo-dpmptsp.png
    └── logo-oss.png
```

## Penyesuaian logo

Ketiga logo di bagian header memakai tinggi tampilan yang sama (64 px pada desktop dan 52 px pada layar kecil). Lebar menyesuaikan rasio gambar agar logo tidak terdistorsi. Untuk mengubah ukuran, sesuaikan aturan `.logos img` pada CSS di `index.html`.

## Hosting di GitHub Pages

1. Unduh ZIP paket ini lalu ekstrak.
2. Unggah `index.html`, `README.md`, dan folder `assets/` ke root repository GitHub.
3. Buka **Settings → Pages** pada repository.
4. Pada **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/(root)`, lalu klik **Save**.
6. Buka URL GitHub Pages yang ditampilkan setelah proses deployment selesai.

## Catatan backend

GitHub Pages hanya menghosting frontend statis. Fitur pemuatan dan perubahan data tetap memerlukan endpoint backend/API yang dikonfigurasi di HTML (misalnya Google Apps Script yang telah di-deploy sebagai Web App). Pastikan URL endpoint dan izin aksesnya sesuai sebelum digunakan.

## Aset gambar

- `assets/logo-kota-tegal.png`: lambang Kota Tegal.
- `assets/logo-dpmptsp.png`: logo DPMPTSP.
- `assets/logo-oss.png`: logo OSS/Kementerian Investasi/BKPM.
- `assets/favicon.png`: ikon tab browser.
