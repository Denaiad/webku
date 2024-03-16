+++
title = 'Aritmethic'
date = 2024-03-16T12:42:39+07:00
draft = false
+++

# Arithmetic and Variabels

Halo dan selamat datang di kursus pengantar pemrograman! Kursus ini dirancang khusus untuk kamu yang belum pernah menulis kode sebelumnya, tetapi tertarik untuk mempelajari sains data dan *machine learning* (jika kamu memiliki sedikit pengalaman dalam pemrograman dan baru mengenal bahasa Python, Kursus Python akan menjadi pilihan yang lebih tepat untuk memulai).

Di kursus ini, kamu akan mempelajari cara menggunakan kode untuk memberi perintah kepada komputer untuk melakukan tugas-tugas tertentu. Python, salah satu bahasa pemrograman yang populer dalam bidang sains data, akan menjadi fokus pembelajaranmu di sini. Setelah menyelesaikan kursus ini, kamu akan siap untuk melanjutkan ke kursus Python, dan kemudian kursus pengenalan machine learning.

Dalam tutorial ini, kamu akan diperkenalkan dengan beberapa contoh kode Python. Kamu juga akan diberi kesempatan untuk mencoba menuliskan kode sendiri dalam latihan-latihan yang disediakan. (Jika kamu tertarik dengan latihan-latihan, kamu bisa langsung menuju kesana melalui tautan yang tersedia di akhir tutorial ini).

### Printing

Salah satu tugas yang sederhana (namun sangat penting) adalah meminta komputer untuk mencetak pesan tertentu.

Dalam Python, kita menggunakan fungsi **`print()`** untuk meminta komputer mencetak sebuah pesan. Kita hanya perlu menuliskan pesan tersebut di dalam tanda kurung dan memasukkannya sebagai argumen ke dalam fungsi **`print()`**. Berikut adalah contoh penggunaannya:

```python
print("Hello, World!")
```

Kode di atas ditempatkan dalam sebuah sel kode (disebut sebagai *code cell*), dan komputer akan menampilkan pesan yang diminta di bawah sel tersebut. Seperti yang kamu lihat, komputer mencetak pesan sesuai yang kita inginkan.

### Aritmethic

Selain mencetak pesan, kita juga bisa meminta komputer untuk melakukan beberapa operasi aritmatika seperti penjumlahan, pengurangan, perkalian, atau pembagian.

Misalnya, dalam sel kode berikut, komputer diminta untuk menambahkan 2 dengan 1, dan kemudian mencetak hasilnya, yaitu 3. Perhatikan bahwa ini berbeda dengan mencetak teks atau yang biasa kita sebut dengan string. Saat menggunakan angka, kita tidak memerlukan tanda kutip.

```python
print(1 + 2)
```

Kita juga bisa melakukan pengurangan di Python. Code cell berikut mengurangi 9 dengan 5 dan mencetak hasilnya, yakni 4.

```python
print(9 + 5)
```

Kamu benar-benar dapat melakukan banyak sekali kalkulasi dengan Python! Lihat table berikut untuk beberapa contoh.

| Operasi | Simbol | Contoh |
| --- | --- | --- |
| Penjumlahan | + | 1 + 2 = 3 |
| Pengurangan | - | 5 - 4 = 1 |
| Perkalian | * | 2 * 4 = 8 |
| Pembagian | / | 6 / 3 = 2 |
| Eksponen | ** | 3 ** 2 = 9 |

Kamu bisa mengontrol urutan dari operasi dalam kalkulasi panjang menggunakan tanda kurung.

```python
print((1 + 3) * (9 - 2) / 2) ** 2)
```

Biasanya, Python mengikuti aturan PEMDAS saat menentukan urutan operasi.

### Comments

Kita menggunakan komentar untuk memberikan penjelasan tentang apa yang dilakukan oleh kode. Komentar membantu orang lain memahami kode kamu, dan juga bisa berguna bagi kamu sendiri jika kamu kembali melihat kode yang sudah lama kamu tulis. Sampai saat ini, kode yang sudah kita tulis masih sederhana, tetapi penjelasan menjadi lebih penting saat kita menulis kode yang lebih panjang.

Misalnya, dalam sel kode berikut, kita mengalikan 3 dengan 2. Kami juga menambahkan komentar (**`# Perkalian 3 dengan 2`**) di atas kode untuk menjelaskan apa yang akan dilakukan oleh kode tersebut.

