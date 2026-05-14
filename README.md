# Silent Sonata

## Indonesia

Silent Sonata adalah game web rhythm-reaction psikologis fantasi. Pemain membantu seorang pianis muda yang terjebak di dunia koma untuk memulihkan tiga nada inti dan menyusun kembali Final Sonata.

> Visi menipu. Musik berkata jujur.

### Fitur Utama

- Game browser single-file melalui `index.html`.
- Visual 3D menggunakan Three.js.
- Audio interaktif menggunakan Web Audio API.
- Gameplay berbasis mendengar, mengingat, lalu memilih objek nada.
- Tiga nada inti: Low, Mid, dan High.
- Stage progression dari Prologue sampai Epilogue.
- UI bilingual: Indonesia dan English.
- Pengaturan bantu: assist timing, timing ring, dan mono audio.

### Cara Menjalankan

Buka langsung file:

```text
index.html
```

Atau jalankan local server:

```bash
python -m http.server 8000
```

Lalu buka:

```text
http://localhost:8000
```

Catatan: project ini memakai CDN untuk Tailwind CSS, Three.js, dan Google Fonts, jadi koneksi internet diperlukan.

### Cara Bermain

1. Dengarkan nada atau urutan nada.
2. Tunggu instruksi muncul.
3. Klik objek yang sesuai dengan suara.
4. Jika diminta `DIAM`, jangan klik apa pun.
5. Selesaikan stage untuk membuka chapter berikutnya.

Disarankan memakai headphone agar arah suara Low, Mid, dan High lebih jelas.

### Teknologi

- HTML
- CSS
- JavaScript
- Tailwind CSS
- Three.js
- Web Audio API

### File Penting

- `index.html` - file utama game.
- `Silent_Sonata_Full_Game_Execution_Documentation_v2.0.md` - dokumentasi desain dan produksi lengkap.
- `README.md` - ringkasan project.

### Content Warning

Game ini membahas tema koma, memori, tekanan performa, dan trauma pasca-kecelakaan secara simbolis. Tidak ada jumpscare atau kekerasan visual eksplisit.

---

## English

Silent Sonata is a psychological fantasy rhythm-reaction web game. The player helps a young pianist trapped in a coma world recover three core notes and rebuild the Final Sonata.

> Vision lies. Music tells the truth.

### Key Features

- Single-file browser game through `index.html`.
- 3D visuals powered by Three.js.
- Interactive audio powered by the Web Audio API.
- Listen, remember, then select the correct sound object.
- Three core notes: Low, Mid, and High.
- Stage progression from Prologue to Epilogue.
- Bilingual UI: Indonesian and English.
- Assist options: assist timing, timing ring, and mono audio.

### How to Run

Open this file directly:

```text
index.html
```

Or run a local server:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

Note: this project uses CDN links for Tailwind CSS, Three.js, and Google Fonts, so an internet connection is required.

### How to Play

1. Listen to the note or note sequence.
2. Wait for the prompt.
3. Click the object that matches the sound.
4. If the prompt says `SILENCE`, do not click anything.
5. Complete each stage to unlock the next chapter.

Headphones are recommended so the Low, Mid, and High sound directions are easier to recognize.

### Tech Stack

- HTML
- CSS
- JavaScript
- Tailwind CSS
- Three.js
- Web Audio API

### Important Files

- `index.html` - main game file.
- `Silent_Sonata_Full_Game_Execution_Documentation_v2.0.md` - full design and production documentation.
- `README.md` - project summary.

### Content Warning

This game symbolically explores coma, memory, performance pressure, and post-accident trauma. It contains no jumpscares or explicit visual violence.

