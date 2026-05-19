---
title: 'Tanpa coding. Tanpa harga. Tanpa peta.'
description: 'Course AI yang jualan "tanpa jadi programmer" diam-diam ngajarin lo jadi programmer. Yang bohong bukan curriculum-nya. Marketing-nya. Dan harganya.'
date: 2026-05-19
tags: ['ai', 'marketing', 'voice']
pull: 'Lo dikasih setir. Lo gak dikasih peta.'
excerpt: 'Course AI Rp 950.000 yang jualan "tanpa coding" pake stack senior developer. Tiga produk, tiga harga — yang murah ditampilin, yang mahal disembunyiin di balik form. Salah yang ngomong, applied to AI marketing.'
---

Gue scroll YouTube, nemu iklan kursus AI Rp 350.000.

Tagline-nya: *tanpa belajar coding.*

Gue buka Wappalyzer. Stack-nya Ruby on Rails.

---

Rails itu Ruby. MVC. ActiveRecord. Migrations. Asset pipeline. Framework yang dipake GitHub, Shopify, Basecamp, dan ribuan senior developer yang udah 10+ tahun di lapangan. Ini bukan stack-pemula. Bukan stack yang lo pilih kalau lo "tanpa coding."

Course-nya 31 video. Module 2 nama lesson-nya **"Kenapa Ruby on Rails."** Module 3 deploy ke VPS dengan SSL aktif. Module 5 integrasi payment gateway lewat webhook + re-fetch pattern. Lesson 1.3 setup Windows via WSL2.

Tagline-nya tetep: *tanpa belajar coding.*

Salah satu di antara dua itu bohong. Tebak yang mana.

## FAQ-nya jujur. Marketing-nya nggak.

Gue baca FAQ-nya. FAQ-nya jujur. Itu yang bikin marketing-nya nyakitin.

> Headline: *Tanpa Jadi Programmer.*
> FAQ #1: *AI yang nulis kode, kamu yang arahin.*

Lo gak bisa ngarahin kode tanpa ngerti kode. Yang lo arahin itu apa kalau lo gak ngerti structure-nya — bayangin lo arahin orang ke arah yang lo sendiri gak tau.

> Tagline: *Tanpa belajar coding.*
> FAQ #7: *Lesson 1.3 cover setup Windows via WSL2.*

WSL2 itu Windows Subsystem for Linux. Lo install bukan karena lucu. Lo install karena Windows-native gak cukup, dan course-nya butuh Linux toolchain. Itu bukan absence-of-coding. Itu coding's prerequisite. Linguistik dasar.

> Marketing: *Course ini ngajarin yang AI gak bisa.*
> FAQ #8: *PRD, schema design, permission reasoning, deploy decision.*

Itu literally apa yang dikerjain programmer setiap hari. Bukan programmer junior — programmer yang udah ngerti **kenapa** schema-nya begini, **kenapa** permission isolated per-tenant, **kenapa** deploy blue-green bukan in-place restart.

Yang dia tukar di tagline cuma satu kata: *programmer → arahin.*

Tapi yang ngarahin programmer **adalah** programmer.

## Form dulu. Harga belakangan. Tapi gak selalu.

Iklan yang gue liat tadi: Rp 350.000.

Itu harga kursus Excel. Bukan kursus AI yang gue baca selama 10 menit.

Kursus yang gue baca — *Bikin Aplikasi Pakai AI* — **Rp 950.000.**

Lo gak tau itu sampe lo isi nama, email, nomor HP. Form dulu. Harga belakangan.

Mereka punya 3 produk:

- Kursus Excel — **Rp 350.000.** Harganya keliatan di landing page. Dua kali. Atas dan bawah.
- *Bikin Aplikasi Pakai AI* — **Rp 950.000.** Halaman pake template yang sama. Section yang sama: *"Ubah Hidup Anda Hari Ini."* CTA yang sama: *"Belajar Sekarang."* Beda satu hal — angkanya gak ada.
- *BelajarGPT Pro* — **Rp 1.200.000.** Sama. Angkanya gak ada.

Lo ngeliat angka cuma kalo angkanya kecil enough buat keliatan menarik.

Lo gak ngeliat angka kalo angkanya gede enough buat orang mikir dua kali.

Itu bukan oversight. Itu *deliberate.* Designer yang sama, template yang sama, halaman yang dijejer sebelahan di nav-bar. Yang berubah cuma satu — visibility harga.

FAQ #5: *"Detail kita kasih di onboarding setelah daftar (transparent biar kamu bisa decide sebelum mulai)."*

Lo decide setelah ngasih nama, email, nomor HP.

Itu bukan transparent. Itu funnel.

## "Effort setara no-code." Math-nya gak masuk.

Body copy-nya bilang:

> *Effort setara no-code tapi hasilnya web-app beneran.*

No-code itu Bubble, Replit, Lovable. Rp 600K/bulan. Selesai. Itu effort-nya — drag-drop, klik publish, jalan.

Course ini? Rp 950K (sekali) + Claude Pro/Max ($20–100/bulan) + sewa VPS (Rp 50–150K/bulan) + domain (Rp 150K/tahun) + payment gateway fee + quarterly plugin update yang lo harus follow + swap guide kalo Anthropic naik harga + 2 jam/malam konsisten 3–4 bulan + WSL2 setup + Cloudflare DNS + webhook security pattern + Kamal deploy.

