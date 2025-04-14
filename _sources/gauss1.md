---
title: gauss grafik1

---


# Metode Eliminasi Gauss

Metode eliminasi Gauss digunakan untuk menyelesaikan persamaan linear dengan cara mengubahnya ke bentuk eselon baris.
Pertama, sistem persamaan dituliskan dalam bentuk matriks yang disebut matriks Augmentasi.
Kemudian, dilakukan Operasi Baris Elementer(OBE) seperti menukar posisi baris, mengalikan baris  dengan suatu konstanta tidak nol, dan menjumlahkan atau mengurangkan kelipatan suatu baris ke baris lain.
Setelah itu, nilai dapat ditentukan dengan metode Substitusi Balik, yaitu menyelesaikan  persamaan dari baris terakhir ke baris pertama secara bertahap. Dengan demikian, solusi sistem persamaan dapat ditemukan secara terstruktur dan sistematis.

##### Diketahui sistem persamaan linear:
$$\begin{aligned}
x + y + z  &= 6 \\
2x - y + z &= 3 \\
3x + y - z &= 4
\end{aligned}$$

##### Penyelesaian :
1. Bentuk Matriks Augmentasi 
$$\begin{bmatrix}
   1 &  1 & 1 | 6  \\
   2 & -1 & 1 | 3 \\
   3 & 1& -1 | 4 
\end{bmatrix}$$

2. Eliminasi Gauss :

langkah 1. Nol-kan elemen di bawah elemen pivot pertama (1,1)
Gunakan baris pertama untuk mengeliminasi elemen di bawahnya menjadi nol:

##### hasilnya : 
$$\begin{bmatrix}
1 &  1 & 1  |  6  \\
0 & -3 & -1 | -9  \\
0 & -2 & -4 | -14
\end{bmatrix}$$

Langkah 2.Nol-kan elemen di bawah elemen pivot kedua adalah 1 di posisi (2,2).
Gunakan baris kedua untuk mengeliminasi baris ketiga:

##### hasilnya : 
$$\begin{bmatrix}
 1 &  1 & 1  |  6  \\
 0 & -3 & -1 | -9  \\
 0 &  0 & -2 | -6 
\end{bmatrix}$$

3. Substitusi Balik

Langkah 1 dari baris terakhir:
-2z = -4
  z =2
  
Langkah 2 subsitusi z ke baris kedua:
-3y - z = -9
-3y - 2 = -9
-3y = -7
y = 3

Langkah 3 substitusi y dan z ke baris pertama: 
x +y + z = 6
x + 3 + 2 = 6
x = 6 - 5
x = 1

jadi, solusi akhir dari sistem persamaan tersebut adalah 
x = 1, y = 3, z = 2

contoh grafik: 
<iframe scrolling="no" title="grafik22" src="https://www.geogebra.org/material/iframe/id/vxdan5wh/width/1366/height/569/border/888888/sfsb/true/smb/false/stb/false/stbh/false/ai/false/asb/false/sri/false/rc/false/ld/false/sdz/false/ctl/false" width="1366px" height="569px" style="border:0px;"> </iframe>