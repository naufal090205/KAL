---
title: Untitled

---

### Operasi Baris Elementer 

teknik dalam aljabar linear yang digunakan untuk mengubah matriks melalui serangkaian operasi tanpa mengubah solusi sistem persamaan linear yang diwakilinya. OBE sering digunakan dalam metode eliminasi Gauss dan Gauss-Jordan untuk menyelesaikan sistem persamaan linear serta mencari invers matriks.

Tiga Jenis Operasi Baris Elementer
Pertukaran Baris (Swapping Rows)

Menukar posisi dua baris dalam matriks.
Notasi: Ri ↔ Rj (menukar baris ke-𝑖 dengan baris ke-𝑗).

Perkalian Baris dengan Skalar (Scaling a Row)

Mengalikan suatu baris dengan bilangan bukan nol.
Notasi: Ri → k Ri, dengan k =0

Penjumlahan Baris (Row Addition)

Menambahkan kelipatan suatu baris ke baris lain.
Notasi: Ri → Ri + krj (menambahkan k kali baris ke-j kebaris ke-i).


### Eliminasi Gauss 

metode dalam aljabar linear yang digunakan untuk menyelesaikan sistem persamaan linear dengan mengubah matriks koefisien menjadi bentuk eselon baris menggunakan Operasi Baris Elementer (OBE).

Metode ini dinamai berdasarkan Carl Friedrich Gauss dan sering digunakan untuk mencari solusi sistem persamaan linear, menentukan determinan, dan menemukan invers matriks.

Tahapan Eliminasi Gauss
Eliminasi Gauss terdiri dari dua langkah utama:

Membentuk Eselon Baris (Forward Elimination)

Mengubah matriks ke dalam bentuk eselon baris (Row Echelon Form).
Bentuk ini memiliki elemen nol di bawah elemen diagonal utama.
Dilakukan dengan menggunakan Operasi Baris Elementer (OBE).
Substitusi Balik (Backward Substitution)

Digunakan untuk menyelesaikan sistem persamaan setelah terbentuk eselon baris.
Dimulai dari baris terakhir dan bergerak ke atas.



### contoh soal 1

Selesaikan dengan menggunakan eleminasi gauss

$$
\begin{array}{cc}
x_1+2x_2+3x_3&=6\\
2x_1+4x_2+6x_3&=12\\
x_3+x_2&=2
\end{array}
$$

penyelesaian
Langkah 1: Tulis dalam Bentuk Matriks Augmented
Bentuk matriks augmented dari sistem ini adalah:
\begin{bmatrix}
1&2&3&|6\\
2&4&6&|12\\
0&1&1&|2
\end{bmatrix}

Langkah 2: Eliminasi Baris
Kita akan menghilangkan elemen di bawah elmen utama di kolom pertama, gunakan operasi:

\begin{array}{cc}
R_2 \rightarrow R_2 - 2R_1
\end{array}

sehingga:

\
\begin{bmatrix}
1&2&3&|6\\
0&0&0&|0\\
0&1&1&|2
\end{bmatrix}

Langkah 3: Interpretasi baris kedua dirubah menjadi *0 = 0*

\begin{aligned}
x_1+2x_2+3x_3&=6\\
x_2+x_3&=2
\end{aligned}

langkah 4: substitusi dari persamaan kedua : 

\begin{array}{cc}
x_2=2-x_3
\end{array}

substitusikan ke persamaan pertama:

\begin{array}{cc}
x_1+ 2(2-x_3)+3x_3&=6\\
x_1+ 4-2x_3 +3x_3&=6\\
x_1+ 4 +x_3&=6\\
x_1=& 2-x_3
\end{array}

kesimpulan 
solusi umum dari sistem ini adalah:

\begin{aligned}
x_1&=2-x_3\\
x_2&=2-x_3\\
x_3&=X_3
\end{aligned}

### contoh soal 2 
selesaikan dengan menggunakan eliminasi gauss
$
\begin{array}{cc}
x_1+x_2+x_3&=3\\
2x_1+x_3&=5\\
x_1+2x_2&=3
\end{array}
$

penyelesaian
langkah 1 : tulis dalam bentuk matriks augmented
$
\begin{bmatrix}
1&1&1&|3\\
2&0&1&|5\\
1&2&1&|3
\end{bmatrix}
$
langkah 2:eliminasi baris kita akan menghilangkan elemen di bawah elemen utama di kolom pertama.

\begin{array}{cc}
R_2\rightarrow R_2 - 2R_1
\end{array}

\begin{array}{cc}
R_3\rightarrow R_3 - R_1
\end{array}

sehingga matriks berubah menjadi:
$
\begin{bmatrix}
1&1&1&|3\\
0&-2&-1&|-1\\
0&1&-1&|0
\end{bmatrix}
$
selanjutnya, buat elemen utama di baris kedua menjadi 1 dengan membagi baris kedua dengan -2:

\begin{array}{cc}
R_2\rightarrow\frac{R_2}{-2}
\end{array}

hasilnya:

\begin{bmatrix}
1&1&1&|3\\
0&1&\frac{1}{2}&|\frac{1}{2}\\
0&1&-1&|0
\end{bmatrix}

