# Silent Sonata

Silent Sonata adalah game web rhythm-reaction psikologis fantasi tentang seorang pianis muda yang terjebak di dunia koma. Pemain berperan sebagai inner listener: bagian kesadaran yang masih bisa membedakan musik yang jujur dari visual yang menipu.

Premis utama game:

> Vision lies. Music tells the truth.

Game ini berjalan langsung di browser melalui satu file utama, `index.html`, dengan visual 3D real-time, audio sintetis dari Web Audio API, pilihan bahasa Indonesia/English, stage progression, dan pengaturan aksesibilitas dasar.

## Status Project

Status saat ini: Final Release / playable browser build.

Isi repository saat ini:

- `index.html` - build game utama yang dapat dimainkan.
- `Silent_Sonata_Full_Game_Execution_Documentation_v2.0.md` - dokumen desain, cerita, sistem, produksi, dan QA lengkap.
- `README.md` - panduan project ini.

## Fitur Utama

- Game browser single-page tanpa proses build.
- Visual 3D menggunakan Three.js.
- Audio interaktif menggunakan Web Audio API.
- Sistem nada inti: Low, Mid, dan High.
- Gameplay rhythm-reaction berbasis mendengarkan, mengingat, lalu memilih sumber suara.
- Mekanik false visual cue: visual dapat menipu, suara menjadi petunjuk utama.
- Mekanik silence: pada beberapa sequence, jawaban benar adalah tidak menekan apa pun.
- Mekanik echo/reflection: pemain membandingkan nada asli dengan pantulan yang sudah rusak.
- Sistem Memory Corruption sebagai soft-fail, bukan game over keras.
- Progression lock untuk membuka stage secara berurutan.
- Bilingual UI: Indonesia dan English.
- Pengaturan assist timing, timing ring, dan mono audio.
- Content warning bawaan di menu utama.

## Cerita Singkat

Liora, seorang pianis muda, mengalami kecelakaan setelah konser penting dan masuk koma. Di dalam pikirannya, memori, rasa bersalah, tekanan performa, dan harapan untuk pulang berubah menjadi dunia musikal yang surreal.

Pemain membantu Liora memulihkan tiga nada inti, menyusun kembali Final Sonata, dan menghadapi memori-memori yang rusak tanpa bergantung sepenuhnya pada penglihatan.

## Cara Memainkan

1. Dengarkan nada atau sequence yang dimainkan.
2. Perhatikan bahwa visual tidak selalu benar.
3. Saat instruksi muncul, klik sumber suara yang sesuai.
4. Untuk sequence, klik objek dalam urutan nada yang benar.
5. Untuk instruksi `DIAM` / `SILENCE`, jangan klik apa pun sampai waktu habis.
6. Jika salah, Memory Corruption meningkat dan sequence akan diulang.
7. Selesaikan semua sequence untuk membuka chapter berikutnya.

## Objek Nada

| Nada | Objek | Makna | Identitas Audio |
| --- | --- | --- | --- |
| Low | Blue Orb | Grounding / breath | Nada rendah, condong kiri |
| Mid | Rose Crystal | Heart / memory | Nada tengah, posisi tengah |
| High | Gold Prism | Hope / awakening | Nada tinggi, condong kanan |

## Struktur Stage

| Stage | Nama | Fokus Gameplay |
| --- | --- | --- |
| Prologue | The First 3 Notes | Latihan tiga nada inti melalui 5 fragmen |
| Chapter 1 | The Silent Room | Memahami aturan dunia dan silence mechanic |
| Chapter 2 | Hall of False Notes | Echo, pantulan rusak, dan koreksi nada |
| Chapter 3 | The Broken Concert | Tekanan panggung, applause palsu, sequence cepat |
| Chapter 4 | The Accident Memory | Heartbeat, jeda, dan trauma yang divisualkan secara simbolis |
| Chapter 5 | The Last Sonata | Gabungan seluruh motif menuju finale |
| Epilogue | Awakening | Penutup cerita dan kepulangan |

## Menjalankan Game

### Opsi 1: Buka langsung

Buka file berikut di browser:

```text
index.html
```

Cara ini biasanya cukup untuk memainkan game.

### Opsi 2: Jalankan dengan local server

Jika browser membatasi resource tertentu, jalankan server lokal dari folder project:

```bash
python -m http.server 8000
```

Lalu buka:

```text
http://localhost:8000
```

