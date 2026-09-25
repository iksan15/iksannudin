# Portofolio — Muhammad Iksannudin

Website portofolio statis (HTML/CSS murni, tanpa build tools) berdasarkan CV Muhammad Iksannudin.

## Struktur folder
```
portfolio-muhammad-iksannudin/
├── index.html        # halaman utama (semua CSS ada di dalamnya)
├── assets/
│   └── profile.png   # foto profil (diekstrak dari CV)
└── README.md
```

## Cara upload ke GitHub Pages

1. Buat repository baru di GitHub, misalnya `iksannudin-portfolio`.
2. Upload seluruh isi folder ini (index.html, folder assets, README.md) ke repository tersebut.
   - Lewat web: buka repo → **Add file → Upload files** → seret semua file/folder di atas → Commit.
   - Lewat terminal:
     ```bash
     cd portfolio-muhammad-iksannudin
     git init
     git add .
     git commit -m "Initial portfolio site"
     git branch -M main
     git remote add origin https://github.com/USERNAME/iksannudin-portfolio.git
     git push -u origin main
     ```
3. Di repo GitHub, buka **Settings → Pages**.
4. Pada **Source**, pilih branch `main` dan folder `/ (root)`, lalu **Save**.
5. Tunggu 1–2 menit, situs akan aktif di:
   `https://USERNAME.github.io/iksannudin-portfolio/`

## Mengedit konten

Semua teks (pengalaman kerja, skill, pendidikan, kontak) ada langsung di `index.html` dalam Bahasa Indonesia — cari bagian yang ingin diubah dan edit teksnya langsung, tidak perlu tools tambahan.

Untuk mengganti foto profil, timpa file `assets/profile.png` dengan foto baru (pertahankan nama file yang sama, atau ubah path `src` di `index.html` pada bagian `<div class="photo-frame">`).