Effort setara? Math-nya gak masuk.

Itu bukan no-code. Itu **coding-yang-typing-nya-di-outsource**. Beda. Dan bedanya itu yang bikin lo bisa ship hal yang valuable. Tapi *"effort setara no-code"* itu bukan ngomong jujur ke calon murid — itu ngomong yang calon murid mau denger.

## AI ngambil typing-nya. Bukan thinking-nya.

Yang AI ambil dari lo:

- typing tag HTML yang lo udah tau bentuknya
- syntax bahasa yang asing tapi pattern-nya familiar
- boilerplate auth yang sama di setiap project
- generate 12 file scaffold dalam 30 detik
- explain error stack trace dalam bahasa indo

Yang AI **gak** ambil:

- decide schema-nya begimana sebelum lo prompt
- baca error yang gak ke-fix sama AI dan tau itu permission issue, bukan typo
- decide deploy lewat Kamal, Coolify, atau plain Docker
- tau kapan lo butuh background job, kapan lo butuh cron
- decide *"ini fitur layak dibikin"* atau *"ini fitur yang bakal bikin gue stuck 2 minggu"*

Course William ngajarin yang kolom kanan. Curriculum-nya solid. Yang kolom kiri — AI ngerjain. Yang kolom kanan — lo tetep harus mikir, dan mikir-nya itu **adalah coding**, cuma bentuk lain.

Itu yang gue maksud: **AI ngambil typing-nya, bukan thinking-nya.**

## Gue exhibit yang sama

Gue bukan IT. <span class="t-mono">English Education di Unikama.</span> Gue ship Bisnapi pake AI 70% of the time. Boilerplate, types, scaffolding — Claude Code yang nulis. Gue yang baca, edit, deploy.

Tapi 30% sisanya itu yang nentuin Bisnapi survive 1 bulan atau 1 tahun.

Schema migration yang jaga data UMKM. Permission layer yang isolasi tenant satu sama lain. Webhook yang gak duplicate transaksi pas Mayar fire 3x karena network blip. Background job yang clean-up orphan records sebelum data store penuh.

Itu semua gue belajar bukan dari course AI. Bukan dari Cursor. Bukan dari Claude Code. **Dari stuck.**

Stuck pas migration gagal jam 2 pagi karena lo gak ngerti foreign key constraint. Stuck pas permission bocor karena lo skip session-isolation. Stuck pas webhook fire 3x karena lo gak idempotent. Stuck pas deploy crash karena RAM 1GB gak cukup buat Rails + Sidekiq + Postgres.

AI gak ngambil **stuck**-nya. Stuck itu yang ngajarin lo apa-yang-sebenernya-perlu-lo-tau.

Course yang dijualin "tanpa coding" gak siap untuk stuck — karena marketing-nya bilang stuck-nya udah dihandle AI.

## Salah yang ngomong, bukan yang belinya

[Sebelumnya gue tulis](/blog/salah-yang-ngomong): *kalau orang gak ngerti yang lo omongin, itu salah lo, bukan salah dia.*

Sama berlaku di sini.

Yang stuck di module 4 — yang nyerah pas error pertama yang Claude gak bisa fix — itu **bukan** bodoh. Mereka cuma orang yang dijualin *"tanpa coding"* tanpa dikasih tau coding-nya yang mana yang tetep harus diketauin.

Mereka dikasih setir. Diajarin gas, rem, kopling. Tapi gak dikasih peta. Gak ditunjukin jalan-jalan kecil yang nipu di Google Maps. Gak diajarin baca kompas pas signal hilang.

Pas lo nyasar, marketing bakal bilang lo yang salah. *Lo kurang konsisten. Lo kurang prompting skill. Lo kurang join komunitas.*

Padahal yang salah itu yang bilang ada jalan tanpa peta.

## Yang harusnya dikatakan

> *Bikin software dengan coding yang lebih sedikit.*

Bukan **tanpa**. **Lebih sedikit**.

Bedanya satu kata. Konsekuensinya beda total. Yang pertama kasih lo skill realistis di tangan, yang kedua kasih lo dream yang bocor pas lo nyentuh production.

Untuk konteks — gue gak beli course-nya. Curriculum-nya solid di atas kertas, dari FAQ + outline yang publicly visible. Gue gak tau William jelasin WSL2-nya kayak gimana di depan orang yang beneran gak pernah coding. Mungkin pelan dan sabar. Mungkin lewat sambil bilang *"pokoknya jalan."* Gue gak akan claim sesuatu yang gue gak punya akses.

Yang gue critique itu yang publicly visible — landing, FAQ, marketing copy, harga yang disembunyiin. Itu yang nge-shape ekspektasi murid sebelum mereka masuk. Itu yang bikin orang bayar Rp 950K dengan pikiran satu hal, terus dapet pikiran lain.

Course AI bagus itu yang jujur soal apa yang lo bakal hadapi. Yang ngakuin bahwa AI ngambil 70% kerja, dan 30% sisa itu yang justru paling berat. Yang ngajarin lo *cara stuck* — bukan janji lo gak akan stuck.

Karena lo bakal stuck. Itu bukan bug. Itu cara belajarnya.

---

> AI ngambil typing.
> AI gak ngambil thinking.
> Lo dikasih setir.
> Lo gak dikasih peta.
> Yang stuck bukan bodoh — yang ngomong yang salah.
