# 🔥 MR44J - Proxy Checker Massal

**MR44J** adalah alat berbasis web untuk mengecek banyak proxy sekaligus (IP:PORT) secara cepat, ringan, dan tanpa backend tambahan.

🌐 Live: [https://mass-pro.xychecker.workers.dev](https://mass-pro.xychecker.workers.dev)

---

## ✨ Fitur Utama

- ✅ Deteksi proxy aktif/inaktif
- 🌍 Menampilkan negara dan bendera
- 🏢 Informasi organisasi (ASN/ISP)
- ⚡ Delay dan protokol koneksi
- 📂 Upload banyak file `.txt`
- 📝 Input manual proxy
- 💾 Penyimpanan otomatis ke browser
- 📋 Salin & Unduh proxy aktif
- 🌙 Tampilan dark mode
- 🔁 Auto-scroll saat pengecekan berlangsung

---

## 📥 Cara Penggunaan

1. Masukkan proxy secara manual (format: `IP:PORT`)
2. Atau, upload file `.txt` yang berisi daftar proxy
3. Klik tombol **"Mulai Cek"**
4. Lihat hasil di tabel: status, negara, organisasi, protokol, dan delay
5. Gunakan fitur salin atau unduh untuk menyimpan proxy aktif

### Format Input yang Didukung
```
127.0.0.1:8080
38.180.100.80:443
```

---

## 📤 Output

| No | IP | Port | Status   | Country | Org           | Protocol | Delay |
|----|----|------|----------|---------|---------------|----------|-------|
| 1  | ...| ...  | Active ✅| 🇺🇸 US  | Cloudflare, Inc | HTTP/1.1 | 105ms |

---

## 🚀 Teknologi

- **Cloudflare Workers** – untuk API & UI
- **HTML + Vanilla JS** – antarmuka pengguna
- **Fetch API** – komunikasi data
- **API eksternal** – `https://apihealtcheck.vercel.app`

---

## 🧪 Simpanan Otomatis

- Tabel hasil dan statistik akan otomatis disimpan ke **localStorage**
- Saat halaman dimuat ulang, data sebelumnya akan tetap tampil

---

## 📦 Deploy Sendiri (Opsional)

1. Install `wrangler`:
   ```bash
   npm install -g wrangler
   ```

2. Inisialisasi proyek:
   ```bash
   wrangler init mr44j
   ```

3. Ganti isi file `src/index.js` dengan kode dari `worker.js`

4. Deploy ke Cloudflare:
   ```bash
   wrangler publish
   ```

---

## 🧑‍💻 Developer

**MR44J** dikembangkan oleh [MR44J](https://mass-pro.xychecker.workers.dev) sebagai alat open-source untuk membantu pengecekan proxy secara efisien dan cepat.

---

## 📝 Lisensi

MIT License © 2025

---

> Dibuat dengan ❤️ untuk para hunter dan developer oleh **MR44J**