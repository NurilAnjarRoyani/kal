---
title: Invers Matriks

---

---
title : Invers_Matriks

---

# INVERS MATRIKS
### Definisi Matriks Invers

Matriks invers adalah matriks yang jika dikalikan dengan matriks aslinya akan menghasilkan matriks identitas. Jika  ${A}$  adalah suatu matriks persegi (jumlah baris = jumlah kolom), maka invers dari  ${A}$  yang ditulis sebagai  $A^{-1}$  ,memenuhi persamaan:


$$
A \times A^{-1}=A^{-1} \times A=I
$$


dimana  ${I}$  adalah matriks identitas, yaitu dengan elemen diagonal utama bernilai 1 dan elemen lainnya 0. Contoh matriks identitas untuk ukuran 3x3 :


$$
I=\left[\begin{array}{lll}1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1\end{array}\right]
$$


### Syarat Suatu Matriks Memiliki Invers
Tidak semua matriks memiliki invers. Syarat suatu matriks  ${A}$  memiliki invers adalah:
1. Matriks harus persegi (jumlah baris = jumlah kolom).
2. Determinan matriks tidak nol  $\rightarrow|A| \neq 0$  .  Jika determinan matriks = 0, maka matriks tersebut disebut singular dan tidak memiliki invers.
## MATRIK 3 PERSAMAAN


