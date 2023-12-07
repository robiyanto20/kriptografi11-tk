Steganografi dengan Metode LSB (Least Significant Bit)
Kode ini merupakan contoh implementasi steganografi menggunakan metode LSB (Least Significant Bit) dengan menggunakan Python dan pustaka Stegano.

Deskripsi
Kode ini digunakan untuk menyembunyikan pesan teks di dalam gambar dengan memanfaatkan metode LSB. LSB merupakan teknik yang memanfaatkan bit terkecil (bit paling tidak signifikan) dari setiap byte dalam data gambar untuk menyimpan informasi tambahan tanpa secara signifikan mengubah tampilan visual gambar.

Langkah-langkah yang Dilakukan:
Persiapan Pesan Teks
Pesan teks yang akan disembunyikan dapat diubah pada bagian data_to_hide = "ROBIYANTO 312210098.". Silakan ganti bagian ini dengan pesan teks yang diinginkan.

Menyembunyikan Pesan Teks
Menggunakan metode LSB dari pustaka Stegano, pesan teks akan disisipkan ke dalam gambar yang telah ditentukan (gambar.png) pada bagian secret = lsb.hide("gambar.png", data_to_hide).

Menyimpan Gambar Hasil Steganografi
Gambar hasil penyisipan pesan disimpan dengan nama gambar2.png menggunakan perintah secret.save("gambar2.png").

Mengungkapkan Pesan Tersembunyi
Proses pengungkapan pesan tersembunyi dilakukan dengan membaca gambar yang telah dimodifikasi sebelumnya menggunakan perintah revealed_data = lsb.reveal("gambar2.png"). Jika berhasil, pesan teks tersembunyi akan ditampilkan.

Penggunaan
Pastikan Anda telah menginstal pustaka Stegano dengan perintah pip install stegano.

Ubah pesan teks yang ingin Anda sembunyikan pada bagian data_to_hide.

Jalankan kode ini di lingkungan Python.
