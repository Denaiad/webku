+++
title = 'Integral Trigonometri'
date = 2024-03-17T07:03:57+07:00
draft = false
math = true
katex = true
+++

Dalam bagian ini kita akan melihat beberapa integral fungsi trigonometri dan beberapa teknik yang bisa kita gunakan untuk membantu memecahkannya. Mari kita coba dengan sebuah integral yang kita seharusnya telah bisa melakukannya.

$$
\begin{align*}
\int \sin{x}\cos{x} &= \int u^5 du && \text{menggunakan substitusi u = sin(x)}\\
                    &= \frac{1}{6}\sin^{6}(x)+c
\end{align*}
$$

Integral ini mudah dilakukan dengan substitusi karena adanya cosinus, namun, bagaimana dengan integral berikut.

$$
\begin{align*}
\text{Contoh 1 Hitung integral berikut ini}: \
\int sin^{5}x \ dx
\end{align*}
$$

- Solution
    
    Integral ini tidak lagi memiliki cosinus di dalamnya yang memungkinkan kita untuk menggunakan substitusi yang kita gunakan di atas. Oleh karena itu, substitusi tersebut tidak akan berhasil dan kita harus mencari cara lain untuk melakukan integral ini.
    
    Pertama-tama, mari kita perhatikan bahwa kita dapat menulis integral sebagai berikut
    
    $$
    \begin{align*}
        \int sin^{5}x\ dx = \int sin^{4}x\sin{x}\ dx =\int (sin^{2}x)^2\ dx
    \end{align*}
    $$
    
    Sekarang ingat kembali identitas trigonometri,
    
    $$
    \begin{align*}
    \cos^2{x} + \sin^2{x} = 1 \implies \sin^2{x} = 1 - cos^2{x}
    \end{align*}
    $$
    
    Sekarang ingat kembali identitas trigonometri,
    
    $$
    \begin{align*}
    \int{\sin^5{x}\ dx} = \int{(1-\cos^2{x})^2} \sin{x}\ dx
    \end{align*}
    $$
    
    dan sekarang kita dapat menggunakan substitusi $u = \cos{x}$. Dengan melakukan hal ini, kita akan mendapatkan,
    
    $$
    \begin{align*}
    \int{\sin^5{x}\ dx} &= -\int{(1-u^2)^2 \ du} \\
    &= -\int{1 - 2u^2 + u^4 \ du} \\
    &= -\left(u + \dfrac{2}{3}\ u^3 + \dfrac{1}{5}\ u^5 + c \right) \\
    &= -\cos{x} + \dfrac{2}{3}\ \cos^3{x} - \dfrac{1}{5}\ \cos^5{x} + c
    \end{align*}
    $$
    
    Jadi, dengan sedikit penulisan ulang pada integrand, kami dapat menguranginya menjadi substitusi yang cukup sederhana.
    

Perhatikan bahwa kita dapat melakukan penulisan ulang yang kita lakukan pada contoh sebelumnya karena eksponen pada sinus ganjil. Dalam kasus ini, yang perlu kita lakukan adalah menghilangkan salah satu sinus. Eksponen pada sinus yang tersisa akan menjadi genap dan kita dapat dengan mudah mengubah sinus yang tersisa menjadi cosinus menggunakan identitas,

$$
\begin{align}
\cos^2{x} + \sin^2{x} = 1
\end{align}
$$

Jika eksponen pada sinus adalah genap, hal ini akan sulit dilakukan. Kita dapat menghilangkan satu sinus, tetapi sinus yang tersisa akan memiliki eksponen ganjil dan meskipun kita dapat mengubahnya menjadi cosinus, integral yang dihasilkan sering kali lebih sulit daripada integral aslinya dalam banyak kasus.

$$
\begin{align*}
\text{Contoh 2 Hitung integral berikut ini}: \
\int sin^6{x} \cos^3{x} \ dx
\end{align*}
$$