```python
# Perkalian 3 dengan 2
print(3 * 2 )
```

Untuk menandai sebuah baris sebagai komentar (dan bukan kode Python), kamu harus menulis tanda pagar (**`#`**) sebagai karakter pertama. Setelah Python melihat tanda pagar dan mengenali bahwa baris tersebut adalah komentar, komputer akan mengabaikannya sepenuhnya. Hal ini penting, karena sama seperti bahasa Inggris atau Hindi (atau bahasa lainnya!), Python adalah bahasa yang mematuhi aturan dengan ketat. Python lebih ketat daripada pendengaran manusia, dan akan menghasilkan kesalahan jika tidak bisa memahami kode dengan benar.

Kita bisa melihat contoh dari ini dalam sel kode di bawah. Python akan menghasilkan kesalahan (Error) jika kita menghapus tanda pagar, karena teks dalam komentar bukanlah kode Python yang valid, sehingga tidak bisa diinterpretasikan dengan benar.

```python
Perkalian 3 dengan 2
```

```
  File "/tmp/ipykernel_18/3750420471.py", line 1
    Multiply 3 by 2
             ^
SyntaxError: invalid syntax
```

### Variabel

Sejauh ini, kita telah menggunakan kode untuk melakukan perhitungan dan mencetak hasilnya, tetapi hasil tersebut tidak disimpan. Namun, kamu mungkin ingin menyimpan hasilnya untuk digunakan nanti. Untuk ini, kamu akan menggunakan variabel.

### Membuat Variabel

Sel di kode berikutnya membuat sebuah variabel yang disebut **`var_test`** dan menetapkan nilainya sebagai hasil penjumlahan 5 dan 4.

Kita akan mencetak nilai yang ditetapkan pada variabel tersebut, yaitu 9.

```python
# Membuat sebuah variabel dengan nama var_tes dan
# menetapkan nilainya dari 4 + 5
var_tes = 4 + 5

# Mencetak nilai dari var_test
print(var_tes)
```

Umumnya, saat bekerja dengan variabel, kamu harus memilih nama yang ingin kamu gunakan. Nama variabel sebaiknya singkat dan deskriptif. Variabel juga harus memenuhi beberapa persyaratan:

- Variabel tidak boleh mengandung spasi (misalnya, **`var test`** tidak diperbolehkan)
- Variabel hanya boleh terdiri dari huruf, angka, dan garis bawah (misalnya, **`var_test!`** tidak diperbolehkan)
- Variabel harus dimulai dengan huruf atau garis bawah (misalnya, **`1_var`** tidak diperbolehkan)

Kemudian, untuk membuat variabel, kamu harus menggunakan tanda sama dengan (**`=`**) untuk menetapkan nilai yang kamu inginkan.

Kamu selalu bisa melihat nilai yang ditetapkan pada variabel dengan menggunakan fungsi **`print()`** dan menempatkan nama variabel di dalamnya.

Seiring berjalannya waktu, kamu akan belajar cara memilih nama variabel yang baik untuk Python. Pada awalnya, mungkin akan terasa sedikit tidak nyaman, tetapi cara terbaik untuk belajar adalah dengan melihat banyak contoh kode Python.

### Memanipulasi Variabel

Kamu selalu bisa mengubah nilai yang ditetapkan pada sebuah variabel dengan menimpanya dengan nilai baru.

Dalam sel kode berikut, kita mengubah nilai variabel **`var_ku`** dari 3 menjadi 100.

```python
# Menerapkan nilai variabel baru dengan 3
var_ku = 3

# Cetak (print) nilai yang ditetapkan pada var_ku
print(var_ku)

# Mengubah nilai variabel dengan 100
var_ku = 100

# Cetak (print) nilai yang ditetapkan pada var_ku
print(var_ku)
```

```
3
100
```

Perhatikan bahwa secara umum, apa pun yang kamu definisikan sebagai variabel dalam sebuah sel kode, semua sel kode berikutnya juga memiliki akses ke variabel tersebut. Misalnya, kita menggunakan sel kode berikut untuk mengakses nilai dari **`var_ku`** (dari sel kode sebelumnya) dan **`var_test`** (dari awal tutorial ini).