$$
\left\{\begin{array}
{l}2 x+3 y-z=2 \\ 
4 x-y+5 z=4 \\ 
-3 x+2 y+4 z=-3
\end{array}\right.
$$


### 1. Menuliskan Matriks Augmented ${A | I}$
Diketahui matriks  $A$  :


$$
\left\{\begin{array}
{l}2 x+3 y-z=2 \\ 
4 x-y+5 z=4 \\ 
-3 x+2 y+4 z=-3
\end{array}\right.
$$


Untuk mencari invers menuliskan matriks dalam bentuk augmented : 


$$
[A \mid I]=\left[\begin{array}{ccc|ccc}
2 & 3 & -1 & 1 & 0 & 0 \\ 
4 & -1 & 5 & 0 & 1 & 0 \\ 
-3 & 2 & 4 & 0 & 0 & 1
\end{array}\right]
$$


tujuan kita adalah mengubah bagian kiri menjadi matriks identitas, agar bagian kanan menjadi matriks invers  $A^{-1}$  . 

### 2. Mengubah Elemen (1,1) Menjadi 1
supaya elemen pertama (1,1) menjadi 1, kita membagi baris pertama dengan 2 : 
Operasi perhitungan :


$R_1=\frac{1}{2} R_1$


$$
\begin{gathered}
R_1=\frac{1}{2} R_1 \\
{\left[\begin{array}{ccc|ccc}
1 & \frac{3}{2} & -\frac{1}{2} & \frac{1}{2} & 0 & 0 \\
4 & -1 & 5 & 0 & 1 & 0 \\
-3 & 2 & 4 & 0 & 0 & 1
\end{array}\right]}
\end{gathered}
$$


### 3. Membuat Elemen (2,1) dan (3,1) Menjadi Nol
kita ubah elemen (2,1) dan (3,1) menjadi nol dengan operasi perhitungan :


-  $2 \rightarrow R_2=R_2 - 4R_1$
-  $3 \rightarrow R_3=R_3 + 3R_1$


Tabel Perhitungan untuk  $R_2=R_2-4 R_1$  :


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline R_2(1) & 4-4(1) & 0 \\
\hline R_2(2) & -1-4\left(\frac{3}{2}\right)=-1-6 & -7 \\
\hline R_2(3) & 5-4\left(-\frac{1}{2}\right)=5+2 & 7 \\
\hline R_2(4) & 0-4\left(\frac{1}{2}\right)=-2 & -2 \\
\hline R_2(5) & 1-4(0) & 1 \\
\hline R_2(6) & 0-4(0) & 0 \\
\hline
\end{array}
$$


Jadi, baris kedua setelah operasi:


$$
R_2=(0,-7,7,-2,1,0)
$$

 
Tabel Perhitungan untuk  $R_3=R_3+3 R_1$  :


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline R_3(1) & -3+3(1) & 0 \\
\hline R_3(2) & 2+3\left(\frac{3}{2}\right)=2+\frac{9}{2}=\frac{13}{2} & \frac{13}{2} \\
\hline R_3(3) & 4+3\left(-\frac{1}{2}\right)=4-\frac{3}{2}=\frac{5}{2} & \frac{5}{2} \\
\hline R_3(4) & 0+3\left(\frac{1}{2}\right)=\frac{3}{2} & \frac{3}{2} \\
\hline R_3(5) & 0+3(0) & 0 \\
\hline R_3(6) & 1+3(0) & 1 \\
\hline
\end{array}
$$


Jadi, baris ketiga setelah operasi:


$$
R_3=\left(0, \frac{13}{2}, \frac{5}{2}, \frac{3}{2}, 0,1\right)
$$


#### Hasil Matriks setelah eliminasi :


$$
\left[\begin{array}{ccc|ccc}
1 & \frac{3}{2} & -\frac{1}{2} & \frac{1}{2} & 0 & 0 \\
0 & -7 & 7 & -2 & 1 & 0 \\
0 & \frac{13}{2} & \frac{5}{2} & \frac{3}{2} & 0 & 1
\end{array}\right]
$$


### 4. Mengubah Elemen (2,2) Menjadi 1
pada tahap ini, kita akan mengubah elemen (2,2) dari -7 menjadi 1 dengan cara membagi seluruh baris ke 2 dengan -7
Operasi Perhitungan : 


$R_2=\frac{1}{-7} R_2$


Tabel Perhitungan untuk   $R_2=\frac{1}{-7} R_2$


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline R_2(1) & 0 \div(-7) & 0 \\
\hline R_2(2) & -7 \div(-7) & 1 \\
\hline R_2(3) & 7 \div(-7) & -1 \\
\hline R_2(4) & -2 \div(-7) & \frac{2}{7} \\
\hline R_2(5) & 1 \div(-7) & -\frac{1}{7} \\
\hline R_2(6) & 0 \div(-7) & 0 \\
\hline
\end{array}
$$


Jadi, baris kedua setelah operasi:


$$
R_2=\left(0,1,-1, \frac{2}{7},-\frac{1}{7}, 0\right)
$$


#### Hasil Matriks setelah eliminasi :


$$
\left[\begin{array}{ccc|ccc}
1 & \frac{3}{2} & -\frac{1}{2} & \frac{1}{2} & 0 & 0 \\
0 & 1 & -1 & \frac{2}{7} & -\frac{1}{7} & 0 \\
0 & \frac{13}{2} & \frac{5}{2} & \frac{3}{2} & 0 & 1
\end{array}\right]
$$


### 5. Membuat Elemen (1,2) dan (3,2) Menjadi Nol
pada langkah ini, kita akan membuat elemen (1,2) dan (3,2) menjadi 0 dengan menggunakan baris kedua yang sudah diubah sebelumnya.
operasi perhitungan :


-  $R_1=R_1-\frac{3}{2} R_2$


-  $R_3=R_3-\frac{13}{2} R_2$


Tabel perhitungan untuk  $R_1=R_1-\frac{3}{2} R_2$


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline R_1(1) & 1-\frac{3}{2}(0) & 1 \\
\hline R_1(2) & \frac{3}{2}-\frac{3}{2}(1)=0 & 0 \\
\hline R_1(3) & -\frac{1}{2}-\frac{3}{2}(-1)=-\frac{1}{2}+\frac{3}{2}=1 & 1 \\
\hline R_1(4) & \frac{1}{2}-\frac{3}{2}\left(\frac{2}{7}\right)=\frac{1}{2}-\frac{6}{14}=\frac{7}{14}-\frac{6}{14}=\frac{1}{14} & \frac{1}{14} \\
\hline R_1(5) & 0-\frac{3}{2}\left(-\frac{1}{7}\right)=0+\frac{3}{14} & \frac{3}{14} \\
\hline R_1(6) & 0-\frac{3}{2}(0)=0 & 0 \\
\hline
\end{array}
$$


Jadi, baris pertama setelah operasi:


$$
R_1=\left(1,0,1, \frac{1}{14}, \frac{3}{14}, 0\right)
$$


Tabel perhitungan untuk  $R_3=R_3-\frac{13}{2} R_2$
 
 
$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline R_3(1) & 0-\frac{13}{2}(0) & 0 \\
\hline R_3(2) & \frac{13}{2}-\frac{13}{2}(1)=0 & 0 \\
\hline R_3(3) & \frac{5}{2}-\frac{13}{2}(-1)=\frac{5}{2}+\frac{13}{2}=\frac{18}{2}=9 & 9 \\
\hline R_3(4) & \frac{3}{2}-\frac{13}{2}\left(\frac{2}{7}\right)=\frac{3}{2}-\frac{26}{14}=\frac{21}{14}-\frac{26}{14}=-\frac{5}{14} & -\frac{5}{14} \\
\hline R_3(5) & 0-\frac{13}{2}\left(-\frac{1}{7}\right)=0+\frac{13}{14} & \frac{13}{14} \\
\hline R_3(6) & 1-\frac{13}{2}(0)=1 & 1 \\
\hline
\end{array}
$$


Jadi, baris ketiga setelah operasi:


$$
R_3=\left(0,0,9,-\frac{5}{14}, \frac{13}{14}, 1\right)
$$


#### Hasil Matriks setelah eliminasi :


$$
\left[\begin{array}{ccc|ccc}
1 & 0 & 1 & \frac{1}{14} & \frac{3}{14} & 0 \\
0 & 1 & -1 & \frac{2}{7} & -\frac{1}{7} & 0 \\
0 & 0 & 9 & -\frac{5}{14} & \frac{13}{14} & 1
\end{array}\right]
$$


### 6. Mengubah Elemen (3,3) Menjadi 1
bagi baris ketiga dengan 9
Operasi perhitungan :


$R_3=R_3-\frac{1}{9}$


Tabel Perhitungan untuk $R_3=R_3-\frac{1}{9}$


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline R_3(1) & 0 \div 9 & 0 \\
\hline R_3(2) & 0 \div 9 & 0 \\
\hline R_3(3) & 9 \div 9 & 1 \\
\hline R_3(4) & -\frac{5}{14} \div 9=-\frac{5}{126} & -\frac{5}{126} \\
\hline R_3(5) & \frac{13}{14} \div 9=\frac{13}{126} & \frac{13}{126} \\
\hline R_3(6) & 1 \div 9 & \frac{1}{9} \\
\hline
\end{array}
$$


Jadi, baris ketiga setelah operasi:


$$
R_3=\left(0,0,1,-\frac{5}{126}, \frac{13}{126}, \frac{1}{9}\right)
$$


#### Hasil Matriks setelah eliminasi :


$$
\left[\begin{array}{ccc|ccc}
1 & 0 & 1 & \frac{1}{14} & \frac{3}{14} & 0 \\
0 & 1 & -1 & \frac{2}{7} & -\frac{1}{7} & 0 \\
0 & 0 & 1 & -\frac{5}{126} & \frac{13}{126} & \frac{1}{9}
\end{array}\right]
$$


### 7. Mengubah Elemen (3,3) Menjadi Nol
Pada langkah ini, kita akan mengubah elemen (3,3) menjadi nol dengan operasi perhitungan :


-   $R_1=R_1-R_3$  untuk mengubah  $R_1(3)=1$           menjadi nol.
-   $R_2=R_2+R_3$  untuk mengubah  $R_2(3)=-1$           menjadi nol.

Tabel Perhitungan untuk  $R_1=R_1-R_3$  : 


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline R_1(1) & 1-0 & 1 \\
\hline R_1(2) & 0-0 & 0 \\
\hline R_1(3) & 1-1=0 & 0 \\
\hline R_1(4) & \frac{1}{14}-\left(-\frac{5}{126}\right)=\frac{9}{126}+\frac{5}{126}=\frac{14}{126}=\frac{1}{9} & \frac{1}{9} \\
\hline R_1(5) & \frac{3}{14}-\frac{13}{126}=\frac{27}{126}-\frac{13}{126}=\frac{14}{126}=\frac{1}{9} & \frac{1}{9} \\
\hline R_1(6) & 0-\frac{1}{9}=-\frac{1}{9} & -\frac{1}{9} \\
\hline
\end{array}
$$


Jadi, baris pertama setelah operasi:


$$
R_1=\left(1,0,0, \frac{1}{9}, \frac{1}{9},-\frac{1}{9}\right)
$$


Tabel Perhitungan untuk  $R_2=R_2+R_3$  : 


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline R_2(1) & 0+0 & 0 \\
\hline R_2(2) & 1+0 & 1 \\
\hline R_2(3) & -1+1=0 & 0 \\
\hline R_2(4) & \frac{2}{7}+\left(-\frac{5}{126}\right)=\frac{36}{126}-\frac{5}{126}=\frac{31}{126} & \frac{31}{126} \\
\hline R_2(5) & -\frac{1}{7}+\frac{13}{126}=-\frac{18}{126}+\frac{13}{126}=-\frac{5}{126} & -\frac{5}{126} \\
\hline R_2(6) & 0+\frac{1}{9}=\frac{1}{9} & \frac{1}{9} \\
\hline
\end{array}
$$


Jadi, baris kedua setelah operasi:


$$
R_2=\left(0,1,0, \frac{31}{126},-\frac{5}{126}, \frac{1}{9}\right)
$$


#### Hasil Matriks setelah eliminasi :


$$
\left[\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{1}{9} & \frac{1}{9} & -\frac{1}{9} \\
0 & 1 & 0 & \frac{31}{126} & -\frac{5}{126} & \frac{1}{9} \\
0 & 0 & 1 & -\frac{5}{126} & \frac{13}{126} & \frac{1}{9}
\end{array}\right]
$$


#### Perhitungan Matriks  $$  X = A^{-1} \times B  $$

Diketahu matriks :


$$
\begin{gathered}
A^{-1}=\left[\begin{array}{ccc}
\frac{1}{9} & \frac{1}{9} & -\frac{1}{9} \\
\frac{31}{126} & -\frac{5}{126} & \frac{1}{9} \\
-\frac{5}{126} & \frac{13}{126} & \frac{1}{9}
\end{array}\right] \\
B=\left[\begin{array}{c}
2 \\
4 \\
-3
\end{array}\right]
\end{gathered}
$$


Tabel Perhitungan untuk X1 : 


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline (1 / 9) \times 2 & \frac{2}{9} & \frac{2}{9} \\
\hline (1 / 9) \times 4 & \frac{4}{9} & \frac{4}{9} \\
\hline (-1 / 9) \times(-3) & \frac{3}{9} & \frac{3}{9} \\
\hline Total & \frac{2}{9}+\frac{4}{9}+\frac{3}{9} & 1 \\
\hline
\end{array}
$$


Tabel perhitungan untuk X2 : 


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline (31 / 126) \times 2 & \frac{62}{126} & \frac{62}{126} \\
\hline (-5 / 126) \times 4 & \frac{-20}{126} & \frac{-20}{126} \\
\hline (1 / 9) \times(-3) & \frac{-3}{9}=\frac{-42}{126} & \frac{-42}{126} \\
\hline Total & \frac{62}{126}-\frac{20}{126}-\frac{42}{126} & 0 \\
\hline
\end{array}
$$


Tabel Perhitungan untuk X3 : 


$$
\begin{array}{|l|l|l|}
\hline Elemen & Perhitungan & Hasil \\
\hline (-5 / 126) \times 2 & \frac{-10}{126} & \frac{-10}{126} \\
\hline (13 / 126) \times 4 & \frac{52}{126} & \frac{52}{126} \\
\hline (1 / 9) \times(-3) & \frac{-3}{9}=\frac{-42}{126} & \frac{-42}{126} \\
\hline Total & \frac{-10}{126}+\frac{52}{126}-\frac{42}{126} & 0 \\
\hline
\end{array}
$$


#### Hasil Akhir


$$
X=\left[\begin{array}{l}
1 \\
0 \\
0
\end{array}\right]
$$





