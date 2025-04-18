# SowingTaker-Bot 🌱  
Script ini digunakan untuk mengotomatiskan tugas dan klaim mining di platform Sowing Taker.

---
## 📌 New update!

- Loop after process all wallets and wait 3 Hours
---

## 📌 Fitur

- ✅ **Auto Clear Task**  
  Selesaikan semua tugas (Quiz, Follow, Visit) untuk Task ID 6 & 7 dengan jawaban preset (`["C"]`, `["A"]`, `["D"]` untuk quiz, event ID 15 & 16 untuk follow/visit)

- ⏰ **Auto Claim Mining**  
  Klaim reward mining via `/task/signIn` dengan cooldown 3 jam, menampilkan sisa waktu hingga klaim berikutnya

- 🔌 **Dukungan Proxy**  
  Gunakan proxy dari `proxy.txt` (`http`, `socks5`, `socks4`) dengan auto-switch saat gagal untuk koneksi aman

- 🎁 **Menampilkan Status**  
  Info poin, jumlah sign-in, dan reward setelah klaim mining via `/user/info`

- ⚡ **Log Keren**  
  Console log warna-warni dengan `chalk`, emoji seru (✅🎉), dan banner "Airdrop 888" via `cfonts`

- 🔐 **Wallet Aman**  
  Login menggunakan wallet dari `walletsnew.json` dengan `ethers@5` untuk sign nonce

- 🎮 **Prompt Simpel**  
  Pilih "Mau menggunakan proxy? (y/n)" untuk kedua mode, mudah digunakan

---

## 🚀 Cara Penggunaan

### 1. Clone repository ini

```bash
git clone https://github.com/marioatmajanugraha/sowingTaker-Bot.git
cd sowingTaker-Bot
```

### 2. Install Dependencies

```bash
npm install axios chalk@4 cfonts http-proxy-agent socks-proxy-agent ethers@5 readline-sync
```

### 3. Siapkan file konfigurasi

**Buat file `walletsnew.json` dan isi dengan daftar wallet (address dan private key). Contoh:**

```json
[
    {
        "address": "0xcA717C......",
        "privateKey": "your_private_key_here"
    }
]
```

**(Opsional) Buat `proxy.txt` jika ingin menggunakan proxy. Contoh:**

```
http://username:password@host:port
socks5://username:password@host:port
```

### 4. Jalankan Script

**Untuk Auto Clear Task:**

```bash
node task.obf.js
```

**Untuk Auto Claim Mining:**

```bash
node mine.obf.js
```

---

## 🧾 Ikuti Instruksi

- Jawab prompt `Mau menggunakan proxy? (y/n)`  
- Script akan berjalan otomatis, menyelesaikan tugas atau mengklaim mining reward  
- Mining claim akan menampilkan sisa waktu cooldown *(contoh: "2h 59m 45s")* setelah selesai

---

## ⚠️ Disclaimer

Gunakan script ini dengan bijak dan sesuai aturan platform **Sowing Taker**.  
Developer tidak bertanggung jawab atas penyalahgunaan atau banned akun.  
Simpan `walletsnew.json` dan `proxy.txt` dengan aman, **jangan bagikan data sensitif seperti private key.**

---

## 🤝 Kontribusi

Jika ingin berkontribusi, silakan fork repo ini dan ajukan pull request!  
Kami terbuka untuk ide baru dan perbaikan.

---

## 📞 Kontak

- Jika ada pertanyaan, hubungi: [@balveerxyz](https://t.me/balveerxyz)  
- Join channel Telegram gratis: [t.me/airdroplocked](https://t.me/airdroplocked)

---

✨ **Keep Grinding, Keep Earning!** ✨  
🔥 **Airdrop 888 | Grind. Earn. Repeat.** 🔥
