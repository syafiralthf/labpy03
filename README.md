# Biodata

### Nama = Syafira Luthfi Azzahra

### Kelas = TI.24.A.4

### NIM = 321410353

# Soal Latihan

![Cuplikan layar 2024-10-30 201541](https://github.com/user-attachments/assets/4ae7e6ce-b0e8-445a-b424-51e3bb16eecd)

# Latihan 1.py

```python
import random

n = int(input("Masukkan nilai N: "))

for i in range(1, n+1):
  angka_acak = random.random()
  print(f"data ke: {i} => {angka_acak}")

print("Selesai")
```

```python
import random
```

Baris ini mengimpor modul random, yang berisi fungsi-fungsi untuk menghasilkan angka acak.

```python
n = int(input("Masukkan nilai N: "))
```

Pengguna meminta untuk memasukkan nilai integer ```n``` yang menentukan berapa banyak angka acak yang akan dihasilkan. Fungsi ```input()``` menerima masukan dari pengguna dalam bentuk string, dan ```int()``` mengonversinya menjadi integer.

```python
for i in range(1, n + 1):
```

```for``` adalah perulangan yang akan berjalan sebanyak N kali, ```range(1, n + 1)``` menghasilkan urutan angka mulai dari 1 hingga ```N``` (termasuk ```N```), yang digunakan untuk menentukan jumlah angka acak yang akan dihasilkan.

```python
angka_acak = random.random()
print(f"data ke: {i} => {angka_acak}")
```

Di dalam perulangan, ```random.random()``` digunakan untuk menghasilkan angka acak dalam rentang 0.0 hingga 1.0, dengan nomor urut datanya (```data ke: {i}```). Format ```{i}``` dan {angka_acak} digunakan dalam ```f-string``` untuk menampilkan nilai variabel ```i``` dan ```angka_acak``` secara langsung di dalam string.

```python
print("Selesai")
```

Setelah perulangan selesai, baris ini menampilkan pesan ```"Selesai"``` untuk menandakan bahwa program telah selesai menjalankan seluruh instruksi.

Pengguna meminta untuk memasukkan nilai integer ```n``` yang menentukan berapa banyak angka acak yang akan dihasilkan. Fungsi ```input()``` menerima masukan dari pengguna dalam bentuk string, dan ```int()``` mengonversinya menjadi integer.

```python
for i in range(1, n + 1):
```

```for``` adalah perulangan yang akan berjalan sebanyak N kali, ```range(1, n + 1)``` menghasilkan urutan angka mulai dari 1 hingga ```N``` (termasuk ```N```), yang digunakan untuk menentukan jumlah angka acak yang akan dihasilkan.

```python
angka_acak = random.random()
print(f"data ke: {i} => {angka_acak}")
```

Di dalam perulangan, ```random.random()``` digunakan untuk menghasilkan angka acak dalam rentang 0.0 hingga 1.0, dengan nomor urut datanya (```data ke: {i}```). Format ```{i}``` dan {angka_acak} digunakan dalam ```f-string``` untuk menampilkan nilai variabel ```i``` dan ```angka_acak``` secara langsung di dalam string.

```python
print("Selesai")
```

Setelah perulangan selesai, baris ini menampilkan pesan ```"Selesai"``` untuk menandakan bahwa program telah selesai menjalankan seluruh instruksi.

![Cuplikan layar 2024-10-31 202049](https://github.com/user-attachments/assets/9dd7916e-60dc-43f9-a8c7-e4292f16dcd5)

# Latihan 2.py

```python
# Inisialisasi modal awal
modal_awal = 100000000

# Inisialisasi daftar laba untuk setiap bulan
laba = [0, 0, 0, 0, 0, 0, 0, 0]

# Menghitung laba untuk setiap bulan
laba[2] = modal_awal * 0.01  # Laba bulan ke-3 sebesar 1%
laba[4] = laba[2] * 1.05     # Laba bulan ke-5 meningkat 5% dari bulan ke-3
laba[7] = laba[4] * 0.98     # Laba bulan ke-8 turun 2% dari bulan ke-5

# Menghitung total laba
total_laba = sum(laba)

# Mencetak hasil
print("Laba bulan ke-1 sebesar:", laba[0])
print("Laba bulan ke-2 sebesar:", laba[1])
print("Laba bulan ke-3 sebesar:", laba[2])
print("Laba bulan ke-4 sebesar:", laba[3])
print("Laba bulan ke-5 sebesar:", laba[4])
print("Laba bulan ke-6 sebesar:", laba[5])
print("Laba bulan ke-7 sebesar:", laba[6])
print("Laba bulan ke-8 sebesar:", laba[7])
print("Total laba adalah:", total_laba)
```

```python
modal_awal = 100000000
```

Modal awal ditetapkan sebesar 100 juta rupiah.

```python
laba = [0, 0, 0, 0, 0, 0, 0, 0]
```

Array ```laba``` dibuat untuk menyimpan laba bulanan selama 8 bulan, dengan nilai awal 0 untuk semua bulan.

```python
laba[2] = modal_awal * 0.01  
laba[4] = laba[2] * 1.05     
laba[7] = laba[4] * 0.98
```

laba dihitung sebesar 1% dari ```modal_awal```, yaitu 1 juta rupiah, laba meningkat sebesar 5% dari laba bulan ke-3. Nilainya menjadi 1,05 juta rupiah, laba mengalami penurunan sebesar 2% dari laba bulan ke-5. Nilai laba bulan ke-8 adalah 1,029 juta rupiah.

```python
total_laba = sum(laba)
```

Fungsi ```sum()``` digunakan untuk menjumlahkan semua nilai dalam array ```laba```, yang menghasilkan total laba selama 8 bulan.

```python
print("Laba bulan ke-1 sebesar:", laba[0])
```

Baris-baris ini mencetak laba untuk masing-masing bulan, dan total laba.

Hasil program tersebut:

![Cuplikan layar 2024-10-31 204704](https://github.com/user-attachments/assets/9cf63cb9-8957-44e2-9f40-c6c6b77c6f8b)

# Latihan 3.py

```python
saldo = 1000000

while True:
  print(f"Saldo saat ini: Rp {saldo}")
  print("1. Tarik Uang")
  print("2. Keluar")

  pilihan = input("Pilih menu (1/2): ")

  if pilihan == "1":
    jumlah = int(input("Masukkan jumlah penarikan: "))
    if jumlah <= saldo:
      saldo -= jumlah
      print("Penarikan berhasil!")
    else:
      print("Saldo tidak cukup!")
  elif pilihan == "2":
    print("Terima kasih telah menggunakan ATM BTN!")
    break
  else:
    print("Pilihan tidak valid!")
```

```python
saldo = 1000000
```

Saldo awal pengguna diatur sebesar 1 juta rupiah.

```python
while True:
```

Loop ```while True``` digunakan agar program terus berjalan hingga pengguna memilih opsi untuk keluar ```(break)```

```python
print(f"Saldo saat ini: Rp {saldo}")
print("1. Tarik Uang")
print("2. Keluar")
```

Setiap kali loop berjalan, saldo saat ini akan ditampilkan, bersama dengan dua pilihan menu: Tarik Uang (1) atau Keluar (2).

```python
pilihan = input("Pilih menu (1/2): ")
```

Program meminta pengguna untuk memilih antara opsi Tarik Uang atau Keluar.

```python
if pilihan == "1":
    jumlah = int(input("Masukkan jumlah penarikan: "))
```

Pengguna akan diminta memasukkan jumlah uang yang ingin ditarik, kemudian memeriksa apakah jumlah yang diminta kurang dari atau sama dengan saldo saat ini

```python
if jumlah <= saldo:
```

Jika Benar: Jumlah tersebut dikurangi dari saldo, dan pesan Penarikan berhasil! akan ditampilkan. Jika Tidak Cukup: Program menampilkan pesan Saldo tidak cukup!

```python
elif pilihan == "2":
    print("Terima kasih telah menggunakan ATM BTN!")
    break
```
Jika pengguna memilih "2", pesan Terima kasih telah menggunakan ATM BTN! akan ditampilkan, dan program akan keluar dari loop dengan perintah ```break```.

```python
else:
    print("Pilihan tidak valid!")
```

Jika input pengguna tidak sesuai dengan opsi yang ada (1 atau 2), maka program akan menampilkan pesan Pilihan tidak valid!

Hasil program tersebut:

![Cuplikan layar 2024-10-31 210556](https://github.com/user-attachments/assets/70b87ca7-658e-46cd-8ec6-f8dc4a2afd84)
