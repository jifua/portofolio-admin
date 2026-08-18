# Portofolio Admin — Fitria Rozi

Situs statis (HTML biasa, tanpa framework) berisi ringkasan 3 proyek Excel
dan tombol unduh file aslinya. Siap deploy ke Vercel tanpa proses build.

## Isi folder
```
index.html                 -> halaman portofolio
files/
  Portofolio_Admin_HR.xlsx
  Portofolio_Admin_Purchasing.xlsx
  Portofolio_Admin_Inventory_FIFO.xlsx
```

## Cara deploy ke Vercel (pilih salah satu)

### Opsi A — lewat GitHub (paling umum & mudah dikelola)
1. Buat repository baru di GitHub, upload semua isi folder ini (index.html + folder files/).
2. Buka https://vercel.com -> Add New -> Project -> Import Git Repository -> pilih repo tadi.
3. Framework Preset pilih "Other" (karena ini HTML statis, tidak perlu build command).
4. Klik Deploy. Selesai dalam ~30 detik, dapat URL seperti nama-proyek.vercel.app.

### Opsi B — lewat Vercel CLI (tanpa GitHub)
1. Install Node.js kalau belum ada.
2. Buka terminal di folder ini, jalankan:
   ```
   npm install -g vercel
   vercel login
   vercel
   ```
3. Ikuti pertanyaan di terminal (pilih "Link to existing project? No", biarkan default lainnya).
4. Setelah selesai akan muncul URL live-nya langsung di terminal.

## Update file di kemudian hari
Ganti file .xlsx di folder `files/`, commit & push ulang (opsi A) atau jalankan
`vercel --prod` lagi (opsi B) — link URL tidak berubah.
