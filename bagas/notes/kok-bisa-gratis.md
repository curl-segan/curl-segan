---
title: 'Kok bisa gratis? Duit siapa yang dibakar?'
date: 2026-05-20
description: 'Bukan duit investor. Bukan duit lo. Duit gue — $30/bulan.'
pull: '$30/bulan. Flat. 1 RAKJAT atau 10,000 RAKJAT — gue bayar sama.'
tags: ['infra', 'pricing', 'rakjat', 'cloudflare']
---

Gue sering ditanya: kok bisa gratis? Fiturnya beneran sama? Ada hidden cost-nya? Duit siapa yang dibakar?

Jawaban yang bikin investor seneng: "growth strategy, land-and-expand, freemium funnel." Jawaban yang bikin tech bro angguk-angguk: "marginal cost mendekati nol di scale."

Semua bener. Tapi bukan itu.

**Alasan utama: gue gak punya investor yang duitnya perlu dibakar.**

## Matematikanya

[Post sebelumnya](/blog/kenapa-cloudflare) gue jelasin kenapa gue pilih Cloudflare. Sekarang gue kasih liat efeknya ke lo.

Infra Bisnapi sebulan:

| Stack | Biaya | Catatan |
|-------|-------|---------|
| Cloudflare Workers | **$5** | Compute, flat, 10 juta request included |
| Aiven Postgres | **$25** | Database, flat, unlimited queries |
| Bandwidth | **$0** | Unlimited. Selamanya. |
| R2 Storage | **$0** | 10 GB included |
| **Total** | **$30/bulan** | **Flat. Gak naik pas lo sukses.** |

Mau 1 RAKJAT atau 10,000 RAKJAT — gue bayar sama.

200 transaksi/hari per RAKJAT. 1,000 RAKJAT aktif. Itu 6 juta request/bulan — masih 60% dari included allocation. Database? Unlimited queries, flat $25. Gak ada per-row charge. Gak ada "usage spike" yang bikin tagihan meledak jam 2 pagi.

$30/bulan. 1,000 RAKJAT. Itu matematikanya.

## Kenapa yang lain gak bisa?

| | Bisnapi (CF + Aiven) | AWS Equivalent |
|---|---|---|
| Compute | $5 (Workers flat) | $30 (EC2 + ALB) |
| Database | $25 (Aiven flat) | $25 (RDS — tapi **naik** kalau traffic naik) |
| Bandwidth | $0 | $14 (dan naik terus) |
| Monitoring | $0 (included) | $10+ |
| **Total 1K RAKJAT** | **$30** | **$72+** |
| **Total 10K RAKJAT** | **$30** | **$310+** |

10,000 RAKJAT? AWS udah $310/bulan. Database perlu scale, bandwidth $135 **doang**. Gue? Tetep $30. Flat. Aiven gak charge per-query. Cloudflare gak charge per-GB.

Makanya free tier mereka dipangkas abis-abisan kaya orang cukur rambut model tentara. Bukan karena pelit — karena infrastruktur mereka yang mahal.

*(Dan jujur — bukan cuma infra. Lo juga bayarin WeWork mereka, billboard mereka, sama "Customer Success Manager" yang kerjanya kirim email template.)*

## "Tapi database flat $25 gak bakal kuat?"

Aiven Postgres — managed, auto-backup, monitoring built-in. $25/bulan buat plan yang handle ratusan ribu queries per hari tanpa keringetan. Ini bukan SQLite di laptop — ini Postgres enterprise-grade yang di-host di cloud, cuma tanpa markup 4x yang biasa lo bayar di AWS RDS.

Kenapa Aiven? Karena mereka juga inget rasanya jadi kecil. Plan $25 mereka bukan "starter yang sengaja di-throttle." Itu plan yang beneran jalan buat production workload.

Sama kayak Cloudflare — gue pilih partner yang pricing model-nya **flat**, bukan yang nge-charge lo lebih mahal pas lo lagi sukses.

## "Kalau 50K RAKJAT?"

Upgrade Aiven ke plan berikutnya — $50/bulan. Still flat. Still unlimited queries. Cloudflare? Mungkin nambah $15-20 buat request overage. Total jadi $70/bulan buat serve 50,000 RAKJAT.

AWS di titik yang sama? $675 bandwidth **doang**. Belom compute, belom database scale.

Dan kalau Aiven atau Cloudflare tiba-tiba pivot pricing? Sama kayak yang gue tulis di [post sebelumnya](/blog/kenapa-cloudflare) — hari itu terjadi, gue mulai cari exit plan. Sampe situ, bet yang gue ambil sadar.

## "Terus lo dapet duit dari mana?"

RAKJAT gratis. Yang bayar dapet dedicated AI neurons, multi-outlet, HRIS, tax automation, priority support. Fitur yang emang butuh compute lebih — jadi masuk akal kalau ada harga.

Tapi RAKJAT? 200 transaksi/hari, POS, laporan, stok? Cost gue buat serve 1 RAKJAT itu **kurang dari Rp 5 per hari**. Gue gak perlu charge lo apa-apa. Bukan charity — emang gak worth it buat di-charge.

## Compliance yang gak perlu gue bayar mahal

Cloudflare: ISO 27001, SOC 2 Type II, PCI DSS Level 1.

Aiven: ISO 27001, SOC 2 Type II, HIPAA, GDPR.

Data lo literally di infra mereka. Karena infra-nya udah certified, gue cuma perlu urus layer aplikasi doang. Scope audit kecil = biaya audit kecil = timeline pendek.

SaaS yang self-host di bare metal? Audit **semua layer**. Physical. Network. Infra. App. Mahal. Lama. Makanya banyak yang claim "ISO 27001 aligned" — kedengeran keren, tapi artinya: belum certified, cuma ngikutin framework-nya doang.

Gue juga belum certified — yet. Bedanya — jalan gue ke situ lebih pendek dan lebih murah. Karena gue pilih partner yang udah jalan duluan, bukan karena gue lebih pinter.

## Deal-nya

Temen gue yang jualan frozen food — margin seribu-dua ribu per bungkus, jual 20 biji sehari kalau lagi rame. Lo mau dia bayar Rp 150k/bulan buat software? Itu 5 hari kerja dia cuma buat bayar tools.

Gue di sini bukan buat siphon duit dari kerja keras lo. Lo udah capek jualan dari pagi, ngitung stok, bayar karyawan, urus pajak. Lo gak butuh software yang nambah beban — apalagi yang nge-charge lo lebih mahal pas bisnis lo mulai jalan.

Gue di sini sebagai enabler. Kasih lo tools yang proper — Silicon Valley grade, harga nasi kucing — tanpa minta lo bayar harga enterprise buat fitur yang harusnya standar.

Itu deal-nya. Gue jaga infra. Lo fokus jualan. Titik.

## Rantainya

> Cloudflare kasih gue $0 bandwidth.<br>
> Aiven kasih gue $25 unlimited database.<br>
> Dua-duanya kasih gue compliance scope yang kecil.<br>
> Gue kasih lo $0 RAKJAT tier — fitur sama, tanpa batas waktu.<br>
> Lo grow, lo hire, keluarga lo makan.

RAKJAT bukan charity. Bukan marketing gimmick. Bukan "limited time offer."

**Itu matematika yang gue pass ke lo.**
