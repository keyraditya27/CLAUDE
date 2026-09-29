# CLAUDE — pusat aturan & skill ARL

Tempat menyimpan aturan dan skill Claude yang dipakai di **semua** pekerjaan PT Arah Ruang Langit, supaya tidak perlu ditulis ulang di tiap proyek.

## Isi

| File | Untuk apa |
|---|---|
| `CLAUDE.md` | Aturan umum: tentang ARL, bahasa & nada, cara kerja, keamanan |
| `.claude/skills/gaya-arl/` | Gaya visual ARL untuk laporan & halaman HTML — warna, huruf, komponen, **logo resmi**, CSS siap salin, dan halaman contoh |
| `.claude/skills/pembukuan-agensi/` | Aturan pembukuan & pajak ARL sebagai PT agensi: dana titipan, PPh 23, prive, koreksi fiskal, penyusutan, kalender pajak |
| `templates/CLAUDE-proyek.md` | Kerangka `CLAUDE.md` untuk proyek baru |

Contoh hasil gaya ARL: buka `.claude/skills/gaya-arl/aset/contoh.html` di browser.

## Cara memakai

**Di Claude Code (komputer sendiri)** — berlaku untuk semua proyek:

```
git clone https://github.com/keyraditya27/CLAUDE.git ~/arl-claude
mkdir -p ~/.claude/skills
cp ~/arl-claude/CLAUDE.md ~/.claude/CLAUDE.md
cp -r ~/arl-claude/.claude/skills/* ~/.claude/skills/
```

Kalau `~/.claude/CLAUDE.md` sudah ada isinya, tempelkan isi file ini di bawahnya — jangan ditimpa.

**Di satu proyek saja** — salin folder skill yang dibutuhkan ke `.claude/skills/` di repo proyek itu, lalu tulis `CLAUDE.md` proyek dari `templates/CLAUDE-proyek.md`.

**Di claude.ai** — skill bisa diunggah lewat Settings → Capabilities → Skills: kompres satu folder skill (mis. `gaya-arl/`) jadi `.zip`, lalu unggah.

## Proyek yang memakai aturan ini

- [`keyraditya27/owner`](https://github.com/keyraditya27/owner) — ARL Keuangan Internal (Next.js + Supabase + PWA). Sumber gaya visual dan aturan pembukuan di repo ini.

## Mengubah aturan

Ubah di sini dulu, lalu salin ulang ke tempat pemakaiannya. Satu sumber, supaya tidak ada dua versi aturan yang saling bertentangan.

Jangan pernah menyimpan kunci API, file `.env`, atau data klien di repo ini.
