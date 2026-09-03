# -kelas-3E-Algoritma-Pemograman

# 🧮 Sistem Persamaan Linear Dua Variabel (SPLDV)

## 📝 Deskripsi Masalah

Sistem Persamaan Linear Dua Variabel (SPLDV) merupakan materi matematika tingkat SMP yang digunakan untuk menentukan nilai dua variabel, yaitu x dan y, dari dua persamaan linear.

Pada tugas ini dibuat sebuah program sederhana menggunakan Python untuk menentukan nilai x dan y dari dua persamaan linear dengan bentuk:

ax + by = c

dx + ey = f

Program akan menerima enam nilai sebagai input, yaitu a, b, c, d, e, dan f. Selanjutnya program menghitung nilai determinan untuk menentukan apakah SPLDV memiliki solusi tunggal.

Jika determinan tidak sama dengan nol, program akan menghitung nilai x dan y. Jika determinan sama dengan nol, program akan memberikan informasi bahwa SPLDV tidak memiliki solusi tunggal.

## 📥 Input-Proses-Output

| Bagian | Keterangan |
|---|---|
| Input | Nilai a, b, c, d, e, dan f |
| Proses | Menghitung determinan D = (a × e) − (b × d) |
| Proses | Menghitung x = ((c × e) − (b × f)) / D |
| Proses | Menghitung y = ((a × f) − (c × d)) / D |
| Output | Menampilkan nilai x dan y |
| Kondisi | Jika D = 0, SPLDV tidak memiliki solusi tunggal |

## 💻 Pseudocode

```text
START

INPUT a, b, c
INPUT d, e, f

D ← (a × e) - (b × d)

IF D = 0 THEN
    OUTPUT "SPLDV tidak memiliki solusi tunggal"
ELSE
    x ← ((c × e) - (b × f)) / D
    y ← ((a × f) - (c × d)) / D

    OUTPUT "Nilai x =", x
    OUTPUT "Nilai y =", y
END IF

END
```
