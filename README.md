# Form Pengajuan Memo (GitHub Migration)

Proyek ini memigrasikan frontend "Form Pengajuan Memo" dari Google Apps Script (HTMLService) ke standalone frontend (GitHub Pages) dengan desain modern dan sistem SSO.

## Struktur Project

```text
├── gas/                 # BACKUP - Script asli yang berjalan di GAS (HTML Service)
├── index.html           # NEW - Frontend baru (Premium UI + SSO) - Deploy ke GitHub
├── api-backend.gs       # NEW - Script API baru untuk backend (Fetch-based)
├── SETUP.md             # Panduan instalasi dan deployment
└── README.md            # Dokumentasi project ini
```

## Fitur Utama

1.  **Premium UI**: Desain Glassmorphism modern dengan dukungan Dark & Light mode.
2.  **SSO (Single Sign-On)**: Menggunakan Google Identity Services untuk login otomatis dan pencatatan identitas pengirim yang aman.
3.  **Decoupled Architecture**: Frontend berjalan secara independen (bisa di GitHub Pages, Vercel, dll) dan berkomunikasi via API ke Google Apps Script.
4.  **Google Sheets Integration**: Tetap menggunakan Google Sheets sebagai database utama.

## Cara Menggunakan

Silakan ikuti instruksi lengkap pada file **[SETUP.md](SETUP.md)** untuk:
1.  Mendapatkan Google Client ID untuk SSO.
2.  Mendeploy `api-backend.gs` sebagai Web App.
3.  Konfigurasi URL API di `index.html`.

## Lisensi
Proyek Internal CMU.
