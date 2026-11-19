# High Res - versi Jekyll

Tukaran tema Tumblr "High Res" v1.2 (Justin Ouellette, 4 May 2015) kepada tapak Jekyll.

## Guna
```
bundle install
bundle exec jekyll serve
```
Buka http://localhost:4000

## Tetapan
Semua pilihan "Customize" Tumblr ada dalam `_config.yml` di bawah `highres:`.
Pautan halaman di atas tajuk diatur melalui `nav:`.

## Jenis post
Letak fail di `_posts/YYYY-MM-DD-nama.md` dan tetapkan `post_type`:

| post_type | Front matter |
|---|---|
| text (lalai) | `title` (pilihan) + isi |
| photo | `photo`, `photo_alt`, `photo_link` (pilihan) + isi sebagai kapsyen |
| photoset | `photos:` (senarai) + isi sebagai kapsyen |
| link | `title`, `link_url` + isi |
| quote | `quote`, `source` |
| chat | `title`, `chat:` (senarai `label`/`line`) |
| video | `video` (kod embed iframe) + isi |
| audio | `audio`, `album_art` + isi |
| answer | `asker`, `asker_avatar`, `question` + isi sebagai jawapan |

Tag: `tags: [satu, dua]`, pautan ke halaman `/tags/`.

## Yang tidak dibawa dari Tumblr
- Infinite scroll, nombor note, post notes, ikon "following", pautan ask/submit (bergantung pada platform Tumblr)
- Google Analytics lama (ga.js) diganti gtag GA4: isi `google_analytics: G-XXXX`
