---
title: "Berangkat ke Jakarta: Ngecek Server, Ngecek Otak, Ngecek Logika"
date: 2026-06-07
categories:
  - Life & Tech
tags:
  - jakarta
  - server
  - logical-fallacy
  - engineer-life
  - narasi
author: "Sugeng El Mafioso"
---

## Pagi-Pagi Sudah `ping` 🕐

Jam lima pagi, waktu Jakarta masih setengah sadar. Gue duduk di terminal, jari ngetik tanpa banyak mikir:

```
ping server-jkt.staging.digitalsekuriti.id -c 10
```

Sedangkan di luar layar, realitasnya lebih ribet. Tas ransel udah digendong ☕, kopi masih setengah panas di mug kesayangan, dan hati ini lagi antara *excited* sama grogi — kayak devs pas mau `git push origin main` di hari Jumat sore 😅

Jakarta. Kota yang servernya selalu *unik*. Unik dalam artian: unik *cara dia rusak* 🏙️✨

## Kenapa Harus Pergi Sendiri? 🤔

Banyak yang nanya, "Lu kenapa nggak remote aja? Nggak semua masalah butuh kehadiran fisik." Dan mereka *bener*. Tapi ada sesuatu yang nggak bisa di-*migrate* lewat VPN: **intuisi.**

Bayangin gini — lu lagi debug production server. Logs-nya bersih, CPU idle, memory stabil. Tapi *rasanya* sesuatu salah. Kayak kucing yang dengarnya ada tikus di tembok tapi nggak keliatan 🐱🔍 Nah, ketika gue nyampe ke data center di Jakarta, langsung bisa denger suara fan yang agak *ngorok*, lihat lampu status yang kedip-kedip kayak anak TK baru belajar biner, dan merasakan suhu ruangan yang bikin keringat dingin di tengah AC beku ❄️

Itu yang nggak bisa diganti `ssh`. **Keberadaan fisik memberi data yang tidak terstruktur.** Dan seringkali, data tidak terstruktur itu yang paling jujur.

## Logika yang Tersesat di Jalan Raya Jakarta 🚦

Sambil menunggu proses instalasi server selesai — sambil macet di Jl. HR Rasuna Said 👨‍💻 — gue mulai mikir soal *logical fallacies*. Fallacy atau kesesatan logika itu bukan cuma soal debat akademik. Mereka ada di mana-mana. Di media sosial, di rapat perusahaan, bahkan di antara sesama devs pas review code.

Coba gue bahas satu per satu, sambil menunggu lampu merah yang sepertinya nggak pernah habis.

### 1. *Post Hoc Ergo Propter Hoc* — "Setelah Ini, Maka Karena Ini" 🔗

Fallacy paling klasik. A terjadi sebelum B, jadi A pasti penyebab B. Sederhana, kan? Tapi sering banget bikin kita salah diagnosa.

**Contoh nyata:**

> "Pas gue *update* server, traffic langsung naik 40%. Berarti *update*-nya berhasil!"

Hmm... atau traffic naik karena memang hari kerja? Atau ada campaign marketing yang jalan? Atau sekadar fluktuasi normal?

Ini kayak waktu tetangga bilang, "Dulu bapak saya merokok seumur hidup, nggak pernah sakit. Terus anak-anaknya malah kanker semua karena rokok." — Ya, itu *correlation* bukan *causation*, Om 🚬

**Analogi:**
Lu minum obat flu. Esok hari lu sembuh. Apakah obatnya yang bikin sembuh? Atau tubuhlu memang udah siap pulih? Fallacy ini muncul karena kita terlalu cepat menghubungkan waktu dengan sebab.

### 2. *Slippery Slope* — "Jalan Licin yang Nggak Ada Habisnya" 🎢

"Kalau kita ubah tech stack, nanti seluruh tim akan bingung. Kalau semua orang bingung, produktivitas turun. Kalau produktivitas turun, company merger. Kalau merger, semua di-*downsizing*."

Wkwk. Santai lah. *Slippery slope* itu seperti cerita yang makin lama makin ke akar pohon — dan kadang benar, tapi sering juga *overreaction*.

**Contoh di dunia engineering:**

> "Kalau kita pake JavaScript lagi, nanti kita balik ke masa ketika semua kode berantakan seperti jalanan Jakarta pas hujan turun."

Bener nggak bener? Hmm... tergantung pada siapa lu tanya. Tapi intinya, *slippery slope* itu membuat satu perubahan kecil terlihat seperti domino yang bakal menjatuhkan semuanya 💥

### 3. *Ad Hominem* — "Serang Seseorang, Bukan Argumennya" 🎯

Ini fallacy favorit para politisi dan code reviewer.

> "Lu bilang microservices lebih baik? Lu aja nggak pernah bikin arsitektur yang scalable. Jadi apa sih alasanmu?"

