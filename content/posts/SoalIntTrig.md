+++
title = 'Soal Integral Trigonometri'
date = 2024-03-19T07:03:57+07:00
draft = false
math = true
katex = true
+++

$$
\begin{align*}
\int{\sec^5{x}\tan^6{x}\ dx}&= \int{\sec^5{x}(\tan^2{x})^3\ dx}\newline &=\int{\sec^5{x}(\sec^2{x}-1)^3\ dx}
\end{align*}
$$

Kita misalkan sebentar $u = \sec{x}$ untuk memudahkan penggunaan sifat disributif

$$
\begin{align*}
\int{\sec^5{x}\tan^6{x}\ dx}&=\int{u^5(u^2-1)^3\ dx}\newline
&=\int{u^{11}-3u^9+3u^7-u^5\ dx}\newline
&= \int{\sec^{11}{x}-3\sec^9{x}+3\sec^7{x}-\sec^5{x}\ dx}
\end{align*}
$$

Dengan menggunakan reduksi formula :

$$
\begin{align*}
\int{\sec^n{x}\ dx}&= \dfrac{\sec^{n-2}{x}\tan{x}}{(n-1)}+\dfrac{n-2}{n-1}\int{\sec^{n-2}\ dx}
\end{align*}
$$

Diperoleh sebagai berikut,

$$
\begin{align*}
\int{\sec^{11}{x}\ dx}&= \dfrac{\sec^{9}{x}\tan{x}}{10}+\dfrac{9}{10}\int{\sec^{9}{x}\ dx}\newline
\int{\sec^{9}{x}\ dx}&= \dfrac{\sec^{7}{x}\tan{x}}{8}+\dfrac{7}{8}\int{\sec^{7}{x}\ dx}\newline
\int{\sec^{7}{x}\ dx}&= \dfrac{\sec^{5}{x}\tan{x}}{6}+\dfrac{5}{6}\int{\sec^{5}{x}\ dx}\newline
\int{\sec^{5}{x}\ dx}&= \dfrac{\sec^{3}{x}\tan{x}}{4}+\dfrac{3}{4}\int{\sec^{3}{x}\ dx}\newline
\int{\sec^{3}{x}\ dx}&= \dfrac{\sec{x}\tan{x}}{2}+\dfrac{1}{2}\int{\sec{x}\ dx}\newline
\end{align*}
$$

Kita tahu bahwa $\int{\sec{x}\ dx}=\ln|{\sec{x}+\tan{x}}|+ c$ sehingga kita bisa mensubstitusi ulang keata

$$
\begin{align*}
\int{\sec^{3}{x}\ dx}&= \dfrac{\sec{x}\tan{x}}{2}+\dfrac{1}{2}\ln|{\sec{x}+\tan{x}}|\newline

\int{\sec^{5}{x}\ dx}&= \dfrac{\sec^{3}{x}\tan{x}}{4}+\dfrac{3}{4}\left(\dfrac{\sec{x}\tan{x}}{2}+\dfrac{1}{2}\ln|{\sec{x}+\tan{x}}|\right)\newline

&= \dfrac{\sec^{3}{x}\tan{x}}{4}+\dfrac{3}{8}\sec{x}\tan{x}+\dfrac{3}{8}\ln|{\sec{x}+\tan{x}}| \newline

\int{\sec^{7}{x}\ dx}&= \dfrac{\sec^{5}{x}\tan{x}}{6}+\dfrac{5}{6}\left(\dfrac{\sec^{3}{x}\tan{x}}{4}+\dfrac{3}{8}\sec{x}\tan{x}+\dfrac{3}{8}\ln|{\sec{x}+\tan{x}}|\right) \newline
&=\dfrac{\sec^{5}{x}\tan{x}}{6}+\dfrac{5}{24}\sec^{3}{x}\tan{x}+\dfrac{15}{48}\sec{x}\tan{x}+\dfrac{15}{48}\ln|{\sec{x}+\tan{x}}|\newline

\int{\sec^{9}{x}\ dx}&= \dfrac{\sec^{7}{x}\tan{x}}{8}+\dfrac{7}{8}\left(\dfrac{\sec^{5}{x}\tan{x}}{6}+\dfrac{5}{24}\sec^{3}{x}\tan{x}+\dfrac{15}{48}\sec{x}\tan{x}+\dfrac{15}{48}\ln|{\sec{x}+\tan{x}}|\right)\newline
&=\dfrac{\sec^{7}{x}\tan{x}}{8}+\dfrac{7}{48}\sec^{5}{x}\tan{x}+\dfrac{35}{192}\sec^{3}{x}\tan{x}+\dfrac{105}{384}\sec{x}\tan{x}+\dfrac{105}{384}\ln|{\sec{x}+\tan{x}}|\newline

\int{\sec^{11}{x}\ dx}&= \dfrac{\sec^{9}{x}\tan{x}}{10}+\dfrac{9}{10}\left(\dfrac{\sec^{7}{x}\tan{x}}{8}+\dfrac{7}{48}\sec^{5}{x}\tan{x}+\dfrac{35}{192}\sec^{3}{x}\tan{x}+\dfrac{105}{384}\sec{x}\tan{x}+\dfrac{105}{384}\ln|{\sec{x}+\tan{x}}|\right)\newline
&= \dfrac{\sec^{9}{x}\tan{x}}{10}+\dfrac{9}{80}\sec^{7}{x}\tan{x}+\dfrac{63}{480}\sec^{5}{x}\tan{x}+\dfrac{315}{1920}\sec^{3}{x}\tan{x}+\dfrac{945}{3840}\sec{x}\tan{x}+\dfrac{945}{3840}\ln|{\sec{x}+\tan{x}}|
\end{align*}
$$