```python
print(var_ku)
print(var_tes)
```

```
100
9
```

Selanjutnya, sel kode memberi tahu Python untuk menambahkan nilai variabel **`var_ku`** saat ini sebesar 3.

Untuk melakukan hal ini, kita menggunakan **`var_ku =`** seperti sebelumnya. Dan juga seperti sebelumnya, nilai baru yang ingin kita tetapkan pada variabel berada di sebelah kanan tanda sama dengan (**`=`**).

```python
# Meningkatkan nilai dengan 3
var_ku = var_ku + 3

# Print nilai yang ditetapkan pada var_ku
print(var_ku)
```

```
103
```

### Menggunakan banyak variabel

Dalam banyak kasus, penggunaan banyak variabel adalah hal yang umum. Hal ini berguna terutama ketika kita memiliki perhitungan panjang dengan banyak input variabel.

Dalam sel kode berikutnya, kita menghitung jumlah detik dalam empat tahun. Perhitungan ini menggunakan lima input variabel.

```python
# Membuat variabel
bil_tahun = 4
hari_per_tahun = 365
jam_per_hari = 24
menit_per_jam = 60
detik_per_menit = 60

# Menghitung bilangan detik dalam empat tahun
detik_total = detik_per_menit * menit_per_jam *jam_per_hari * hari_per_tahun * bil_tahun
print(detik_total)

```

```
126144000
```

Dengan demikian, terdapat 126,144,000 detik dalam empat tahun.

Perhatikan bahwa menggunakan variabel memungkinkan kita untuk melakukan perhitungan tanpa variabel seperti hanya **`60 * 60 * 24 * 365 * 4`**, tetapi akan lebih sulit untuk memastikan bahwa perhitungan tanpa variabel tersebut tidak memiliki kesalahan, karena lebih sulit dibaca. Ketika kita menggunakan variabel (seperti **`bil_tahun`**, **`hari_per_tahun`**, dan lainnya), kita dapat melacak bagian-bagian dari perhitungan tersebut lebih mudah, dan lebih mudah untuk memeriksa dan memperbaiki kesalahan.

Perhatikan juga bahwa menggunakan variabel menjadi sangat berguna ketika nilai input dapat berubah. Misalnya, katakanlah kita ingin memperbarui sedikit estimasi dengan mengubah nilai jumlah hari dalam setahun dari 365 menjadi 365.25, untuk memperhitungkan tahun kabisat. Kemudian kita hanya perlu mengubah nilai yang ditetapkan pada **`hari_per_tahun`** tanpa harus mengubah variabel lain dan melakukan perhitungan kembali.

```python
# Update untuk menyertakan tahun kabisat
hari_per_tahun = 366.25

# Menghitung bilangan detik dalam empat tahun
detik_total = detik_per_menit * menit_per_jam *jam_per_hari * hari_per_tahun * bil_tahun
print(detik_total)
```

```
126230400.0
```

**Catatan:** Kamu mungkin melihat **`.0`** ditambahkan pada akhir angka, yang mungkin terlihat tidak diperlukan. Hal ini disebabkan oleh fakta bahwa dalam perhitungan kedua, kita menggunakan angka dengan pecahan (365.25), sedangkan dalam perhitungan pertama kita mengalikan dengan angka bulat. Lebih lanjut tentang hal ini akan kamu pelajari pada materi 3, ketika kita membahas tipe data.

### Debugging

Salah satu kesalahan yang umum terjadi ketika menggunakan variabel adalah kesalahan pengetikan. Misalnya, jika kita menuliskan **`jam_per_hari`** sebagai **`jm_per_hari`**, Python akan menghasilkan pesan kesalahan **`NameError: name 'jm_per_hari' is not defined`**.

```python
print(jm_per_hari)
```

```python
--------------------------------------------------------------------------
NameError Traceback (most recent call last)
/tmp/ipykernel_18/142450907.py in <module>
----> 1 print(jm_per_hari)

NameError: name 'jm_per_hari' is not defined
```

Ketika kamu melihat **`NameError`** seperti ini, itu menunjukkan bahwa kamu perlu memeriksa pengejaan variabel yang diacu sebagai "tidak didefinisikan". Untuk memperbaiki kesalahan tersebut, kamu hanya perlu memperbaiki pengejaannya..