**BINGO.** Itu *ad hominem*. Dia menyerang orangnya, bukan argumennya. Ya, mungkin lu belum pernah bikin arsitektur besar-besaran, tapi itu nggak berarti argumenlu salah. Bisa aja lu benar justru karena lu belajar dari kegagalan orang lain.

Analogi yang paling jelas: ketika lu nasehati temanmu buat berhenti merokok, terus dia bilang, "Omong lu doang! Lu aja masih sering begadang." — Ya, mungkin gue begadang, tapi nasehatnya tetap valid ☕

### 4. *Straw Man* — "Menyembunyikan Pohon di Balik Rumput" 🌾

*Lu membuat argumen palsu (seperti orang-orangan sawah) yang lebih mudah dijatuhkan, lalu lu jatuhkan argumen aslinya secara tidak sadar.*

**Contoh:**

> Teman: "Mungkin kita nggak perlu meeting setiap hari. Cukup dua kali seminggu."
> Lu: "Jadi lo mau kita nggak komunikasi sama sekali? Nanti semua tim kerja sendiri-sendiri!"

Teman cuma bilang *kurangi* meeting, bukan *hapus* total. Tapi lu langsung bikin versi ekstrem dari argumennya — kayak bikin orang-orangan sawah yang bisa diam dan kemudian menepuk dada, "Lihat, gue berhasil mengalahkan dia!" 🧑‍🌾

### 5. *Appeal to Authority* — "Karena Kata Beliau, Maka Benar" 👑

"Si CTO udah bilang microservices adalah masa depan. Jadi pasti baik."

Tidak salah. Tapi nggak selalu benar juga. *Appeal to authority* itu kayak ketika kita menganggap sesuatu benar hanya karena yang mengatakannya adalah *orang yang penting*. Padahal, otoritas di satu domain nggak otomatis membuat mereka benar di semua domain.

**Analogi:**
Ketika seorang chef terkenal bilang, "Lu harus minum air putih delapan gelas sehari," — dia bukan dokter. Tapi lu tetap percaya? Ya, karena dia *chef ternama*. Itu power of authority, baik dan buruknya bersama-sama 👨‍🍳

### 6. *False Dilemma* — "Hanya Dua Pilihan, Padahal Banyak Jalan" 🛤️

"Lu mau pakai cloud atau on-premise. Pilih satu!"

Seolah-olah nggak ada *hybrid*. Seolah-olah dunia ini cuma punya dua pilihan dan satu lagi pasti salah.

**Contoh sehari-hari:**

> "Either lu kerja full-time di kantor, atau lu pengangguran yang living off savings."

Padahal, masih ada remote work, freelance, side hustle, dan segudang cara untuk tetap makan sambil nggak duduk di kursi kantor setiap hari 💻

## Server dan Logika: Dua Dunia yang Bertemu ⚙️

Sambil menunggu server baru selesai dikonfigurasi — satu per satu *rack* hidup seperti kota yang bangkit dari tidur — gue memikirkan bahwa **debugging server itu mirip debugging logika kita sehari-hari.**

Kadang kita salah diagnosa karena:
- Terburu-buru mengambil kesimpulan (*post hoc*) 🏃
- Melihat terlalu banyak konsekuensi (*slippery slope*) 🌊
- Menyerang penyebab, bukan masalah (*ad hominem*) 👤
- Membuat straw man dari argumen yang sebenarnya valid 🧱
- Terlalu mempercayai otoritas 👑
- Menganggap hitam-putih padahal kelabu ⚫⚪

Dan seringkali, solusinya sama: **berhenti sejenak. Napas. Amati. Jangan buru-buru klik `deploy`.** ⏸️

## Sesampainya di Tujuan 🎯

Akhirnya, server itu berjalan. Dengan tenang. Tanpa bunyi *ngorok* yang mengganggu. Semua lampu hijau menyala seperti bintang-bintang kecil di langit Jakarta yang kadang bisa dilihat dari jendela data center ✨

Gue duduk di kursi roda kantor sambil menatap layar. Di luar, jalanan Jakarta tetap macet. Orang-orang tetap berdebat tentang hal-hal yang seharusnya nggak perlu diperdebatkan. Dan gue tersenyum — karena hari ini, selain server yang berjalan baik, otak gue juga ikut terbangun 🧠💡

## Penutup: Jadilah Detective Logika 🔎

Nanti kali lu lagi debat di chat grup, atau saat meeting, atau bahkan pas review code temanmu — coba tanya:

> *"Apakah argumen ini benar, atau hanya terdengar benar?"

Karena pada akhirnya, server yang baik bukan cuma soal hardware dan uptime. Server yang baik juga punya *logika* yang jelas: *why it works, how it scales*, dan *what happens when it breaks*. 💪

Dan begitu juga dengan kita.

---

*Gimana? Pernah nggak lu ketahuan fallacy pas lagi debat atau coding? Share di komentar ya! 👇✨*