- Solution
    
    Jadi, dalam kasus ini kita memiliki sinus dan kosinus dalam soal, dan dalam hal ini eksponen pada sinus genap sedangkan eksponen pada kosinus ganjil. Jadi, kita dapat menggunakan teknik yang sama dalam integral ini. Kali ini kita akan menghilangkan kosinus dan mengubah sisanya menjadi sinus
    
    $$
    \begin{align*}
    \int{\sin^6{x}\cos^3{x}\ dx} &= \int{\sin^6{x}\cos^2{x}\cos{x}\ dx}\\
    &= \int{sin^6{x}\ (1-\sin^2{x})\cos{x}\ dx} &&&&& \text{u = sin x} \\
    &= \int{u^6 (1-u^2)\ du}\\
    &= \int{u^6-u^8 \ du}\\
    &= \dfrac{1}{7}\sin^7{x} - \dfrac{1}{9}\sin^9{x}+c
    \end{align*}
    $$
    

Pada titik ini, mari kita berhenti sejenak untuk meringkas apa yang telah kita pelajari sejauh ini tentang mengintegrasikan pangkat sinus dan kosinus

$$
\begin{align*}
\int{\sin^n{x}\cos^m{x}\ dx} \tag 2
\end{align*}
$$

Dalam integral ini jika eksponen pada sinus $(n)$ ganjil, kita dapat menghilangkan satu sinus, mengubah sisanya menjadi cosinus menggunakan $(1)$  dan kemudian gunakan substitusi $u = \cos(x)$. Demikian juga, jika eksponen pada kosinus $(m)$  ganjil, kita dapat menghilangkan satu kosinus dan mengubah sisanya menjadi sinus dan menggunakan substitusi $u = \sin(x)$.

Tentu saja, jika kedua eksponennya ganjil, maka kita dapat menggunakan salah satu metode. Namun, dalam kasus ini biasanya lebih mudah untuk mengonversi suku dengan eksponen yang lebih kecil.

Satu kasus yang belum kita bahas adalah apa yang terjadi jika kedua eksponennya genap? Dalam kasus ini, teknik yang kita gunakan pada beberapa contoh pertama tidak akan berhasil dan pada kenyataannya tidak ada satu metode yang pasti untuk melakukan integral ini. Setiap integral berbeda dan dalam beberapa kasus akan ada lebih dari satu cara untuk melakukan integral.

Dengan demikian, sebagian besar, jika tidak semua, integral yang melibatkan produk sinus dan kosinus di mana kedua eksponennya genap dapat dilakukan dengan menggunakan satu atau lebih rumus berikut untuk menulis ulang integrand

$$
\begin{align*}
\cos^2{x}&=\dfrac{1}{2}(1+\cos{(2x)})\newline
\sin^2{x}&=\dfrac{1}{2}(1-\cos{(2x)})\newline
\sin{x}\cos{x}&=\dfrac{1}{2}\sin{(2x)}
\end{align*}
$$

Dua rumus pertama adalah rumus sudut setengah standar dari kelas trigonometri yang ditulis dalam bentuk yang akan lebih nyaman untuk kita gunakan. Yang terakhir adalah rumus sudut ganda standar untuk sinus, sekali lagi dengan sedikit penulisan ulang.

Mari kita lihat sebuah contoh

$$
\begin{align*}
\text{Contoh 3 Hitung integral berikut ini}: \
\int \sin^2{x}\cos^2{x}\  dx
\end{align*}
$$

