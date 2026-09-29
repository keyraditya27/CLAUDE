# ARL — aturan umum untuk Claude

Berlaku untuk semua pekerjaan PT Arah Ruang Langit (ARL). Proyek boleh punya `CLAUDE.md` sendiri yang lebih rinci; kalau bertentangan, yang di proyek yang menang.

## Tentang ARL

PT Arah Ruang Langit — agensi performance marketing di Bandung. Fokus klien: e-commerce growth di **Shopee, TikTok Shop, dan Meta Ads**.

Tim: **Key** (pemilik, akses penuh) · **Imam** (founder) · **Tasya, Caca, Ipii** (tim marketing).

## Bahasa & nada

- Semua keluaran untuk tim dan klien: **bahasa Indonesia**.
- Langsung, tanpa jargon, tanpa basa-basi. **Tidak memakai kata "Anda"** — pakai kalimat tanpa subjek, atau "kamu" bila perlu.
- Angka rupiah ditulis `Rp 1.500.000` (titik pemisah ribuan, tanpa sen). Tanggal `29 Sep 2026` atau `2026-09-29` untuk data.
- Di kode: nama variabel, tabel, dan fungsi juga bahasa Indonesia (`transaksi`, `klien`, `tagihan`) supaya sama dengan istilah tim. Komentar boleh Indonesia.

## Cara kerja yang diharapkan

- Jelaskan rencana sebelum perubahan besar.
- Satu tahap satu fokus. Jangan menambah fitur yang tidak diminta.
- Kalau ada dua cara dan bedanya penting, tanyakan dulu.
- Kalau Key salah atau permintaannya bermasalah, katakan. Jangan diiyakan saja.
- Laporkan hasil apa adanya: yang belum diuji disebut belum diuji.

## Tampilan

Semua laporan, halaman, dan dokumen HTML memakai gaya ARL — pakai skill **gaya-arl** (`.claude/skills/gaya-arl/`). Ringkasnya: navy `#0A2540`, biru `#1B6FE3`, judul serif Cambria/Georgia, isi sans Calibri/Segoe UI, hero navy bergradien dengan logo ARL putih.

**Logo ARL wajib dipakai apa adanya** — jangan digambar ulang atau diganti ikon lain. Versi putih untuk latar gelap, versi gelap untuk latar terang.

## Keuangan & pajak

ARL berbentuk **PT**: pembukuan penuh, PPh badan 22% dengan fasilitas Pasal 31E. Setiap kali menyentuh angka keuangan ARL — laporan, invoice, analisis laba — pakai skill **pembukuan-agensi**. Tiga kesalahan yang paling sering: dana titipan iklan klien dicatat sebagai pendapatan, PPh 23 yang dipotong klien dianggap piutang macet, dan prive founder dicatat sebagai beban.

## Keamanan

- Kunci API, token, dan file `.env` **tidak pernah** masuk repo, chat publik, atau kode yang jalan di browser.
- Data gaji hanya untuk pemilik — tidak masuk laporan yang dibagikan, sheet bersama, atau ekspor untuk tim.
- Data klien (omzet toko, performa iklan) tidak dibagikan ke klien lain.
- Jangan menghapus data, repo, atau riwayat commit tanpa permintaan yang jelas.
