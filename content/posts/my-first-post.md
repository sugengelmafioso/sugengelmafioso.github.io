---
date: 2026-04-07T20:06:45+07:00
title: "Selamat Datang, Dunia! 🌍"
draft: false
tags: ["intro", "hugo", "github-pages", "startups"]
---

Halo teman-teman! 👋

Ini adalah *first post* saya di blog baru yang saya beri nama **Sugeng el Mafioso** — sebuah ruang untuk berbagi pikiran, catatan teknis, dan observasi seputar dunia *tech* dan geopolitik (iya, saya memang suka campur aduk 😄).

## Apa yang Baru?

Kemarin, saya *daringi* (punya *personal domain* sendiri!) dengan:

- **Stack tech**: Hugo + tema `hugo-coder` + GitHub Pages
- **Workflow**: GitHub Actions otomatis build & deploy
- **Content**: Posts, About, Projects, dan halaman statis lainnya

Yang membuat saya * excited* adalah betapa *streamlined*-nya proses setup kali ini. Dalam hitungan jam saja (plus sedikit *debugging* karena versi Go yang *off-by-one*), blog ini sudah *live* dan bisa diakses di `https://sugengelmafioso.github.io`.

## Catatan Kecil dari Proses Setup

Berikut beberapa hal yang *worth sharing* dari proses *migrasi* ini:

### 1. Hugo is Fast (super fast! ⚡)

Kebetulan saya memilih Hugo sebagai *static site generator* karena:

- Satu binary doang — gak perlu instal Node.js/Ruby/Python dulu
- Build waktu *nol point something* detik
- *Theme system* yang keren dan fleksibel

Kalau dulu waktu saya pakai Jekyll, *build* bisa *lag* banget. Nah, dengan Hugo ini *no more waiting*! 🚀

### 2. GitHub Pages + Actions = ❤️

Saya *not a big fan* *manually* push ke FTP atau *commit* ke branch `gh-pages`. Dengan *workflow* GitHub Actions, semua otomatis:

1. Push ke `main` → trigger build
2. Build selesai → deploy otomatis ke Pages
3. *Bonus*: caching untuk asset & CSS/JS

Yang *cool*, saya bisa *track*进展 di *Actions tab* — jadi tahu kapan *deploy* selesai dan apa saja yang *changed*.

### 3. Theme `hugo-coder` — Simple & Clean

Saya pakai `hugo-coder` karena *minimalist* banget — pas banget buat saya yang suka *content over decoration*. Fitur favorit:

- Dark/light mode otomatis (sesuai *system preference*)
- *Social links* yang mudah dikonfigurasi
- *Emoji support* *out of the box* (penting banget buat tone yang *relatable*)

## Sekilas Tentang Nama "el Mafioso"

*Fun fact*: "el Mafioso" itu *ambilan* dari bahasa Spanyol, berarti *"the Mafia man"* atau *"the guy who knows things"*. Tapi di sini, itu lebih ke *nickname* yang *nyelonong* aja — ada unsur *playful* juga sih 😎.

## Next Steps?

Baru mulai, jadi *planning* untuk postingan berikutnya:

- 🌍 Analisis geopolitik (terutama di kawasan Asia-Pacific)
- 🔧 Catatan teknis: AI agents, LLM orchestration
- 📚 *Book notes* dan *takeaways* dari bacaan

Kalau ada hal-hal yang *spesific* yang kamu * curious about*, *feel free* *drop a comment* atau *reach out* via email di `sugeng@digitalsekuriti.id` (iya, saya udah ganti domain — *less personal, more professional*! 🎯).

Sampai jumpa di *next post*! 🙌

— Sugeng