- Solution
    
    Seperti yang telah disebutkan di atas, sering kali ada lebih dari satu cara untuk melakukan integral yang kedua eksponennya genap. Integral ini adalah salah satu contohnya. Setidaknya ada dua teknik penyelesaian untuk masalah ini. Kita akan melakukan kedua solusi tersebut dimulai dengan yang mungkin lebih panjang dari keduanya, tetapi juga yang paling sering digunakan oleh banyak orang.
    
    *Solusi 1*
    Dalam solusi ini kita akan menggunakan dua rumus setengah sudut di atas dan hanya mengganti mereka ke dalam integral
    
    $$
    \begin{align*}
    \int{\sin^2{x}\cos^2{x}\ dx} &= \int{\dfrac{1}{2}(1-\cos{(2x)})\left(\frac{1}{2}\right)(1+\cos{(2x)})\ dx} \newline
    &= \dfrac{1}{4} \int{1-\cos^2{(2x)} \ dx}
    \end{align*}
    $$
    
    Jadi, kita masih memiliki integral yang tidak dapat diselesaikan sepenuhnya, namun perhatikan bahwa kita telah berhasil mengurangi integral menjadi hanya satu suku yang menyebabkan masalah (kosinus dengan pangkat genap) daripada dua suku yang menyebabkan masalah.
    
    Sebenarnya untuk menghilangkan sisa istilah masalah yang perlu kita lakukan adalah menggunakan kembali rumus setengah sudut pertama yang diberikan di atas
    
    $$
    \begin{align*}
    \int{\sin^2{x}\cos^2{x}\ dx} &=\dfrac{1}{4}\int{1-\dfrac{1}{2}(1+\cos{(4x)}) \ dx}\newline
    &= \dfrac{1}{4} \int{\dfrac{1}{2}-\dfrac{1}{2}\cos{(4x)} \ dx}\newline
    &= \dfrac{1}{4}\left(\dfrac{1}{2}x-\dfrac{1}{8}\sin{(4x)}\right)+c\newline
    &= \dfrac{1}{8}x - \dfrac{1}{32}\sin{(4x)}+c
    \end{align*}
    $$
    
    Jadi, solusi ini membutuhkan total tiga identitas trigonometri untuk menyelesaikannya.
    
    *Solusi 2*
    Pada solusi ini kita akan menggunakan rumus sudut ganda untuk membantu menyederhanakan integral sebagai berikut.
    
    $$
    \begin{align*}
    \int{\sin^2{x}\cos^2{x}\ dx} &=\int{(\sin{x}\cos{x})^2\ dx}\newline
    &= \int{\left(\dfrac{1}{2}\sin{(2x)}\right)^2\ dx}\newline
    &= \dfrac{1}{4}\int{\sin^2{(2x)}\ dx}
    \end{align*}
    $$
    
    Sekarang, kita menggunakan rumus setengah sudut untuk sinus untuk mengurangi menjadi integral yang dapat kita lakukan.
    
    $$
    \begin{align*}
    \int{\sin^2{x}\cos^2{x}\ dx} &=\dfrac{1}{8}\int{1-\cos{(4x)}\ dx}\newline
    &= \dfrac{1}{8}x-\dfrac{1}{32}\sin{(4x)}+c
    \end{align*}
    $$
    
    Metode ini hanya membutuhkan dua identitas trigonometri untuk menyelesaikannya.
    
    Perhatikan bahwa perbedaan antara kedua metode ini lebih kepada "kekacauan". Metode kedua tidak jauh lebih mudah (selain membutuhkan satu identitas trigonometri yang lebih sedikit), metode ini tidak terlalu berantakan dan sering kali diterjemahkan ke dalam proses yang "lebih mudah".
    

Pada contoh sebelumnya, kita telah melihat dua metode solusi berbeda yang memberikan jawaban yang sama. Perhatikan bahwa hal ini tidak selalu terjadi. Bahkan, lebih sering kita akan mendapatkan jawaban yang berbeda. Namun, seperti yang telah kita bahas pada bagian Integrasi per Bagian, kedua jawaban tersebut tidak akan berbeda lebih dari sebuah konstanta.

Secara umum, ketika kita memiliki hasil kali sinus dan cosinus di mana kedua eksponennya genap, kita perlu menggunakan serangkaian rumus setengah sudut dan / atau sudut ganda untuk mengurangi integral ke dalam bentuk yang dapat kita integrasikan. Selain itu, semakin besar eksponennya, semakin banyak kita perlu menggunakan rumus-rumus ini dan karenanya semakin berantakan masalahnya.

Terkadang dalam proses mereduksi integral yang kedua eksponennya sama, kita akan menemukan hasil perkalian sinus dan kosinus yang argumennya berbeda. Ini akan membutuhkan salah satu dari rumus berikut untuk mengurangi produk menjadi integral yang dapat kita lakukan.

$$
\begin{align*}
\sin{\alpha}\cos{\beta}&= \dfrac{1}{2}[\sin{(\alpha-\beta)}+\sin{(\alpha+\beta)}]\newline
\sin{\alpha}\sin{\beta}&= \dfrac{1}{2}[\cos{(\alpha-\beta)}-\cos{(\alpha+\beta)}]\newline
\cos{\alpha}\cos{\beta}&= \dfrac{1}{2}[\cos{(\alpha-\beta)}+\cos{(\alpha+\beta)}]\newline
\end{align*}
$$

