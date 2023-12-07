

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

---

Untuk membuat README yang bagus untuk kode tersebut di GitHub, ada beberapa poin yang perlu dijelaskan:

---

## Steganografi dengan Penggunaan One-Time Pad

Ini adalah kode Python yang memanfaatkan steganografi dan enkripsi One-Time Pad (OTP) untuk menyembunyikan dan mengungkap pesan rahasia pada gambar.

### Deskripsi Singkat

Kode ini mengizinkan pengguna untuk:

- **Menyembunyikan Pesan**: Memasukkan pesan teks dan kunci untuk menyembunyikannya dalam gambar.
- **Mengungkap Pesan Tersembunyi**: Mencoba mengungkap pesan yang disembunyikan dari gambar steganografi yang dihasilkan.

### Langkah-langkah

1. **Kompress dan Enkripsi Pesan**: Pesan teks dimampatkan menggunakan zlib, kemudian dienkripsi dengan kunci OTP yang dimasukkan pengguna.
2. **Konversi Data**: Pesan terkompresi dikonversi menjadi data biner.
3. **Penyembunyian**: Data biner disematkan dalam gambar menggunakan teknik Steganografi LSB (Least Significant Bit).
4. **Revealing**: Usaha untuk mengungkapkan pesan tersembunyi dari gambar steganografi yang dihasilkan.
   
### Cara Penggunaan

1. Pengguna diminta untuk memasukkan pesan yang akan disembunyikan dan kunci OTP.
2. Kunci dikonfirmasi untuk memastikan kesesuaian.
3. Gambar awal dan gambar setelah penyembunyian akan ditampilkan.
4. Proses mencoba untuk mengungkapkan pesan tersembunyi.

### Catatan Penting

- Pastikan gambar yang diinginkan ada dan dinamai `pi.png`.
- Penggunaan kunci yang benar-benar identik penting dalam pengungkapan pesan tersembunyi.

### Dependencies

- `stegano`: Untuk menyembunyikan dan mengungkap data dalam gambar.
- `PIL`: Untuk manipulasi gambar.

### Cara Menjalankan

Pastikan untuk menginstal dependency yang dibutuhkan terlebih dahulu. Kemudian jalankan script dengan Python 3.

```bash
pip install stegano
pip install pillow
python nama_script.py
```

### Contoh Penggunaan

Input Pesan:
```
Hello, this is a hidden message!
```

Input Kunci:
```
MySecretKey123
```

---

