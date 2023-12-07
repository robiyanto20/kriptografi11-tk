

---

# Steganografi Gambar dengan LSB (Least Significant Bit)

Kode ini adalah contoh sederhana dari penggunaan steganografi menggunakan metode LSB pada gambar. LSB memungkinkan kita untuk menyembunyikan data ke dalam gambar tanpa mengubah penampilannya secara signifikan.

## Cara Menggunakan

### Langkah 1: Menyembunyikan Data

1. Ganti nilai `data_to_hide` dengan data yang ingin Anda sembunyikan dalam gambar.
2. Pastikan gambar yang ingin Anda gunakan untuk menyembunyikan data memiliki nama dan path yang sesuai di dalam kode (`lsb.hide("gambar.png", data_to_hide)`). Pastikan juga gambar sudah ada di direktori yang sama dengan kode.
3. Jalankan kode.
4. Gambar hasil steganografi akan disimpan dengan nama `"gambar2.png"` di direktori yang sama.

### Langkah 2: Mengungkap Data Tersembunyi

1. Gunakan gambar `"gambar2.png"` yang telah disimpan untuk mengungkap data tersembunyi.
2. Jalankan kode dan periksa output yang akan menampilkan data yang berhasil diungkapkan.

Pastikan untuk mengganti nama gambar, memasukkan data yang ingin disembunyikan, dan memeriksa hasilnya sesuai kebutuhan Anda.
