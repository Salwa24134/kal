---
title: Menghitung Invers

---
# Menghitung Invers

##### Diketahui persamaan 
$$\begin{aligned}
x1 + 2x2 + 3x3  &= 1 \\
4x1 + 5x2 + 6x3  &= 4 \\
7x1 + 8x2 + 10x3 &= 7
\end{aligned}$$

##### Penyelesaian :
Bentuk Matriks Augmentasi [A|I] dan melakukan operasi baris sampai mengubah A menjadi matriks identitas I
$$\begin{bmatrix}
1 & 2 & 3  | 1 & 0 & 0  \\
4 & 5 & 6  | 0 & 1 & 0  \\
7 & 8 & 10 | 0 & 0 & 1 
\end{bmatrix}$$


1. Buat elemen (1,1) tetap 1 (jika sudah 1 lanjut ke langkah berikutnya)
2. Eliminasi di kolom pertama (Buat 0 di(2,1) dan (3,1))
    2.1 R2 < R2 - 4R1
    2.2 R3 < R3 - 7R1
$$\begin{bmatrix}
1 & 2 & 3    | 1 & 0 & 0   \\
0 & -3 & -6  | -4 & 1 & 0  \\
0 & -6 & -11 | -7 & 0 & 1 
\end{bmatrix}$$

3. Buat elemen (2,2) menjadi 1, bagi baris kedua dengan -3:
    3.1 R2 < R2/(-3)
$$\begin{bmatrix}
1 & 2 & 3    | 1 & 0 & 0      \\
0 & 1 & 2    | 4/3 & -1/3 & 0  \\
0 & -6 & -11 | -7 & 0 & 1     
\end{bmatrix}$$ 

4. Eliminasi elemen di kolom kedua (Buat 0 di(1,2)dan (3,2))
    4.1 R1 < R1 - 2R2
    4.2 R3 < R3 + 6R2
$$\begin{bmatrix}
 1 & 0 & -1| -5/3 & 2/3 & 0  \\
 0 & 1 & 2 | 4/3 & -1/3 & 0  \\
 0 & 0 & 1 |  3  & -2   & 1 
\end{bmatrix}$$ 

5. Eliminasi elemen di kolom ketiga (Buat 0 di (1,3) dan (2,3))
    5.1 R1 < R1 + R3
    5.2 R2 < R2 - 2R3
$$\begin{bmatrix}
1 & 0 & 0 | 2 & -3 & 1  \\
0 & 1 & 0 |-5 & 3 & -2  \\
0 & 0 & 1 | 3 & -2 & 1 
\end{bmatrix}$$
 
 Bagian kiri menjadi matriks identitas, dan bagian kanan adalah invers dari A:
 A-1 = $$\begin{bmatrix}
  2 & -3 & 1  \\
 -5 & 3 & -2  \\
  3 & -2 & 1 
\end{bmatrix}$$
 

6. Menghitung x = A-1b
kalikan :
x = A-1b =  
$$\begin{bmatrix}
   2 & -3 & 1  [1] \\
  -5 & 3 & -2  [4] \\
   3 & -2 & 1  [7]
\end{bmatrix}$$

Hitung elemen-elemennya :
1. Elemen pertama
(2x1)+(-3x4)+(1x7) = 2 - 12 + 7 = 1

2. Elemen kedua
(-5 x 1)+(3x4)+(-2x7) = -5 + 12 -14 = 0

3. Elemen ketiga
(3x1) + (-2x4) + (1x7) = 3 - 8 + 5 = 0

Jadi, hasil akhirnya adalah 
x = $$\begin{bmatrix}
   1 \\
   0 \\
   0
\end{bmatrix}$$