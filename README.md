Dataset Putusan Pengadilan PN Raba Bima – Kasus Narkotika dan Psikotropika

Deskripsi Umum
Dataset ini berisi kumpulan putusan pengadilan negeri (PN) Raba Bima yang berkaitan dengan tindak pidana Narkotika. 
Dokumen diambil dari sumber terbuka putusan3.mahkamahagung.go.id yang merupakan portal resmi publikasi putusan Mahkamah Agung Republik Indonesia.

Tujuan dari dataset ini adalah untuk mendukung penelitian di bidang Natural Language Processing (NLP), 
Information Retrieval (IR), dan Text Mining Hukum, khususnya dalam menganalisis pola dan tren.

Struktur Data Set
Dataset disimpan dalam format Excel dengan kolom-kolom berikut:

Kolom	:                               Deskripsi:
Nomor_putusan	                        Nomor resmi putusan pengadilan (misal: 123/Pid.Sus/2023/PN Rbi)
Lembaga Peradilan                     Nama lembaga peradilan yang mengeluarkan putusan (misal: PN Raba Bima)
Barang_bukti	                        Daftar barang bukti yang disita
Amar_putusan	                        Hasil akhir putusan (contoh: pidana penjara, denda, rehabilitasi)

Proses Pengumpulan dan Preprosesing
1. Pengumpulan Data
   - Data dikumpulkan dari situs putusan3.mahkamahagung.go.id
   - menggunakan kata kunci “Narkotika” dan “Psikotropika” pada wilayah PN Raba Bima.
   - Setiap putusan diunduh, disimpan, dan dilalukan rangkuman putusan sesuai sama struktur
     kolom (seperti: Nomor_putusan, Lembaga Peradilan, Barang_bukti Amar_putusan)	dan dikonversi di ke format excel.

2. Praeprosesing Data
   - Pembersihan teks dari URL, hapus angka, simbol,dan tanda baca yang tidak relevan.
   - Normalisasi teks: huruf kecil, penghapusan spasi berlebih, dan penghilangan kata tak bermakna.
   - Ekstraksi bagian penting seperti barang bukti dan amar putusan dengan regex atau segmentasi teks.
   - TF-IDF Vectorization + Indexing dan VISUALISASI SIMILARITY
  
Etika dan Lisensi Penggunaan
- Dataset ini bersumber dari dokumen publik resmi Mahkamah Agung RI.
- Tidak mengandung data pribadi sensitif di luar yang telah dipublikasikan secara sah.
- Hanya digunakan untuk keperluan akademik, penelitian, dan pembelajaran.
- Tidak untuk kepentingan komersial atau distribusi ulang tanpa izin.

Atribusi:
Sumber Data: Mahkamah Agung RI – Direktori Putusan
URL: https://putusan3.mahkamahagung.go.id