Mari kita lihat contoh dari salah satu jenis integral ini.

$$
\begin{align*}
\text{Contoh 4 Hitung integral berikut ini}: \
\int \cos{(15x)}\cos{(4x)}\  dx
\end{align*}
$$

- Solution
    
    Integral ini membutuhkan rumus terakhir yang tercantum di atas.
    
    $$
    \begin{align*}
    \int \cos{(15x)}\cos{(4x)}\ dx&= \dfrac{1}{2}\int \cos{(11x)}+\cos{(19x)}\ dx\newline
    &= \dfrac{1}{2}\left(\dfrac{1}{11}\sin{(11x)}+\dfrac{1}{19}\sin{(19x)}\right)+c
    \end{align*}
    $$
    

Oke, pada titik ini kita telah membahas hampir semua kasus yang mungkin terjadi yang melibatkan produk sinus dan kosinus. Sekarang saatnya untuk melihat integral yang melibatkan produk dari sekan dan tangen.

Kali ini, mari kita lakukan sedikit analisis tentang kemungkinannya sebelum kita langsung masuk ke dalam contoh. Integral umumnya adalah,

$$
\begin{align*}
\int \sec^n{x}\tan^m{x}\ dx\tag3
\end{align*}
$$

Hal pertama yang harus diperhatikan adalah kita dapat dengan mudah mengubah pangkat genap dari secant menjadi tangen dan pangkat genap dari tangen menjadi secant dengan menggunakan rumus yang mirip dengan $(1)$. Sebenarnya, rumus tersebut dapat diturunkan dari $(1)$ jadi ayo kita lakukan itu.

$$
\begin{align*}
\cos^2{x} + \sin^2{x} &= 1\newline
\dfrac{\sin^2{x}}{\cos^2{x}}+\dfrac{\cos^2{x}}{\cos^2{x}}&= \dfrac{1}{\cos^2{x}}\newline
\tan^2{x}+1&= \sec^2{x} \tag4
\end{align*}
$$

Sekarang, kita akan membahas tentang $(3)$ Sama halnya dengan cara kami menangani $(2)$. Pada akhirnya, kita akan menggunakan salah satu dari substitusi berikut ini.

$$
\begin{align*}
u&=\tan{x} &&&&&& du=\sec^2{x}\ dx\newline
u&=\sec{x} &&&&&& du=\sec{x}\tan{x}\ dx
\end{align*}
$$

Jadi, jika kita menggunakan substitusi $u=\tan{x}$ kita akan membutuhkan dua sekan yang tersisa agar substitusi dapat bekerja. Ini berarti bahwa jika eksponen pada secant $(n)$ bahkan kita dapat menghilangkan dua dan kemudian mengubah sisa sekan menjadi garis singgung menggunakan $(4)$

Selanjutnya, jika kita ingin menggunakan substitusi $u=\sec{x}$  kita akan membutuhkan satu secant dan satu tangen yang tersisa untuk menggunakan substitusi ini. Ini berarti bahwa jika eksponen pada tangen $(m)$ ganjil dan kita memiliki setidaknya satu sekan di integrand, kita dapat menghilangkan salah satu tangen beserta salah satu sekan tentunya. Tangen kemudian akan memiliki eksponen genap sehingga kita dapat menggunakan $(4)$ untuk mengubah tangen lainnya menjadi secant. Perhatikan bahwa metode ini mengharuskan kita untuk memiliki setidaknya satu secant dalam integral. Jika tidak ada secant maka kita perlu melakukan sesuatu yang berbeda.

Jika eksponen pada secant genap dan eksponen pada tangen ganjil, maka kita dapat menggunakan salah satu dari keduanya. Sekali lagi, akan lebih mudah untuk mengonversi suku dengan eksponen terkecil.

Mari kita lihat beberapa contoh.

$$
\begin{align*}
\text{Contoh 5 Hitung integral berikut ini}: \
\int sec^9{x} \tan^5{x} \ dx
\end{align*}
$$

