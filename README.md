# Undian reka bentuk Home — PPDK.CH

Folder ini berdiri sendiri (tiada build). Muat naik seluruh folder ke GitHub Pages.

## Kandungan
- `index.html` — pemilih: Varian A – G, paparan Desktop/Telefon, Skrin penuh, butang Undi
- `v/varian_A.html` hingga `v/varian_G.html` — mockup penuh (data simulasi)

## Muat naik ke GitHub Pages
1. Cipta repo baharu (cth. `ppdk-undian-home`), muat naik kandungan folder ini ke akar repo.
2. Settings → Pages → Source: `Deploy from a branch` → `main` / `(root)` → Save.
3. Pautan: `https://<nama-pengguna>.github.io/ppdk-undian-home/`

## Pautan terus ke pilihan
Tambah `#huruf` pada pautan, cth. `…/ppdk-undian-home/#E` membuka Varian E.

## Sambungkan borang undian
Buka `index.html`, cari `const POLL_URL = '';` dan isi pautan borang (Google Forms / Microsoft Forms).
Untuk Google Forms dengan jawapan pra-isi, letak `{pilihan}` di tempat nilai:

    const POLL_URL = 'https://docs.google.com/forms/d/e/XXXX/viewform?usp=pp_url&entry.123456={pilihan}';

Jika dibiarkan kosong, butang "Hantar undian" menyalin pilihan pengundi ke papan keratan untuk ditampal ke WhatsApp/emel.

## Nota
- Repo GitHub Pages percuma adalah **awam**. Mockup ini guna data simulasi; nama & koordinat sekolah adalah maklumat awam. Tiada nama pegawai, kata laluan atau kunci API.
- `noindex` ditetapkan supaya enjin carian tidak mengindeks halaman.
- Fon dimuat dari Google Fonts (perlu internet).
