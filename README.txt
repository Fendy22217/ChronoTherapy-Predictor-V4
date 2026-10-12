CHRONOTHERAPY PREDICTOR — PROTOTIPE OFFLINE

File: index.html, manifest.json, sw.js, ikon PNG.

Fitur awal:
- Dashboard data pasien, pengukuran, laporan
- Input pasien menggunakan kode anonim
- Input pengukuran tekanan darah dengan tanggal/waktu
- Ringkasan deskriptif per pasien
- Ekspor CSV dan cadangan/pemulihan JSON
- Penyimpanan lokal browser
- PWA/offline melalui hosting HTTPS

PENTING:
Versi ini BELUM berisi model prediksi kronoterapi klinis yang tervalidasi. Tidak memberikan rekomendasi waktu pemberian obat. Gunakan hanya untuk uji alur aplikasi dan data simulasi atau data penelitian yang telah dianonimkan dengan izin yang sesuai. Jangan memasukkan nama, NIK, nomor rekam medis, atau data identitas langsung.
Untuk memasang sebagai aplikasi dengan ikon dan dukungan offline, unggah isi folder ke repository GitHub publik dan aktifkan Settings > Pages > Deploy from a branch > main > /(root) > Save. Buka URL Pages saat online, lalu instal melalui menu Chrome > Tambahkan ke layar utama.


IDENTITAS PENGEMBANG:
apt. Fendy Prasetyawan, S.Farm., M.Farm.

DISCLAIMER:
Aplikasi ini dikembangkan sebagai prototipe untuk membantu pencatatan, pengelolaan, dan peninjauan data dalam kegiatan akademik atau penelitian. Apabila digunakan untuk penelitian, pengguna bertanggung jawab memastikan adanya persetujuan etik bila diperlukan, izin penggunaan data, perlindungan kerahasiaan, serta kepatuhan terhadap peraturan dan protokol penelitian yang berlaku. Versi ini belum merupakan instrumen prediksi klinis yang tervalidasi, sehingga hasilnya tidak boleh dijadikan satu-satunya dasar diagnosis, penentuan waktu pemberian obat, atau perubahan terapi. Keputusan klinis harus tetap didasarkan pada penilaian tenaga kesehatan yang berwenang, pedoman klinis, dan bukti ilmiah yang relevan. Validasi dan tanggung jawab atas penggunaan data serta interpretasi hasil berada pada pengguna.

UPDATE VERSI: Kolom ginjal (CKD/eGFR) dihapus. Kesimpulan eksploratif pasien membandingkan rerata tekanan darah pagi dan malam bila tersedia minimal dua pengukuran untuk masing-masing periode. Fitur ini tidak menentukan jadwal minum obat dan belum tervalidasi secara klinis.

UPDATE OUTPUT: Jika rerata tekanan darah pagi relatif lebih tinggi, aplikasi menampilkan 'Kandidat untuk evaluasi pemberian malam'; jika tekanan darah malam relatif lebih tinggi, aplikasi menampilkan 'Kandidat untuk evaluasi pemberian pagi'. Jika selisih kecil atau pengukuran kurang dari 2 pada setiap periode, aplikasi menyatakan belum cukup dasar. Ini aturan eksploratif, bukan rekomendasi klinis tervalidasi; jangan mengubah jadwal obat tanpa evaluasi tenaga kesehatan.

VERSI 4 — SARAN WAKTU & EFEKTIVITAS TERAMATI:
- Menampilkan kandidat waktu evaluasi berdasarkan perbandingan pola tekanan darah pagi/malam.
- Mencatat hubungan waktu pengukuran dengan dosis: sebelum dosis, 1–4 jam, 4–8 jam, >8 jam, atau tidak diketahui.
- Jika tersedia sedikitnya dua pengukuran sebelum dosis dan dua pengukuran 1–4 jam setelah dosis, menampilkan perubahan rerata tekanan darah teramati. Ini bukan bukti kausal dan tidak menyimpulkan bahwa obat lebih efektif pagi atau malam.
- Perbandingan efektivitas pagi vs malam memerlukan rancangan penelitian yang memadai, data waktu dosis, pengukuran berulang yang terstandar, serta validasi statistik/klinis.