- Solution
    
    Pertama, perhatikan bahwa karena eksponen pada sekawan tidak genap, kita tidak dapat menggunakan substitusi $u=\tan{x}$. Namun, eksponen pada tangen adalah ganjil dan kita memiliki sekan dalam integral sehingga kita akan dapat menggunakan substitusi $u=\sec{x}$. Ini berarti menghilangkan satu tangen (bersama dengan secant)dan mengubah sisa tangen menjadi secant menggunakan $(4)$
    
    $$
    \begin{align*}
    \int sec^9{x} \tan^5{x} \ dx &= \int sec^8{x} \tan^4{x} \tan{x} \sec{x} \ dx \newline
    &= \int sec^8{x}(\sec^2{x}-1)^2\tan{x} \sec{x} \ dx &&&&&& \textit{u = sec {x}} \newline
    &=\int{u^8(u^2-1)^2 \ du} \newline
    &=\int{u^{12}-2u^{10}+u^8 \ du} \newline
    &=\dfrac{1}{13}\sec^{13}{x}-\dfrac{2}{11}\sec^{11}{x}+\dfrac{1}{9}\sec^{9}{x}+c\newline
    \end{align*}
    $$
    

$$
\begin{align*}
\text{Contoh 6 Hitung integral berikut ini}: \
\int sec^4{x} \tan^6{x} \ dx
\end{align*}
$$

- Solution
    
    Jadi, dalam contoh ini pangkat pada tangen adalah genap sehingga substitusi $u = \sec{x}$ tidak akan bekerja. Pangkat pada secant juga genap dan sehingga kita bisa menggunakan substitusi $u = \tan{x}$ untuk integral ini. Yang berarti bahwa kita harus menghilangkan dua secant dan menggantinya menjadi tangen. Ini bekerja untuk integral berikut.
    
    $$
    \begin{align*}
    \int \sec^4{x} \tan^6{x} \ dx &= \int \sec^2{x} \tan^6{x} \sec^2{x} \ dx \newline
    &= \int (\tan^2{x}+1) \tan^6{x} \sec^2{x} \ dx && \textit{u = tan = {x}} \newline
    &=\int{(u^2+1) \ u^6 \ du} \newline
    &=\int{u^{8}+u^{6}\ du} \newline
    &=\dfrac{1}{9}\tan^{9}{x}+\dfrac{1}{7}\tan^{7}{x}c\newline
    \end{align*}
    $$
    

Kedua contoh sebelumnya sangat cocok dengan pola yang dibahas di atas sehingga tidak terlalu sulit untuk diterapkan. Namun, ada beberapa pengecualian pada pola di atas dan dalam kasus ini tidak ada metode tunggal yang dapat digunakan untuk setiap masalah. Setiap integral akan berbeda dan mungkin memerlukan metode penyelesaian yang berbeda untuk mengevaluasi integral tersebut.

Pertama mari kita lihat beberapa integral yang mempunyai eksponen ganjil pada tangen-nya, namun tidak untuk secannya. Dalam kasus ini kita tidak dapat menggunakan substitusi $u = \sec{x}$ karena memerlukan paling sedikit satu secant dalam integralnya

$$
\begin{align*}
\text{Contoh 7 Hitung integral berikut ini}: \
\int \tan{x}\ dx
\end{align*}
$$

- Solution
    
    Untuk melakukan integral ini yang perlu kita lakukan hanyalah mengingat kembali definisi tangen dari segi sinus dan cosinus.
    
    $$
    \begin{align*}
    \int{\tan{x}\ dx} &= \int{\dfrac{\sin{x}}{\cos{x}}\ dx} &&&& \textit{u = cos {x}} \newline
    &= -\int{\dfrac{1}{u}\ du} \newline
    &= -\ln|\cos{x}|+c &&&& r\ln{x} = \ln{x^r}]\newline
    &= \ln{|\cos{x}|^{-1}}+c\newline
    &= \ln{|\sec{x}|}+c
    \end{align*}
    $$
    
    $$
    \begin{align*}
    \int {\tan^3{x}\ dx} &= \int {\tan{x}\tan^2{x}\ dx}\newline
    &= \int {\tan{x}(\sec^2{x}-1)\ dx}\newline
    &= \int {\tan{x}\sec^2{x}\ dx}-\int{\tan{x}\ dx}\newline
    \end{align*}
    $$
    
    Perhatikan bahwa bagi banyak orang,
    
    $$
    \begin{align*}
    \int {\tan^3{x}\ dx} &= \dfrac{1}{2}\tan^2{x}-\ln{|\sec{x}|}+c
    \end{align*}
    $$
    
    Kita melangkah lebih jauh dengan beberapa penyederhanaan. Penyederhanaan tersebut dilakukan semata-mata untuk menghilangkan tanda minus yang ada di depan logaritma. Hal ini tidak harus dilakukan secara umum, namun selalu mudah untuk menghilangkan tanda minus dan dalam hal ini mudah untuk menghilangkannya tanpa menimbulkan kerumitan nyata pada jawabannya dan itulah yang kita lakukan.
    

