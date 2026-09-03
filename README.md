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

## Flowchart

<img width="950" height="1050" alt="mermaid-diagram" src="https://github.com/user-attachments/assets/4e661985-bd80-49a6-94cb-914b400c8ef6" />




## Test Case

| Test Case | Input                          | Kondisi | Hasil yang Diharapkan               |
| --------- | ------------------------------ | ------- | ----------------------------------- |
| 1         | a=2, b=1, c=7, d=1, e=-1, f=1  | D ≠ 0   | x = 2.67 dan y = 1.67               |
| 2         | a=1, b=1, c=10, d=2, e=-1, f=5 | D ≠ 0   | x = 5 dan y = 5                     |


## Implementasi Python
Implementasi program dibuat menggunakan bahasa pemrograman Python dan dapat dijalankan melalui Visual Studio Code.

print("Program Penyelesaian SPLDV")
print("Bentuk persamaan:")
print("ax + by = c")
print("dx + ey = f")

a = float(input("Masukkan nilai a: "))
b = float(input("Masukkan nilai b: "))
c = float(input("Masukkan nilai c: "))

d = float(input("Masukkan nilai d: "))
e = float(input("Masukkan nilai e: "))
f = float(input("Masukkan nilai f: "))

D = (a * e) - (b * d)

if D == 0:
    print("SPLDV tidak memiliki solusi tunggal.")
else:
    x = ((c * e) - (b * f)) / D
    y = ((a * f) - (c * d)) / D

    print("Nilai x =", x)
    print("Nilai y =", y)


## Hasil Pengujian

<img width="613" height="215" alt="Tangkapan Layar 2026-09-03 pukul 13 51 08" src="https://github.com/user-attachments/assets/4e8e3a25-ab73-4db6-832a-f9a23e361add" />

<img width="617" height="214" alt="Tangkapan Layar 2026-09-03 pukul 13 52 15" src="https://github.com/user-attachments/assets/0f7c65c6-b1c9-4f89-ba7d-d06f32b6c431" />