Catatan: `index.html` memuat Tailwind CSS, Three.js, dan Google Fonts dari CDN. Koneksi internet diperlukan agar tampilan dan library eksternal termuat dengan benar.

## Teknologi

- HTML
- CSS
- JavaScript
- Tailwind CSS CDN
- Three.js CDN
- Web Audio API
- Inline SVG untuk ilustrasi memory reveal

## Kontrol

| Aksi | Kontrol |
| --- | --- |
| Mulai game | Klik tombol `Mulai Pemulihan` / `Begin Recovery` |
| Pilih stage | Klik `Pilih Stage` / `Select Stage` |
| Mengganti bahasa | Klik tombol `ID` / `EN` di menu |
| Memilih nada | Klik objek 3D yang sesuai |
| Bermain di layar sentuh | Tap objek yang sesuai |
| Membuka pengaturan | Klik tombol settings di HUD |

## Pengaturan Aksesibilitas

Game menyediakan beberapa opsi bantu:

- Assist Timing: memperpanjang reaction window.
- Timing Ring: menampilkan indikator waktu.
- Mono Audio: mengubah audio stereo menjadi mono.

Rekomendasi bermain: gunakan headphone atau speaker stereo agar identitas arah Low/Mid/High lebih mudah terbaca.

## Content Warning

Game ini mengeksplorasi tema koma, memori, tekanan performa, dan trauma pasca-kecelakaan secara simbolis. Tidak ada jumpscare atau kekerasan visual eksplisit, tetapi beberapa sequence memakai suasana gelap, distorsi audio, dan imagery kecelakaan yang abstrak.

## Struktur Kode Singkat

Semua implementasi utama berada di `index.html`:

- `DICT` - teks UI bilingual.
- `STORY` - memory reveal setiap chapter.
- `SVGS` - ilustrasi ending/chapter reveal.
- `AudioSystem` - mesin audio berbasis Web Audio API.
- `VisualSystem` - scene, kamera, objek, partikel, dan interaksi Three.js.
- `GameController` - state machine, progression, input, fail/success, dan chapter flow.

## State Gameplay

Game memakai alur state sederhana:

```text
MENU -> CUTSCENE -> INIT -> LISTEN -> CLICK_NOW -> RESULT -> DONE
```

Inti desainnya adalah pemain harus mendengar dulu, baru bertindak. Klik terlalu cepat akan dianggap gagal karena pemain belum "mendengarkan".

## Progression dan Save

Build saat ini menyimpan progression di runtime selama sesi bermain. Stage berikutnya terbuka setelah chapter selesai. Jika halaman di-refresh, progression dapat kembali ke awal karena belum ada sistem penyimpanan permanen yang aktif.

## Troubleshooting

Jika layar gelap atau visual tidak muncul:

- Pastikan browser mendukung WebGL.
- Pastikan koneksi internet aktif untuk memuat Three.js dari CDN.
- Coba jalankan melalui local server.

Jika audio tidak terdengar:

- Klik tombol mulai terlebih dahulu. Browser modern hanya mengizinkan audio setelah interaksi pengguna.
- Pastikan volume browser dan perangkat aktif.
- Gunakan headphone untuk pengalaman terbaik.

Jika tampilan terlihat polos:

- Pastikan Tailwind CSS CDN berhasil dimuat.
- Periksa koneksi internet.

## Dokumentasi Produksi

Dokumen desain lengkap tersedia di:

```text
Silent_Sonata_Full_Game_Execution_Documentation_v2.0.md
```

Dokumen tersebut mencakup:

- production document,
- narrative bible,
- gameplay and systems bible,
- level and encounter design,
- music and audio bible,
- art and asset direction,
- technical implementation plan,
- UX, accessibility, sensitivity, dan QA plan,
- roadmap produksi dan backlog.

## Roadmap Lanjutan

Beberapa pengembangan yang disarankan:

- Memisahkan `index.html` menjadi struktur modular `src/`.
- Menambahkan persistent save via `localStorage`.
- Menambahkan volume slider untuk music, SFX, ambience, dan accessibility cues.
- Menambahkan keyboard controls.
- Menambahkan asset eksternal final untuk ilustrasi, audio, dan environment.
- Membuat automated smoke test untuk memastikan scene Three.js dan audio init berjalan.
- Menyiapkan build offline tanpa CDN.

## Lisensi

Lisensi belum ditentukan. Tambahkan file `LICENSE` sebelum distribusi publik atau rilis open-source.

