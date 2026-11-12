# NusantaraCode – Public Marketing Website

Situs statis informasional NusantaraCode. Dibangun tanpa build tool atau koneksi backend saat halaman dibuka.

## Struktur
- `index.html`: profil singkat, bidang solusi, panduan
- `panduan-memilih-api.html`, `mengelola-kuota-api.html`, `keamanan-integrasi-api.html`: materi edukasi
- `privacy.html`, `terms.html`: informasi dan kebijakan situs
- `assets/styles.css`: gaya responsif lokal
- `ads.txt`: identitas penjual iklan (dipertahankan)
- `sitemap.xml`, `robots.txt`: petunjuk mesin pencari

## Keamanan komersial
Jangan pernah menambahkan endpoint produksi, host backend internal, header autentikasi, token, data respons aktual, kredensial pelanggan, atau playground publik pada situs ini. Materi teknis bersifat konsep, tanpa jalur akses produk. Kredensial, kuota, pembatasan permintaan, dan kontrol penagihan adalah tanggung jawab layanan API sebenarnya dan **tidak** disediakan oleh situs statis ini.

## Checklist manual sebelum dipublikasi
- Periksa klaim produk terhadap layanan yang benar-benar dijual; hapus yang tidak relevan.
- Verifikasi kanal kontak bisnis resmi (belum tersedia di repository; **jangan mengarang** email/telepon).
- Periksa kebijakan privasi dan ketentuan dengan pengelola sebelum berlaku.
- Uji navigasi, responsivitas, dan sitemap; pastikan tidak ada kebocoran host, route, dan data produksi.
- Periksa ulang Kebijakan Program AdSense; keberadaan artikel dan kebijakan tidak menjamin persetujuan.

## Uji lokal
```sh
python3 -m http.server 8080
```
Buka `http://localhost:8080`. Tidak ada runtime API maupun permintaan ke backend bisnis.
