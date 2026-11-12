# ⏱️ Timer UKIN PPG

Timer kelas berbasis satu file HTML untuk memantau **urutan kegiatan pembelajaran** (pendahuluan, inti, penutup) agar tidak ada langkah yang terlewat dan waktu tidak terlampaui. Dirancang untuk guru yang berdiri di depan kelas sementara layar timer diletakkan di belakang kelas, sehingga tampilannya besar dan kontras tinggi.

Tanpa instalasi, tanpa backend, tanpa dependensi. Cukup buka `index.html` di browser.

## Fitur

- **Jadwal custom.** Mulai dari kosong, lalu tambahkan bagian, langkah, dan durasi (menit, boleh desimal seperti 0,5).
- **Tampilan jarak jauh.** Jam hitungan mundur raksasa, judul langkah besar, dan baris "Berikutnya" supaya guru tahu apa yang harus disiapkan.
- **Peringatan lewat warna latar.** Gelap saat aman, kuning saat sisa 1 menit atau kurang, merah saat waktu lewat (hitungan berubah menjadi `+0:30`).
- **Status jadwal.** Menampilkan selisih "lebih cepat" atau "terlambat" dari rencana, serta sisa waktu total.
- **Otomatis lanjut** (bisa dimatikan). Timer pindah sendiri ke langkah berikutnya, jadi guru cukup menekan Mulai sekali.
- **Catatan per langkah** yang tampil besar, misalnya pengingat untuk berkeliling memberi scaffolding atau melakukan penilaian proses.
- **Atur langkah dengan mudah.** Tambah, ubah, hapus, dan pindah urutan; lompat ke langkah mana pun.
- **Bunyi dan getar** saat waktu langkah habis, layar dijaga tetap menyala saat timer berjalan, dan mode layar penuh.
- **Tersimpan otomatis** di `localStorage` browser, jadi jadwal dan kemajuan tidak hilang saat halaman ditutup.
- **Contoh bawaan.** Tombol "Isi contoh Modul" memuat jadwal contoh 19 langkah (total 80 menit, 2 × 40 menit) untuk materi Pembersihan Data (*Data Cleaning*), mapel Koding dan Kecerdasan Artifisial kelas 8.

## Cara pakai

1. Buka `index.html` di browser (laptop, tablet, atau HP).
2. Di layar **Atur Langkah**, isi **Bagian**, **Langkah**, **Menit**, dan **Catatan** (opsional), lalu tekan **Tambah langkah**.
3. Tutup pengaturan, lalu tekan **MULAI**.
4. Pada mode manual, tekan **▶▶** untuk lanjut ke langkah berikutnya. Pada mode otomatis, timer pindah sendiri.

### Pintasan keyboard

| Tombol | Fungsi |
| --- | --- |
| `Spasi` | Mulai / jeda |
| `→` | Langkah berikutnya |
| `←` | Langkah sebelumnya |
| `F` | Layar penuh |

## Menjalankan

Bisa mengakses https://mohamadsaifulanwar.github.io/timer-ukin-ppg/ untuk langsung menggunakannya.

## Catatan teknis

- Satu file HTML berisi CSS dan JavaScript murni (*vanilla*).
- Penghitung waktu memakai selisih `performance.now()`, jadi tetap akurat walau tab sempat tertahan.
- Data disimpan per browser dan per perangkat. Jadwal di HP tidak otomatis muncul di laptop.
- Bunyi peringatan baru aktif setelah pengguna menekan tombol Mulai (aturan autoplay browser).

## Lisensi

Siapa saja boleh memakai, mengubah, dan menjual kode ini asalkan tetap mencantumkan https://github.com/mohamadsaifulanwar/.
