+++
title = 'Luas dan Estimasi Menggunakan Jumlah Berhingga'
date = 2024-03-10T09:16:38+07:00
draft = false
math = true
+++


Dalam catatan singkat "Luas dan Estimasi Menggunakan Jumlah Berhingga," saya ingin membagikan beberapa tips dan pandangan saya tentang bagaimana menghitung luas di bawah kurva menggunakan estimasi. Pertama, penting untuk memahami bahwa luas di bawah kurva dapat dihitung dengan mengaplikasikan konsep jumlah berhingga. Ini berarti membagi area yang ingin dihitung menjadi bagian-bagian kecil yang lebih mudah diukur, kemudian menambahkan luas bagian-bagian tersebut untuk mendapatkan perkiraan luas total.

Langkah pertama dalam melakukan estimasi adalah membagi area di bawah kurva menjadi segmen-segmen kecil (sub-interval) yang lebih sederhana, seperti persegi atau persegi panjang. Selanjutnya, kita menghitung luas masing-masing sub-interval ini menggunakan metode yang lebih sederhana, dengan mengalikan panjang dan lebar. Setelah itu, kita menambahkan luas semua sub-interval tersebut untuk mendapatkan perkiraan luas total di bawah kurva.

Penting untuk diingat bahwa semakin banyak sub-interval yang digunakan dalam estimasi, semakin akurat perkiraan luasnya. Namun, kita juga perlu mempertimbangkan keseimbangan antara akurasi dan kompleksitas perhitungan. Dengan memahami konsep ini, kita dapat menghitung luas di bawah kurva dengan lebih efisien dan akurat menggunakan estimasi.

Jika Anda ingin mengetahui lebih lanjut tentang tips atau pandangan saya dalam menghitung luas di bawah kurva menggunakan estimasi, mari kita jelajahi bersama-sama dalam catatan singkat ini!

Sebelum kita masuk lebih jauh ke dalamnya, ada baiknya saya mengenalkan tiga metode penting dalam perhitungan luas dan estimasi yang akan kita bahas, yakni :

1. Jumlah Atas
2. Jumlah Bawah

Untuk memahami metode-metode tersebut, kita perlu memiliki pemahaman dasar tentang grafik fungsi. Berikut, saya akan memberikan penjelasan singkatnya secara demonstratif.

![Grafik 1.1](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/8a521f95-28c6-4dfa-9a9c-2b0589541415/Untitled.png)

Grafik 1.1

Dalam grafik di atas, kita dapat melihat bahwa lebar suatu kurva direpresentasikan oleh f(x) dan panjangnya direpresentasikan oleh x. Dengan memahami kedua hal ini, kita dapat menghitung luasnya dengan mengalikan x dengan f(x), sehingga luasnya adalah 10 x 5 = 50. Yang ingin saya tegaskan di sini adalah bahwa **f(x) mewakili lebar dan x mewakili panjang**.

Setelah memahami dasar-dasar grafik fungsi, mari kita lanjutkan dengan menghitung luas area menggunakan variasi grafik yang berbeda. Sebelumnya, kita telah melihat grafik konstan; sekarang, mari kita jelajahi beberapa jenis grafik lainnya.

![Grafik 1.2](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/e6b4258c-b000-4c90-b91e-03b2a97074bf/Untitled.png)

Grafik 1.2

![Grafik 1.3](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/73ad204d-d1bc-4814-a6ba-8e40f1301163/Untitled.png)

Grafik 1.3

![Grafik 1.4](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/18932adf-f6e9-49e6-9bb4-1edcc8151264/Untitled.png)

Grafik 1.4

## 1. Jumlah Luas Atas

Untuk memudahkan dalam memahaminya, mari langsung kita coba menggunakan metode dengan menyelesaikan suatu soal.

Contoh Soal 

1. Estimasi luas daerah dibawah kurva menggunakan aturan jumlah atas dengan $4$ bagian dan $8$ bagian pada fungsi $f(x) = 4 - x^2$ pada interval $x = 0$ sampai $x = 2$.

Hal yang diketahui dari soal:

$f(x) = 4 - x^2$

Interval $[a,b]$ = $[0,2]$

$n = 4$ dan $n = 8$

Langkah - Langkah :

1. Tentukan terlebih dahulu panjang sub-interval (panjang persegi) **untuk setiap persegi** dibawah kurva menggunakan : $\Delta x = \frac{a-b}{n}$

Sehingga panjang sub-interval pada soal adalah: 

untuk $n = 4$,  $\Delta x = \frac{2-(0)}{4} = \frac{2}{4} = 0.5$

untuk $n = 8$,  $\Delta x = \frac{2-(0)}{8} = \frac{2}{8} = \frac{1}{4} = 0.25$

1. Visualisasikan (gambarkan) grafik.

Untuk $n = 4$

![Grafik 1.5](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/0a44f486-e64a-4933-bd38-84648e33055b/Untitled.png)

Grafik 1.5

**`TIPS :`**

![Grafik 1.6](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/daf18665-f15c-4737-a97d-530aa053fc79/Untitled.png)