$$
\begin{align*}
\text{Contoh 8 Hitung integral berikut ini}: \
\int \tan^3{x}\ dx
\end{align*}
$$

- Solution
    
    Caranya adalah dengan melakukan manipulasi integrand berikut ini.
    
    $$
    \begin{align*}
    \int {\tan^3{x}\ dx} &= \int {\tan{x}\tan^2{x}\ dx}\newline
    &= \int {\tan{x}(\sec^2{x}-1)\ dx}\newline
    &= \int {\tan{x}\sec^2{x}\ dx}-\int{\tan{x}\ dx}\newline
    \end{align*}
    $$
    
    Sekarang kita dapat menggunakan substitusi $u = \tan{x}$ pada integral pertama dan hasil dari contoh sebelumnya pada integral kedua. Maka integralnya adalah,
    
    $$
    \begin{align*}
    \int {\tan^3{x}\ dx} &= \dfrac{1}{2}\tan^2{x}-\ln{|\sec{x}|}+c
    \end{align*}
    $$
    

Perhatikan bahwa semua pangkat ganjil tangen (kecuali pangkat pertama) dapat diintegrasikan menggunakan metode yang sama yang kita gunakan pada contoh sebelumnya. Contohnya

$$
\begin{align*}
\int{\tan^5{x}\ dx}&= \int{\tan^3{x}(\sec^2{x}-1)\ dx}&= \int{\tan^3{x}\sec^2{x}\ dx}-\int{\tan^3{x}\ dx}
\end{align*}
$$

Jadi, pergantian yang cepat $(u = \tan{x})$ akan menghasilkan integral pertama dan integral kedua akan selalu pangkat ganjil sebelumnya.

Sekarang mari kita lihat beberapa contoh dimana eksponen pada garis potongnya ganjil dan eksponen pada garis singgungnya genap. Dalam kasus ini, penggantian yang digunakan di atas tidak akan berhasil.

Perlu dicatat juga bahwa kedua integral berikut merupakan integral yang akan kita lihat pada bagian selanjutnya dari bab ini dan bab selanjutnya. Oleh karena itu, bukanlah ide yang buruk untuk mencatat hasil ini sehingga Anda dapat menyiapkannya saat Anda membutuhkannya nanti.

$$
\begin{align*}
\text{Contoh 9 Hitung integral berikut ini}: \
\int \sec{x}\ dx
\end{align*}
$$

- Solution
    
    Yang ini tidak terlalu buruk setelah Anda melihat apa yang harus Anda lakukan. Integral itu sendiri tidak dapat diselesaikan. Namun, jika kita memanipulasi integran sebagai berikut kita bisa melakukannya.
    
    $$
    \begin{align*}
    \int{\sec{x}\ dx} &= \int{\dfrac{\sec{x}(\sec{x}+\tan{x})}{\sec{x}+\tan{x}}\ dx}\newline
    &= \int{\dfrac{\sec^2{x}+\tan{x}\sec{x}}{\sec{x}+\tan{x}}\ dx}
    \end{align*}
    $$
    
    Dalam bentuk ini kita dapat mengerjakan integral dengan menggunakan substitusi $u = \sec{x} + \tan{x}$. Melakukan hal ini memberi,
    
    $$
    \begin{align*}
    \int {\sec{x}\ dx} &= \ln{|\sec{x}+\tan{x}|}+c
    \end{align*}
    $$
    

