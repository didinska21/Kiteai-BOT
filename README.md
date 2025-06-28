# Kiteai-BOT

Bot otomatis untuk mengelola akun EVM, termasuk fitur claim faucet dan fitur lainnya (WIP). Dibuat dengan Python 3.12 dan mudah dijalankan dengan virtual environment.

## Fitur Utama

- Otomatisasi klaim faucet (via 2captcha)
- Multi-akun EVM
- Proses berulang dengan dukungan multi-thread (coming soon)
- Ideal untuk testing, riset, dan automation crypto tools

## Instalasi

### 1. Clone repository
```bash
git clone https://github.com/didinska21/Kiteai-BOT
cd Kiteai-BOT
```

### 2. Install Python dan Virtual Environment
```bash
sudo apt update
sudo apt install python3.12
sudo apt install python3.12-venv
```

### 3. Setup environment
```bash
python3 -m venv venv
source venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

## Konfigurasi

### API Key 2Captcha (Opsional, untuk fitur klaim)
Buat file `2captcha_key.txt` dan masukkan API key dari [2captcha.com](https://2captcha.com/):
```bash
nano 2captcha_key.txt
```

### Daftar Akun EVM
Masukkan address EVM kamu ke dalam `accounts.txt`:
```bash
nano accounts.txt
```

Format:
```
0xabc123...
0xdef456...
```

## Menjalankan BOT

### Run
```bash
python bot.py
```

### (Opsional) Jalankan di background
```bash
nohup python bot.py &
```

## Contoh Struktur File
```
Kiteai-BOT/
â”œâ”€â”€ accounts.txt
â”œâ”€â”€ 2captcha_key.txt
â”œâ”€â”€ bot.py
â”œâ”€â”€ requirements.txt
â””â”€â”€ ...
```

## FAQ

Q: Apakah bisa jalan di Windows?  
A: Belum diuji, tapi kemungkinan besar bisa dengan Python 3.12 dan venv.

Q: Apakah bisa dipakai tanpa 2captcha?  
A: Bisa, tapi hanya fitur yang tidak memerlukan captcha.

Q: Apakah ini open source?  
A: Ya. Silakan fork dan kembangkan!

## Kontak

Dikembangkan oleh Didin Ska  
Untuk pertanyaan atau kontribusi, silakan buka issue di GitHub.

## Lisensi

MIT License
