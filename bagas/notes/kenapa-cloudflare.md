---
title: 'Kenapa gue pilih Cloudflare.'
date: 2026-05-08
description: 'Bukan karena mereka paling canggih. Karena mereka remember being small.'
pull: 'Cloudflare remember being small. Makanya gue bisa kasih lo free tier yang gak busuk.'
tags: ['infra', 'cloudflare', 'rakjat']
---

Gue sering ditanya: kenapa Bisnapi di Cloudflare? Kenapa gak AWS? Vercel? Supabase?

Jawaban marketing-version-nya: edge-native, latency rendah, post-quantum, single-provider. Semua bener. Tapi itu bukan alasan utama.

**Alasan utama: Cloudflare remember being small.**

## Yang penting bukan story-nya, tapi efek-nya ke lo

Cloudflare started 2009 dengan satu prinsip: bandwidth, DDoS protection, dan CDN harusnya gratis untuk yang masih kecil. 17 tahun kemudian — itu masih bener. $0 bandwidth. $0 DDoS protection. $5/bulan unlimited workers.

Itu yang bikin Bisnapi bisa exist hari ini. Bukan karena gue jago — karena Cloudflare gak nge-charge gue per-request waktu gue masih ngitung-ngitung Rupiah.

## Yang gue bawa ke Bisnapi

Gue 1 orang. Gue bootstrap. Gue gak punya dana 5 milyar buat AWS bills. Tapi karena Cloudflare ngasih gue tools yang masuk akal — gue bisa kasih lo:

- **Tier RAKJAT gratis selamanya.** 100 transaksi/hari. Bukan trial. Bukan versi lite.
- **Mulai Rp 45.000/bulan** buat full POS + ERP + CRM.
- **Latency ~30ms** dari Indonesia, karena Cloudflare punya 300+ edge locations termasuk Jakarta. AWS ap-southeast-1 di Singapore = ~150ms+ kalau lo di luar Jakarta. Selisihnya kerasa pas warung lagi rame jam makan siang.

Soal harga: Bisnapi tier full stack (POS + ERP + HRIS + CRM + Tax) ada di Rp 350k–600k/bulan. Mekari Full Stack — Jurnal + Talenta + Klikpajak + Qontak — sekitar Rp 1.77 juta/bulan, atau ~Rp 5.8 juta/bulan untuk paket enterprise full team. Itu yang bikin angka 96% bisa di-quote dengan jujur. Bukan satu tier vs satu tier — bandingin yang setara.

Gue gak bisa kasih lo itu semua kalau gue di AWS. Bandwidth bills doang udah bunuh margin. Gue harus naikin harga, atau hapus free tier, atau nge-throttle aggressive. Yang artinya — gue bakal jadi Mekari versi kecil.

## "Tapi single-provider itu risk?"

Iya. Gue tau.

Cloudflare bisa down (Juni 2022, Juli 2023). Cloudflare bisa pivot pricing. Cloudflare bisa tiba-tiba decide kalo Asia-Pacific gak strategic.

Tapi 17 tahun mereka udah prove satu hal: mereka gak pernah pivot ke "screw the little guy." Hari mereka mulai charge $0.15/GB bandwidth, gue mulai cari exit plan. Sampe situ — gue all in. Bet yang gue ambil sadar, bukan blind.

Multi-provider di skala UMKM bukan hedge — itu overhead yang gue gak punya budget atau waktu untuk bayar. Single-provider yang trustworthy lebih bagus dari multi-provider yang mahal.

## Rantainya gak berhenti di gue

> Cloudflare remember being small.<br>
> Bagas remember being small.<br>
> Bisnapi remember being small.<br>
> Rakjat Kita — remember being small.

Itu rantainya. Cloudflare kasih gue tools. Gue kasih lo software. Lo grow, lo hire, keluarga lo makan. Lo inget bisnis kecil yang bantu lo waktu lo masih kecil. Begitu seterusnya.

Itu yang gue maksud **"RAKJAT bukan strategi growth, tapi janji."** Free tier bakal tetep ada selamanya — bukan karena gue baik hati, tapi karena Cloudflare jaga gue. Gue cuma nerusin.

Pilih infrastruktur lo bukan dari tech spec doang. Pilih dari **siapa yang bakal masih ada saat lo butuh mereka, dan masih inget gimana rasanya jadi kecil.**