Ide yang digunakan dalam contoh di atas adalah ide bagus untuk diingat. Mengalikan pembilang dan penyebut suatu suku dengan suku yang sama di atas terkadang dapat menghasilkan integral yang dapat diintegralkan. Perhatikan bahwa metode ini tidak selalu berhasil dan meskipun berhasil, tidak selalu jelas apa yang Anda perlukan untuk mengalikan pembilang dan penyebutnya. Akan tetapi, jika integral tersebut berhasil dan Anda dapat mengetahui suku apa yang Anda perlukan, maka integral tersebut dapat disederhanakan secara signifikan.

Inilah contoh berikutnya.

$$
\begin{align*}
\text{Contoh 10 Hitung integral berikut ini}: \
\int \sec^3{x}\ dx
\end{align*}
$$

- Solution
    
    Integral ini berbeda dari integral lain yang telah kita kerjakan di bagian ini. Langkah pertama dalam melakukan integral ini adalah melakukan integrasi per bagian dengan menggunakan pilihan berikut $u \ dan \ dv$
    
    $$
    \begin{align*}
    u&=\sec{x} &&&&&& dv&=\sec^2{x}\ dx\newline
    du&=\sec{x}\tan{x}\ dx &&&&&& v &=\tan{x}\ dx
    \end{align*}
    $$
    
    Perhatikan bahwa menggunakan integrasi per bagian pada masalah ini bukanlah pilihan yang jelas, tetapi ini berfungsi dengan baik di sini. Setelah melakukan integrasi dengan bagian-bagian yang kita miliki,
    
    $$
    \begin{align*}
    \int {\sec^3{x}\ dx} &= \sec{x}+\tan{x}-\int{\sec{x}\tan^2{x}\ dx}
    \end{align*}
    $$
    
    Kini integral baru tersebut juga mempunyai eksponen ganjil pada garis potongnya dan eksponen genap pada garis singgungnya sehingga contoh hasil kali garis potong dan garis singgung sebelumnya tetap tidak ada gunanya bagi kita.
    
    Untuk melakukan integral ini pertama-tama kita akan menulis garis singgung integral dalam bentuk garis potong. Sekali lagi, ini belum tentu merupakan pilihan yang jelas namun itulah yang perlu kita lakukan dalam kasus ini.
    
    $$
    \begin{align*}
    \int {\sec^3{x}\ dx} &= \sec{x}+\tan{x}-\int{\sec{x}(\sec^2{x}-1)\ dx}\newline
    &= \sec{x}+\tan{x}-\int{\sec^3{x}\ dx}+\int{\sec{x}\ dx}
    \end{align*}
    $$
    
    Sekarang, kita dapat menggunakan hasil dari contoh sebelumnya untuk mengerjakan integral kedua dan memperhatikan bahwa integral pertama adalah integral yang diminta untuk kita evaluasi dengan tanda minus di depannya. Jadi, tambahkan ke kedua sisi untuk mendapatkan,
    
    $$
    \begin{align*}
    2\int {\sec^3{x}\ dx} &= \sec{x}+\tan{x}+\ln|{\sec{x}+\tan{x}|}
    \end{align*}
    $$
    
    Akhirnya bagi dua dan selesai.
    
    $$
    \begin{align*}
    \int {\sec^3{x}\ dx} &= \dfrac{1}{2}(\sec{x}+\tan{x}+\ln|{\sec{x}+\tan{x}|})+c
    \end{align*}
    $$
    

Sekali lagi, perhatikan bahwa kita kembali menggunakan gagasan untuk mengintegrasikan ruas kanan hingga integral asli muncul, lalu memindahkannya ke ruas kiri dan membaginya dengan koefisiennya untuk menyelesaikan evaluasi. Kami pertama kali melihat ini di bagian Integrasi berdasarkan Bagian dan pada saat itu mencatat bahwa ini adalah teknik yang bagus untuk diingat. Berikut adalah contoh lain dari teknik ini.

Sekarang kita telah melihat perkalian garis potong dan garis singgung, mari kita akui juga bahwa karena kita dapat menghubungkan garis potong dan kotangen dengan cara

$$
\begin{align*}
1+\cot^2{x}=\csc^2
{x}
\end{align*}
$$

