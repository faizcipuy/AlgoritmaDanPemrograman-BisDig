#Penjelasan no 1
Program ini dibuat untuk menghitung diskon belanja dan menentukan jumlah yang harus dibayar setelah diskon diterapkan. Diskon hanya diberikan jika total belanja lebih dari Rp500.000.

Penjelasan Alur Kode:

1. Fungsi hitung_total_setelah_diskon(total_belanja)

Fungsi ini menerima nilai total belanja dari pengguna, lalu menghitung:

Jika belanja lebih dari Rp500.000, maka pembeli dapat diskon 10%.

Contoh: Belanja Rp600.000 → diskon 10% = Rp60.000 → total bayar = Rp540.000

Jika tidak lebih dari Rp500.000, maka tidak dapat diskon, dan total bayar tetap seperti total belanja.

Hasil dari fungsi ini adalah dua nilai sekaligus:

total_bayar: jumlah yang harus dibayar setelah diskon

diskon: jumlah potongan yang didapat

Kenapa pakai fungsi?
Supaya logika penghitungan diskon dipisah dari bagian input/output. Ini bikin program:

Lebih rapi

Lebih mudah dibaca dan dipelihara

Bisa digunakan ulang di tempat lain (misalnya untuk toko online, kasir, dll)

2. Bagian Input:

Pengguna diminta memasukkan total belanja lewat keyboard:

Masukkan total belanja (Rp):

Nilai input dikonversi jadi float supaya bisa menerima angka desimal, misalnya Rp521.500.

3. Pemanggilan Fungsi & Proses:

Program memanggil fungsi hitung_total_setelah_diskon(total_belanja)
dan menyimpan hasilnya di dua variabel: total_bayar dan diskon.

4. Menampilkan Hasil ke Layar:

Program mencetak:

Berapa besar diskon yang didapat

Berapa total yang harus dibayar setelah diskon

Gunakan format :,.0f supaya:

Angka ditampilkan dengan titik ribuan (contoh: Rp540.000)

Tanpa angka desimal (bulat) 

#Penjelasan no 2
Tujuan Program:

Program ini dibuat untuk menghitung faktorial dari sebuah angka yang dimasukkan oleh pengguna. Faktorial adalah hasil perkalian semua bilangan bulat dari 1 sampai angka itu sendiri.

Contoh:

5! = 5 × 4 × 3 × 2 × 1 = 120

Penjelasan Alur Program:

1. Fungsi faktorial(n):

Fungsi ini menggunakan rekursi, yaitu memanggil dirinya sendiri untuk menyelesaikan masalah.

Kalau n adalah 0 atau 1, langsung dikembalikan 1. Ini karena:

0! = 1 (definisi matematis)
1! = 1

Kalau n lebih dari 1, maka:

Misalnya faktorial(4) → hasilnya adalah 4 * faktorial(3)

faktorial(3) → 3 * faktorial(2)

dan seterusnya sampai ke faktorial(1) yang nilainya 1.

Setelah itu, hasilnya akan dihitung balik ke atas, seperti tumpukan.

Kenapa pakai rekursi?
Karena faktorial punya sifat alami yang cocok dengan rekursi:
n! = n × (n-1)!. Jadi pendekatannya elegan dan langsung mengikuti rumus matematika.

2. Input dari Pengguna:

Pengguna diminta memasukkan sebuah angka bulat (int), misalnya 5.

3. Pengecekan Angka Negatif:

Karena faktorial tidak didefinisikan untuk angka negatif, maka program memeriksa:

Jika angka < 0, tampilkan pesan peringatan.

Kalau tidak (berarti 0 atau positif), lanjut ke langkah berikutnya.

4. Menghitung dan Menampilkan Hasil:

Program memanggil fungsi faktorial(angka) dan menyimpan hasilnya di variabel hasil.

Kemudian mencetak:

Faktorial dari 5 adalah 120

Kenapa Menggunakan Cara Ini?

Rekursi dipilih karena mencerminkan rumus matematika faktorial secara langsung, jadi kode lebih pendek dan bersih.

Struktur if-else membuat program aman dari input negatif, yang bisa bikin error kalau dihitung faktorialnya.

Pisahkan logika hitung dan input supaya programnya lebih mudah diperluas dan dipahami.

#Penjelasan no 3
Tujuan Program:

Program ini dibuat untuk menghitung faktorial dari sebuah angka yang dimasukkan oleh pengguna. Faktorial adalah hasil perkalian semua bilangan bulat dari 1 sampai angka itu sendiri.

Contoh:

5! = 5 × 4 × 3 × 2 × 1 = 120

Penjelasan Alur Program:

1. Fungsi faktorial(n):

Fungsi ini menggunakan rekursi, yaitu memanggil dirinya sendiri untuk menyelesaikan masalah.

Kalau n adalah 0 atau 1, langsung dikembalikan 1. Ini karena:

0! = 1 (definisi matematis)
1! = 1

Kalau n lebih dari 1, maka:

Misalnya faktorial(4) → hasilnya adalah 4 * faktorial(3)

faktorial(3) → 3 * faktorial(2)

dan seterusnya sampai ke faktorial(1) yang nilainya 1.

Setelah itu, hasilnya akan dihitung balik ke atas, seperti tumpukan.

Kenapa pakai rekursi?
Karena faktorial punya sifat alami yang cocok dengan rekursi:
n! = n × (n-1)!. Jadi pendekatannya elegan dan langsung mengikuti rumus matematika.

