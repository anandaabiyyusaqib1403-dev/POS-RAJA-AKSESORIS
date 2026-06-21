# Raja Aksesoris POS

Repository: https://github.com/anandaabiyyusaqib1403-dev/POS-RAJA-AKSESORIS

Website Point of Sale untuk counter HP Raja Aksesoris dengan alur kasir, input transaksi digital, manajemen produk, dashboard laporan, dan cetak struk thermal 58mm.

## Stack

- React + Vite
- Tailwind CSS
- Supabase Auth + PostgreSQL
- Vercel

## Fitur utama

- Login role-based untuk `kasir` dan `pemilik`
- Halaman `/kasir` untuk transaksi aksesoris dan cetak struk
- Halaman `/kasir/digital` untuk pencatatan pulsa, kuota, voucher, dan token
- Halaman `/produk` untuk kelola produk, stok minimum, dan stok masuk
- Halaman `/dashboard` untuk ringkasan omzet, grafik omzet, metode bayar, top produk, dan export CSV
- Mode demo fallback saat env Supabase belum diisi

## Setup lokal

1. Install dependency:

```bash
npm install
```

2. Buat file `.env`:

```bash
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

3. Jalankan migration SQL di `supabase/migrations/20260412_raja_aksesoris_pos.sql`

4. Jalankan app:

```bash
npm run dev
```

## Demo login

- `owner@raja.test` / `demo123`
- `kasir@raja.test` / `demo123`