kemudian eliminasi elemen di bawah elemen utama dengan:

\begin{array}{cc}
R_3\rightarrow R_3-R_2
\end{array}

sehingga diperoleh:
\begin{bmatrix}
1&1&1&|3\\
0&1&\frac{1}{2}&|\frac{1}{2}\\
0&0&-\frac{3}{2}&|-\frac{1}{2}
\end{bmatrix}
langkah 3: substitusi balik* 
dari baris ketiga:

\begin{array}{cc}
-\frac{3}{2}x_3=-\frac{1}{2}
\end{array}

\begin{array}{cc}
x_3=\frac{1}{3}
\end{array}

dari baris kedua : 

\begin{array}{cc}
x_2+\frac{1}{2}x_3=\frac{1}{2}
\end{array}

\begin{array}{cc}
x_2+\frac{1}{2}\times\frac{1}{3}=\frac{1}{2}
\end{array}

\begin{array}{cc}
x_2+\frac{1}{6}=\frac{1}{2}
\end{array}

\begin{array}{cc}
x_2+\frac{1}{6}-\frac{1}{6}=\frac{3}{6}-\frac{1}{6}=\frac{2}{6}=\frac{1}{3}
\end{array}

dari baris pertama: 
\begin{array}{cc}
x_1+x_2+x_3=3
\end{array}

\begin{array}{cc}
x_1=-\frac{2}{3}=\frac{9}{3}-\frac{2}{3}=\frac{7}{3}
\end{array}

kesimpulan 
jadi, solusi dari sistem persamaan adalah:
\begin{aligned}
x_1&=\frac{7}{3}\\
x_2&=\frac{1}{3}\\
x_3&=\frac{1}{3}
\end{aligned}


### contoh soal 3
selesaikan dengan menggunakan eliminasi gauss
$$
\begin{array}{cc}
2x_1+2x_2&=4\\
x_1+x_2&=2
\end{array}
$$

penyelesaian
langkah 1 : menyelesaikan ke bentuk matriks augmented

\begin{bmatrix}
2&2&|4\\
1&1&|2\\
\end{bmatrix}

langkah 2 : membuat elemen di bawah pivot menjadi nol.

\begin{array}{cc}
R_1\leftarrow R_1-2R_2
\end{array}

setelah melakukan perhitungan kita mendapatkan : 

$$
\begin{bmatrix}
R_1: 2 - 2 \cdot 1=0\\
2-2\cdot 1=0\\
4-2\cdot 2=0
\end{bmatrix}
$$

sehingaa matriks augmented menjadi : 

\begin{bmatrix}
1&1&|2\\
0&0&|0
\end{bmatrix}

dari baris kedua, kita dapat mengekspresikan (x_1) dalam bentuk (x_2) : 

\begin{bmatrix}
x_1+x_2=2\rightarrow x_1=2-x_2
\end{bmatrix}

karena kita memiliki satu persamaan dengan dua variabel,kita dapat menyagakan solusi dalam bentuk parameter.misalkan (x_2 = t), maka:

\begin{array}{cc}
x_1=2-t
\end{array}

jadi, solusi umum dari sistem persamaan ini adalah : 

\begin{cases}
x_1=2-t\\
x_2=t
\end{cases}

di mana (t) adalah parameter bebas.

### contoh soal 4
selesaikan dengan menggunakas eliminasi gauss
$$
\begin{array}{cc}
x_1+x_2&=5\\
x_1+2x_3&=6\\
\end{array}
$$

penyelesaian : 
1. tulis sistem persamaan dalam bentuk matriks augmented : 

\begin{bmatrix}
1&1&0&|&5\\
1&0&2&|&4
\end{bmatrix}

2. lakukan operasi baris untuk mendapatkan bentuk eselon baris: 

\begin{array}{cc}
R_2\rightarrow R_2
\end{array}

Hasilnya : 

\begin{bmatrix}
1&1&0&|&5\\
0&-1&2&|&-1
\end{bmatrix}

\begin{array}{cc}
R_2\rightarrow\frac{R_2}{-1}
\end{array}

hasilnya : 

\begin{bmatrix}
1&1&0&|&5\\
0&1&-2&|&1
\end{bmatrix}

3. lakukan subtitusi mundur untuk menemukan solusi: 

- dari baris 2: 

\begin{array}{cc}
x_1+x_2=2\rightarrow x_1=2-x_2
\end{array}

- dari baris 1:
 
\begin{array}{cc}
x_1+x_2=5\implies x_1+(1+2x_3)=5\implies x_1=4-2x_3
\end{array}

4. solusi akhir : 
 
\begin{aligned}
x_1&=4-2x_3\\
x_2&=1+2x_3\\
x_3&=x_3
\end{aligned}

jadi, solusi dari sistem persamaan adalah:

\begin{array}{cc}
\left(x_1,x_2,x_3\right)=\left(4-2t,1+2t,t\right),\quad t\in\mathbb{r}
\end{array}

sistem ini memiliki banyak solusi karena terdapat parameter bebas $( t )$.