2. Input dari Pengguna:

Pengguna diminta memasukkan sebuah angka bulat (int), misalnya 5.

3. Pengecekan Angka Negatif:

Karena faktorial tidak didefinisikan untuk angka negatif, maka program memeriksa:

Jika angka < 0, tampilkan pesan peringatan.

Kalau tidak (berarti 0 atau positif), lanjut ke langkah berikutnya.

4. Menghitung dan Menampilkan Hasil:

Program memanggil fungsi faktorial(angka) dan menyimpan hasilnya di variabel hasil.

Kemudian mencetak:

Faktorial dari 5 adalah 120

Kenapa Menggunakan Cara Ini?

Rekursi dipilih karena mencerminkan rumus matematika faktorial secara langsung, jadi kode lebih pendek dan bersih.

Struktur if-else membuat program aman dari input negatif, yang bisa bikin error kalau dihitung faktorialnya.

Pisahkan logika hitung dan input supaya programnya lebih mudah diperluas dan dipahami.

#Penjelasan no 4
Tujuan Program:

Program ini dibuat untuk:

1. Menerima nilai dari 5 siswa

2. Menyimpan semua nilai itu

3. Menentukan nilai tertinggi

4. Menampilkan siswa ke berapa yang mendapatkan nilai tertinggi

Penjelasan Alur Program:

1. List Kosong untuk Menyimpan Nilai

nilai_siswa = []

Di sini kita membuat wadah kosong (list) untuk menyimpan semua nilai siswa.

Kenapa list? Karena kita akan menyimpan lebih dari satu nilai dan ingin mengaksesnya nanti satu per satu.

2. Perulangan Input untuk 5 Siswa

for i in range(5):
    nilai = float(input(f"Masukkan nilai siswa ke-{i+1}: "))
    nilai_siswa.append(nilai)

Gunakan perulangan for sebanyak 5 kali (range(5)) untuk memasukkan nilai 5 siswa.

input() dipakai untuk menerima nilai dari pengguna.

float() digunakan agar nilai bisa mengandung desimal (misal: 87.5).

.append(nilai) menambahkan nilai itu ke dalam list nilai_siswa.

Kenapa pakai i+1?
Supaya tampilannya lebih alami buat manusia. Kita biasa mulai menghitung dari 1, bukan dari 0.

3. Mencari Nilai Tertinggi

nilai_tertinggi = max(nilai_siswa)

Fungsi max() dipakai untuk mencari angka paling besar di dalam list nilai_siswa.

Ini lebih efisien daripada membandingkan satu per satu.

4. Mencari Posisi Siswa yang Mendapat Nilai Tertinggi

index_tertinggi = nilai_siswa.index(nilai_tertinggi) + 1

.index() mencari posisi (indeks) dari nilai tertinggi di dalam list.

Tambah +1 karena indeks list dimulai dari 0, tapi siswa kita hitung mulai dari 1.

5. Menampilkan Hasil

print(f"Nilai tertinggi adalah {nilai_tertinggi} dan diperoleh oleh siswa ke-{index_tertinggi}")

Hasilnya ditampilkan dalam bentuk kalimat yang langsung memberi tahu:

Nilai tertingginya berapa

Siswa ke berapa yang mendapatkannya

Kenapa Menggunakan Cara Ini?

Pakai list: supaya data bisa disimpan rapi dan diolah bersama-sama

Looping: efisien untuk menangani input yang berulang

Fungsi max() dan .index(): bikin pencarian data spesifik jadi cepat dan otomatis

Modular dan jelas: kode mudah dibaca dan dipahami, bahkan oleh pemula

#PENJELASAN NO 5
Tujuan Program:

Program ini digunakan untuk menghitung total harga dari 3 barang yang dibeli, lalu menampilkan total pembayarannya dalam format rupiah. 

Penjelasan Alur Kode:

1. Menerima Input Harga dari Pengguna

harga1 = float(input("Masukkan harga barang ke-1: "))
harga2 = float(input("Masukkan harga barang ke-2: "))
harga3 = float(input("Masukkan harga barang ke-3: "))

Program meminta pengguna memasukkan harga dari 3 barang satu per satu.

Setiap input dikonversi ke float, karena harga bisa berupa angka desimal (misalnya Rp10.500,50).

Tujuannya agar bisa dihitung secara matematis (misalnya dijumlahkan nanti).

2. Menghitung Total Harga

total = harga1 + harga2 + harga3

Setelah ketiga harga dimasukkan, program menjumlahkannya untuk mendapatkan total belanja.

Disimpan dalam variabel total.

3. Menampilkan Total Pembayaran

print(f"Total harga pembelian adalah: Rp{total:,.2f}")

Menampilkan hasil total harga ke layar dengan format rupiah:

:,.2f digunakan untuk membuat:

Tanda koma sebagai pemisah ribuan

2 angka di belakang koma untuk desimal

Contohnya, jika totalnya adalah 1234567.8, maka tampil sebagai:

Total harga pembelian adalah: Rp1,234,567.80

Kenapa Menggunakan Cara Ini?

Input satu per satu: memudahkan pengguna agar tidak bingung saat memasukkan data.

Tipe float: agar bisa menerima angka desimal, bukan hanya bilangan bulat.

Langsung dijumlahkan: karena hanya ada tiga angka, jadi penjumlahan manual ini sudah cukup dan sederhana.

Format output :,.2f: membuat tampilan lebih rapi dan profesional, layaknya struk belanja.

#Penjelasan no3

