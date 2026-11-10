# ubuntu-id.github.io

Situs web Komunitas Ubuntu Indonesia, live di https://ubuntu-id.org. Hugo + tema `themes/ubuntukr` (Vanilla Framework, turunan situs ubuntu-kr). Branch default `main`. Remote: `ubuntu-id/ubuntu-id.github.io`.

## Stack

- Hugo extended **0.147.9** dan Dart Sass **1.89.2**, dipin di `.github/workflows/hugo.yml`. Pakai versi yang sama secara lokal.
- Tema memakai `css.Sass` (bukan `resources.ToCSS`, sudah dihapus di Hugo 0.128) dengan transpiler `dartsass`, jadi binary `sass` harus ada di `PATH`. Paket npm `sass` tidak cocok dengan Hugo.
- Dependensi tema: `vanilla-framework` 3.4.0 lewat `themes/ubuntukr/package-lock.json`. `npm ci` di `themes/ubuntukr` dulu sebelum build. Naik ke 4.x mengubah nama kelas CSS, jadi cek tampilan sebelum menerimanya.
- Dua bahasa: Indonesia (default, di `/`) dan Inggris (di `/en/`). Tiap halaman punya `index.md` dan `index.en.md`.

## Build dan tes

```bash
cd themes/ubuntukr && npm ci && cd ../..
hugo --minify -d /tmp/out     # harus selesai tanpa ERROR
```

Sekitar 590 peringatan deprecation Dart Sass dari `vanilla-framework` itu normal. Cek hasil build, bukan hanya exit code:

- tiap `<img src>` lokal harus menunjuk berkas yang ada di output (termasuk di `/en/`);
- `404.html` dan `en/404.html` terbit;
- tidak ada link ke host mati (lihat bawah).

CI (`hugo.yml`): push ke `main` build + deploy ke branch `gh-pages` lewat `peaceiris/actions-gh-pages`; pull request hanya build (check bernama `deploy`). Unduhan Hugo dari github.com kadang gagal (`wget` exit 4): rerun job-nya.

## Konvensi

- Ubah halaman di kedua bahasa. Berkas `*.en.md` harus berbahasa Inggris, bukan sisa Korea dari template ubuntu-kr.
- Gambar halaman dirujuk lewat `image:` di front matter dan diambil dengan `.Resources.Get` di template. Jangan menyusun URL dengan `{{ .RelPermalink }}{{ .Params.image }}`: itu rusak di `/en/` dan untuk halaman tanpa `image`.
- Di dalam `{{ with }}`, `.` berubah. Simpan nilai yang masih dipakai (mis. `{{ $title := .Title }}`) sebelum `with`.
- Judul halaman, deskripsi, canonical, `hreflang`, dan Open Graph dibuat di `themes/ubuntukr/layouts/partials/head.html`. Halaman 404 sengaja `noindex`.
- Link mirror ISO di halaman Unduh hanya untuk mirror yang jalur ISO-nya terbukti ada dan memuat rilis terbaru. Status "Up to date" di Launchpad menilai arsip paket, bukan ISO, jadi buka direktorinya.
- Versi Ubuntu di halaman Unduh (`ubuntuVersions` di front matter `content/download/`) perlu diperbarui tiap rilis April dan Oktober. Catatan rilis ada di `documentation.ubuntu.com/release-notes/<versi>/`.

## Link yang tidak boleh dipakai lagi

`forum.ubuntu-id.org`, `events.ubuntu-id.org`, `event.ubuntu-id.org` (DNS sudah tidak ada), kanal YouTube `user/ubuntuindonesia`, `ubuntulinux.or.id`, dan apa pun ke `ubuntu-kr`. Pengganti yang dipakai: forum ke kategori Discourse Ubuntu Indonesia (`discourse.ubuntu.com/c/community/circles/ubuntu-id/133`), events ke `events.canonical.com`.

## Pengaturan repo

`main` diproteksi: wajib lewat PR dan check `deploy` hijau, force push dan penghapusan diblokir (admin bisa menimpa). Dependabot alerts, security updates, secret scanning, dan push protection aktif. `.github/dependabot.yml` memeriksa GitHub Actions dan npm tema tiap minggu. Branch otomatis dihapus setelah merge.

## Hal yang belum diputuskan

- `gimpscape.org` (halaman sponsor) gagal TLS: belum dipastikan apakah sponsor masih aktif.
- `content/bylaws/akta.pdf` (21,9 MB) sengaja dibiarkan di repo.
- Feed Indico di `events.canonical.com` belum punya kategori Ubuntu Indonesia, jadi daftar event belum bisa ditarik saat build.
