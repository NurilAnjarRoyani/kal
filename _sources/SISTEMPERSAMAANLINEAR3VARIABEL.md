---
title: SISTEM PERSAMAAN LINEAR 3 VARIABEL

---

---
title: sistem_persamaan_3variabel

---

# SISTEM PERSAMAAN LINEAR 3 VARIABEL
## Penyelesaian Sistem Persamaan Linear menggunakan eliminasi Gauss-Jordan
$$
\begin{cases}x+2y+3z=4 & \text { (Persamaan 1) } \\
2x+3y+4z=1 & \text { (Persamaan 2) } \\
3x+4y+z=2 & \text { (Persamaan 3) }\end{cases}
$$

Langkah 1: Membuat Matriks Augmented
Tulis sistem persamaan dalam bentuk matriks augmented:
$$
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 4 \\
2 & 3 & 4 & 1 \\
3 & 4 & 1 & 2
\end{array}\right]
$$

Langkah 2: Eliminasi Gauss-Jordan
Tujuan: Mengubah matriks menjadi bentuk eselon baris tereduksi (row reduced echelon form / RREF).

Langkah 2.1: Membuat elemen pertama pada baris pertama menjadi 1 (sudah 1, tidak perlu perubahan).

Langkah 2.2: Eliminasi elemen di bawah pivot pertama.
- Gunakan operasi baris:
- $ R_2=R_2 - 2R_1$
- $ R_3=R_3 - 3R_1$

Hasilnya:
$$
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 4 \\
0 & -1 & -2 & -7 \\
0 & -2 & -8 & -10
\end{array}\right]
$$

Langkah 2.3: Membuat elemen kedua pada baris kedua menjadi 1.
- Bagi baris kedua $(R_2)$ dengan $-1$:
$$
\left[\begin{array}{ccc|c}
1 & 2 & 3 & 4 \\
0 & 1 & 2 & 7 \\
0 & -2 & -8 & -10
\end{array}\right]
$$

Langkah 2.4: Eliminasi elemen di atas dan di bawah pivot kedua.
- Gunakan operasi baris:
- $ R_1=R_1 - 2R_2$
- $ R_3=R_3 + 2R_2$

Hasilnya:
$$
\left[\begin{array}{ccc|c}
1 & 0 & -1 & -10 \\
0 & 1 & 2 & 7 \\
0 & 0 & -4 & 4
\end{array}\right]
$$

Langkah 2.5: Membuat elemen ketiga pada baris ketiga menjadi 1.
- Bagi baris ketiga $(R_3)$ dengan $-4$:
$$
\left[\begin{array}{ccc|c}
1 & 0 & -1 & -10 \\
0 & 1 & 2 & 7 \\
0 & 0 & 1 & -1
\end{array}\right]
$$

Langkah 2.6: Eliminasi elemen di atas pivot ketiga.
- Gunakan operasi baris:
- $ R_1=R_1 + R_3$
- $ R_2=R_2 - 2R_3$

Hasilnya:
$$
\left[\begin{array}{lll|l}
1 & 0 & 0 & -11 \\
0 & 1 & 0 & 9 \\
0 & 0 & 1 & -1
\end{array}\right]
$$

Langkah 3: Solusi
Dari matriks terakhir, kita dapat membaca solusinya:
$$
x=-11, \quad y=9, \quad z=-1
$$

Verifikasi Solusi
Substitusikan nilai $x, y, z$ ke dalam persamaan asli untuk memverifikasi kebenaran solusi:
1. Persamaan 1:
$$
x+2y+3z=4
$$
Substitusi:
$$
-11 + 2(9) + 3(-1) = -11 + 18 - 3 = 4
$$
2. Persamaan 2:
$$
2x+3y+4z=1
$$
Substitusi:
$$
2(-11) + 3(9) + 4(-1) = -22 + 27 - 4 = 1
$$
3. Persamaan 3:
$$
3x+4y+z=2
$$
Substitusi:
$$
3(-11) + 4(9) + (-1) = -33 + 36 - 1 = 2
$$

### Geogebra Persamaan Linear dengan 3 Variabel
<iframe src="https://www.geogebra.org/calculator/vwxzkyzh?embed" width="800" height="600" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>