Grafik 1.6

`Terkadang dari kita bingung dalam menentukan menggambar persegi pada grafik secara manual. Untuk itu saya punya tips hanya untuk jumlah atas:`

1. `Gambarkan grafik fungsi seperti Grafik 1.5.` 
2. `Fokuskan pada titik puncak, dalam contoh diatas titik puncak berada pada sisi paling kiri kurva. Maka menggambar sub-interval (persegi) sebanyak 4 dimulai dari titik puncak menuju ke titik terendah.`
3. `Ketahuilah bahwa untuk mencari dimana titik itu memulai panjang persegi adalah dengan memasukkan nilai x kedalam f(x). Pada contoh diatas kita harus memasukkan 4 titik ( **Tidak Boleh Lebih Atau Kurang** ) x kedalam fungsi f(x).`
4. `Pastikan bahwa persegi itu tergambar menembus keluar grafik agar dapat dikatakan **jumlah atas.**`

1. Jumlahkan tiap - tiap luas sub-interval

$\Delta x = \frac{1}{2}$

$c_1 = 0,\ c_2 = \frac{1}{2}, \ c_3 = 1,\ c_4 = \frac{3}{2}$

$L = \Delta x\cdot f(c_1) + \Delta x\cdot f(c_2)+...+ \Delta x\cdot f(c_n)$

$\ \ \ = \frac{1}{2}\cdot f(0) +\frac{1}{2}\cdot f(\frac{1}{2})+\frac{1}{2}\cdot f(1)+\frac{1}{2}\cdot f(\frac{3}{2})$

$\ \ \ = \frac{1}{2}\cdot 4 +\frac{1}{2}\cdot \frac{15}{4}+\frac{1}{2}\cdot 3+\frac{1}{2}\cdot \frac{7}{4}$

$\ \ \ = 6.25$

Jadi, luas daerah dibawah kurva menggunakan aturan jumlah atas dengan $4$ bagian pada fungsi $f(x) = 4 - x^2$ pada interval $x = 0$ sampai $x = 2$ adalah $6.25$

Untuk $n = 8$

![Grafik 1.7](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/2af383b7-8ed6-4fa4-bbea-55c76a8dec52/Untitled.png)

Grafik 1.7

$\Delta x = \frac{1}{4}$

$c_1 = 0,\ c_2 = \frac{1}{8}, \ c_3 = \frac{2}{8}, \ c_4 = \frac{3}{8}, \ c_5 = \frac{4}{8}, \ c_6 = \frac{5}{8}, \ c_7 = \frac{6}{8}, \ c_8 = \frac{7}{8}$

$L = \Delta x\cdot f(c_1) + \Delta x\cdot f(c_2)+...+ \Delta x\cdot f(c_n)$

$\ \ \ = \frac{1}{4}\cdot f(0) +\frac{1}{4}\cdot f(\frac{1}{8})+\frac{1}{4}\cdot f(\frac{2}{8})+\frac{1}{4}\cdot f(\frac{3}{8})+\frac{1}{4}\cdot f(\frac{4}{8})+\frac{1}{4}\cdot f(\frac{5}{8})+\frac{1}{4}\cdot f(\frac{6}{8})+\frac{1}{4}\cdot f(\frac{7}{8})$ 

$\ \ \ = \frac{1}{4}\cdot 4 +\frac{1}{4}\cdot \frac{255}{64}+\frac{1}{4}\cdot \frac{63}{16}+\frac{1}{4}\cdot \frac{247}{64}+\frac{1}{4}\cdot \frac{15}{4}+\frac{1}{4}\cdot \frac{231}{64}+\frac{1}{4}\cdot \frac{55}{16}+\frac{1}{4}\cdot \frac{207}{64}$

$\ \ \ = 5.8125$

Jadi, luas daerah dibawah kurva menggunakan aturan jumlah atas dengan $8$ bagian pada fungsi $f(x) = 4 - x^2$ pada interval $x = 0$ sampai $x = 2$ adalah $5.8125$

## 2. Jumlah Luas Bawah

Untuk memudahkan dalam memahaminya, mari langsung kita coba menggunakan metode dengan menyelesaikan suatu soal.

1. Estimasi luas daerah dibawah kurva menggunakan aturan jumlah bawah dengan $4$ bagian dan $8$  bagian pada fungsi $f(x) = 4 - x^2$ pada interval $x = -2$ sampai $x = 2$.

Hal yang diketahui dari soal:

$f(x) = 4 - x^2$

Interval $[a,b]$ = $[0,2]$

$n = 4$ dan $n = 8$

Langkah - Langkah :

1. Tentukan terlebih dahulu panjang sub-interval (panjang persegi) **untuk setiap persegi** dibawah kurva menggunakan : $\Delta x = \frac{a-b}{n}$

Sehingga panjang sub-interval pada soal adalah: 

untuk $n = 4$,  $\Delta x = \frac{2-(0)}{4} = \frac{2}{4} = 0.5$

