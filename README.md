# LAMSPAK 2.0 Logic Assessor · @ramalabs

## Fungsi
Aplikasi untuk telaah awal FED IAPS 2.0 **Sarjana Unggul** dengan **73 indikator** matriks. Terdiri dari impor FED, pencocokan nomor butir, audit unsur rubrik, usulan skor **indikatif** jika dasar tekstual memadai, deskripsi dan rekomendasi spesifik, perhitungan terstruktur pada lima syarat perlu Unggul, serta penilaian/verifikasi manual.

## Cara memakai
1. Buka `index.html` dengan browser modern atau terbitkan melalui GitHub Pages.
2. Unggah FED format DOCX, TXT atau PDF yang memiliki teks, atau tempelkan teks. **PDF menggunakan pdf.js dari CDN sehingga memerlukan internet** ketika pertama digunakan; PDF hasil scan perlu OCR lebih dulu.
3. Telaah halaman "Penilaian otomatis" dan buka setiap indikator. Audit menampilkan unsur rubrik yang teridentifikasi dan kutipan penopangnya.
4. Untuk indikator **9, 16, 55, 56, 60**, gunakan formulir angka/cek-bukti tambahan; aplikasi menghitung skor sementara dari input tersebut dengan peringatan keterbatasan sumber.
5. Masukkan nomor/halaman dokumen yang sudah dicek dan catat penilaian manual. **Kecocokan narasi bukan bukti pemenuhan**.
6. Gunakan Word/PDF untuk ekspor laporan, JSON untuk backup, dan **Reset Data** untuk kasus baru.

## Cara memasang pada GitHub Pages
Buat repository baru, unggah semua berkas dalam paket ke root repository, lalu pada Settings → Pages pilih Deploy from a branch → main / root.

## Metode dan batasan
- Mesin berbasis aturan deterministik, bukan model AI bahasa yang mengerti penuh konteks atau sistem verifikasi dokumen legal.
- Nomor FED menjadi dasar pemetaan; pencarian tanpa nomor adalah kandidat yang harus dikonfirmasi.
- Skor 1/2 pada naratif hanya indikasi ketika unsur tertentu tertangkap bersama petunjuk sumber; bukan skor final asesor. Skor 0 tidak ditarik dari ketiadaan teks.
- Pada lima syarat perlu, angka yang diperiksa adalah **input pengguna** dan tidak diambil secara tak terkendali dari seluruh PDF.
- RIPK dihitung sebagai rerata tertimbang berdasarkan jumlah lulusan per tahun dari input. Rekonsiliasikan definisi perhitungan dengan formulir instrumen.
- Tracer study memeriksa ambang respon dan persentase kesesuaian. Jika respon kurang dari minimum, nilai belum ditetapkan karena memerlukan ketentuan penyesuaian resmi.
- Keanggotaan dihitung per DPRPS unik dengan bukti masih berlaku, bukan jumlah kartu sertifikat.
- Laboratorium harus memenuhi lima unsur dengan bukti pemeriksaan, bukan sekadar disebut dalam FED.
- Data kasus contoh dari berkas pengguna **tidak terdapat** dalam HTML/ZIP. Data diproses dan disimpan di browser; jangan unggah JSON backup yang berisi data institusi ke repositori publik.
- Footer aplikasi: **@ramalabs**.

## Rujukan
Matriks Penilaian Unggul Sarjana dalam berkas `14_IAPS-2.0-Unggul_Sarjana`, Pedoman Memahami IAPS 2.0, dan materi pelatihan asesor yang disediakan pengguna. Selalu konfirmasi instrumen dan tahun asesmen yang berlaku sebelum menetapkan nilai resmi.