semua pekerjaan yang kami lakukan untuk perkalian secant dan tangen juga akan berfungsi untuk perkalian csc dan cot. Kami serahkan kepada Anda untuk memverifikasinya.

Ada satu topik terakhir yang akan dibahas di bagian ini sebelum melanjutkan.

Sampai di sini kita hanya melihat hasil kali sinus dan cosinus serta hasil kali sec dan tangen. Namun, metode yang digunakan untuk mengerjakan integral ini juga dapat digunakan pada beberapa hasil bagi yang melibatkan sinus dan cosinus serta hasil bagi yang melibatkan sec dan tan (dan karenanya hasil bagi yang melibatkan kosekan dan kotangen)

Mari kita lihat sekilas contohnya

$$
\begin{align*}
\text{Contoh 11 Hitung integral berikut ini}: \
\int \dfrac{\sin^7{x}}{\cos^4{x}}\ dx
\end{align*}
$$

- Solution
    
    Jika ini adalah hasil kali sinus dan kosinus, kita pasti tahu apa yang harus dilakukan. Kita akan menghapus sinus (karena eksponen sinus ganjil) dan mengubah sinus lainnya menjadi cosinus. Ide yang sama akan berhasil dalam kasus ini. Kita akan menghapus sinus dari pembilangnya dan mengubah sisanya menjadi kosinus sebagai berikut,
    
    $$
    \begin{align*}
    \int \dfrac{\sin^7{x}}{\cos^4{x}}\ dx&= \int \dfrac{\sin^6{x}}{\cos^4{x}}\sin{x}\ dx\newline
    &=\int \dfrac{(\sin^2{x})^3}{\cos^4{x}}\sin{x}\ dx\newline
    &=\int \dfrac{(1-\cos^2{x})^3}{\cos^4{x}}\sin{x}\ dx
    \end{align*}
    $$
    
    Pada titik ini yang perlu kita lakukan hanyalah menggunakan substitusi $u = \cos{x}$ dan kita sudah selesai
    
    $$
    \begin{align*}
    \int \dfrac{\sin^7{x}}{\cos^4{x}}\ dx&=-\int \dfrac{(1-u^2)^3}{u^4}\ du\newline
    &=-\int (u^{-4}-3u^{-2}+3-u^2)\ du\newline
    &= -\left(-\dfrac{1}{3}\dfrac{1}{u^3}+3\dfrac{1}{u}+3u-\dfrac{1}{3}u^3\right)+c\newline
    &= \dfrac{1}{3\cos^3{x}}-\dfrac{3}{\cos{x}}-3\cos{x}+\dfrac{1}{3}\cos^3{x}+c
    \end{align*}
    $$
    

Jadi, dalam keadaan yang tepat, kita dapat menggunakan ide yang dikembangkan untuk membantu kita menangani hasil kali fungsi trigonometri untuk menangani hasil bagi fungsi trigonometri. Pertanyaan wajarnya adalah, kondisi apa yang tepat?

Pertama-tama perhatikan bahwa jika hasil bagi telah dibalik seperti pada integral ini,

$$
\begin{align*}
\int{\dfrac{\cos^4{x}}{\sin^7{x}}\ dx}
\end{align*}
$$

kita tidak akan mampu menghilangkan satu sinus pun.

$$
\begin{align*}
\int{\dfrac{\cos^4{x}}{\sin^7{x}}\ dx}&= \int{\dfrac{\cos^4{x}}{\sin^6{x}}\dfrac{1}{\sin{x}}\ dx}
\end{align*}
$$

Dalam hal ini, sinus yang “dihapus” tetap berada di penyebutnya dan tidak ada gunanya bagi kita untuk melakukan substitusi $u = \cos{x}$ karena substitusi ini memerlukan sinus pada pembilang hasil bagi. Perhatikan juga bahwa, meskipun kita dapat mengubah sinus menjadi kosinus, integral yang dihasilkan tetap merupakan integral yang cukup sulit.

Jadi, kita dapat menggunakan metode yang kita terapkan pada hasil kali fungsi trigonometri dengan hasil bagi fungsi trigonometri dengan syarat suku yang perlu dihilangkan bagiannya adalah pembilang dari hasil bagi tersebut.
