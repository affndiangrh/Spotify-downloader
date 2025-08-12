# Spotify Downloader With CLI

**Spotify Downloader CLI** adalah aplikasi terminal untuk mengunduh lagu, album, atau playlist dari Spotify dengan metadata lengkap dan cover album. Audio diambil dari YouTube dan dikonversi ke format MP3, FLAC, atau M4A sesuai pilihan. Metadata dan cover album diambil langsung dari Spotify.

### Fitur - Fitur

- Download lagu, album, atau playlist Spotify.
- Mendukung format audio: `mp3`, `flac`, `m4a`.
- Metadata lengkap: judul, artis, album, nomor track, tanggal rilis, cover album.
- Tampilan CLI interaktif dan berwarna.
- Multi-thread download untuk kecepatan maksimal.

### Instalasi

1. **Clone Repository**
   ```sh
   git clone [------](https://github.com/affndiangrh/Spotify-downloader.git)
   cd Spotify-downloader
   ```
2. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```
3. **Install FFmpeg (Wajib)**

   ```sh
   winget install ffmpeg
   ```

   Pastikan FFmpeg sudah ada di PATH.

4. **Buat file `.env`**
   ```
   SPOTIFY_CLIENT-ID=isi_client_id_spotify
   SPOTIFY_CLIENT-SEC=isi_client_secret_spotify
   ```
   Cara mendapatkan Client ID dan Secret:
   - Daftar di [Spotify Developer Dashboard](https://developer.spotify.com/dashboard)
   - Buat aplikasi baru, lalu copy Client ID dan Client Secret.

### Cara Pakai

Jalankan program di terminal:

```sh
python spotify.py
```

Ikuti instruksi di layar, masukkan link Spotify (track, album, atau playlist).

Contoh:

```
>>> Masukkan link Spotify (atau ketik 'exit' untuk keluar): https://open.spotify.com/album/xxxxxxx
```

Pilih format audio dan folder output jika ingin custom:

```sh
python spotify.py -f flac -o MusikSaya
```

### Catatan

- Audio diambil dari YouTube, bukan langsung dari Spotify.
- Format FLAC tetap tergantung kualitas sumber YouTube (bukan lossless asli Spotify).
- Metadata dan cover album diambil dari Spotify.

### Kontributor

- Affandi Anugrah
- GitHub Copilot

---