untuk $n = 8$,  $\Delta x = \frac{2-(0)}{8} = \frac{2}{8} = \frac{1}{4} = 0.25$

1. Visualisasikan (gambarkan) grafik.

Untuk $n = 4$

![Grafik 1.8](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/88c8ca16-8f5c-4488-b8fe-02fdc6ea8d9d/Untitled.png)

Grafik 1.8

![Grafik 1.9](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/ef899122-fd32-4437-bbc2-fdf697ce436a/Untitled.png)

Grafik 1.9

`TIPS`

`Terkadang dari kita bingung dalam menentukan menggambar persegi pada grafik secara manual. Untuk itu saya punya tips hanya untuk jumlah bawah:`

1. `Gambarkan grafik fungsi seperti Grafik 1.8.` 
2. `Fokuskan pada titik terendah, dalam contoh diatas titik puncak berada pada sisi paling kanan kurva. Maka menggambar sub-interval (persegi) sebanyak 4 dimulai dari titik terendah menuju ke titik puncak.`
3. `Ketahuilah bahwa untuk mencari dimana titik itu memulai panjang persegi adalah dengan memasukkan nilai x kedalam f(x). Pada contoh diatas kita harus memasukkan 4 titik ( **Tidak Boleh Lebih Atau Kurang** ) x kedalam fungsi f(x).`
4. `Pastikan bahwa persegi itu tergambar tidak menembus grafik agar dapat dikatakan **jumlah atas.**`

1. Jumlahkan tiap - tiap luas sub-interval

$\Delta x = \frac{1}{2}$

$c_1 = \frac{1}{2},\ c_2 = \frac{2}{2},\ c_3 = \frac{3}{2},\ c_4 = \frac{4}{2}$

$L = \Delta x\cdot f(c_1) + \Delta x\cdot f(c_2)+...+ \Delta x\cdot f(c_n)$

$\ \ \ = \frac{1}{2}\cdot f(\frac{1}{2})+\frac{1}{2}\cdot f(\frac{2}{2})+\frac{1}{2}\cdot f(\frac{3}{2})+\frac{1}{2}\cdot f(\frac{4}{2})$

$\ \ \ = \frac{1}{2}\cdot \frac{15}{4}+\frac{1}{2}\cdot 3+\frac{1}{2}\cdot \frac{7}{4}+\frac{1}{2}\cdot0$

$\ \ \ = 4.25...$

Jadi, luas daerah dibawah kurva menggunakan aturan jumlah bawah dengan $4$ bagian pada fungsi $f(x) = 4 - x^2$ pada interval $x = 0$ sampai $x = 2$ adalah $4.25...$

Untuk $n = 8$

![Grafik 2.0](https://prod-files-secure.s3.us-west-2.amazonaws.com/3fd570ae-ef42-4f48-8b3f-a3e833c91d04/20e78233-dfd9-4318-9800-665ab76d90fd/Untitled.png)

Grafik 2.0

$\Delta x = \frac{1}{4}$

$c_1 = \frac{1}{8}, \ c_2 = \frac{2}{8}, \ c_3 = \frac{3}{8}, \ c_4 = \frac{4}{8}, \ c_5 = \frac{5}{8}, \ c_6 = \frac{6}{8}, \ c_7 = \frac{7}{8},\ c_8 = \frac{8}{8}$

$L = \Delta x\cdot f(c_1) + \Delta x\cdot f(c_2)+...+ \Delta x\cdot f(c_n)$

$\ \ \ = \frac{1}{4}\cdot f(\frac{1}{8})+\frac{1}{4}\cdot f(\frac{2}{8})+\frac{1}{4}\cdot f(\frac{3}{8})+\frac{1}{4}\cdot f(\frac{4}{8})+\frac{1}{4}\cdot f(\frac{5}{8})+\frac{1}{4}\cdot f(\frac{6}{8})+\frac{1}{4}\cdot f(\frac{7}{8})+\frac{1}{4}\cdot f(\frac{8}{8})$ 

$\ \ \ = \frac{1}{4}\cdot \frac{255}{64}+\frac{1}{4}\cdot \frac{63}{16}+\frac{1}{4}\cdot \frac{247}{64}+\frac{1}{4}\cdot \frac{15}{4}+\frac{1}{4}\cdot \frac{231}{64}+\frac{1}{4}\cdot \frac{55}{16}+\frac{1}{4}\cdot \frac{207}{64}+\frac{1}{4}\cdot 0$

$\ \ \ = 4.8125...$

Jadi, luas daerah dibawah kurva menggunakan aturan jumlah bawah dengan $8$ bagian pada fungsi $f(x) = 4 - x^2$ pada interval $x = 0$ sampai $x = 2$ adalah $4.8125...$

Mari kita jelajahi lebih dalam dan temukan keindahan dalam berbagai jenis grafik yang berbeda. Dengan pemahaman tentang konsep dasar ini, Anda akan memiliki keterampilan yang kuat dalam menghitung luas area di bawah kurva dengan beragam metode. Selamat mengeksplorasi!