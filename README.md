# modul praktikum 4
Nama:ghefira azka fardani 

Kelas:TI.24.A5

NIM: 312410521

## latihan  

### - code program
```phython
list_A = [10, 20, 30, 40, 50]
```
Ini adalah list pertama yang berisi 5 elemen dengan nilai ```[10, 20, 30, 40, 50]```. 
Elemen-elemen ini akan dimanipulasi dalam beberapa langkah berikutnya.
```phython
print("Elemen ke 3:", list_A[2])
```
Di sini, kamu mengakses elemen ketiga dalam list ```list_A```. Perlu diingat bahwa Python menggunakan indeks berbasis nol, 
artinya indeks pertama adalah 0. Jadi, ```list_A[2]``` mengacu pada elemen ke-3, yang nilainya adalah ```30```.

Hasil yang ditampilkan adalah:
```phython
Elemen ke 3: 30
```
```phython
print("Elemen ke 2 sampai ke 4:", list_A[1:4])
```
Ini mengambil elemen mulai dari indeks 1 (elemen kedua) hingga indeks 3 (elemen keempat).
Karena ```list_A[1:4]``` akan mencakup elemen pada indeks 1, 2, dan 3 (elemen kedua, ketiga, dan keempat), hasilnya adalah ```[20, 30, 40]```.

Hasil yang ditampilkan:
```phython
Elemen ke 2 sampai ke 4: [20, 30, 40]
```
```phython
print("Elemen terakhir:", list_A[-1])
```
Di sini, kamu menggunakan indeks negatif untuk mengakses elemen terakhir dari list. 
Indeks ```-1``` selalu mengacu pada elemen terakhir dalam list, jadi ```list_A[-1]``` adalah ```50```. 

Hasil yang ditampilkan:
```phython
Elemen terakhir: 50
```
```phython
list_A[3] = 100
print("List setelah mengubah elemen ke 4:", list_A)
```
Pada langkah ini, elemen ke-4 dalam list (indeks 3) yang sebelumnya bernilai ```40``` diganti menjadi ```100```. Setelah perubahan, ```list_A``` menjadi:
```phython
[10, 20, 30, 100, 50]
```
hasil yang di tampilkan:
```phython
List setelah mengubah elemen ke 4: [10, 20, 30, 100, 50]
```
```phython
list_A[3:] = [200, 300]
print("List setelah mengubah elemen ke 4 sampai terakhir:", list_A)
```
ini, kamu mengganti semua elemen dari indeks 3 hingga akhir list dengan nilai baru ```[200, 300]```.
Sehingga, bagian ```list_A[3:]``` yang sebelumnya ```[100, 50]``` diganti dengan ```[200, 300]```. 

Hasilnya adalah:
```phython
[10, 20, 30, 200, 300]
```
hasil yang di tampilkan
```phython
List setelah mengubah elemen ke 4 sampai terakhir: [10, 20, 30, 200, 300]
```
```phython
list_B = list_A[0:2]
print("List B dari list A:", list_B)
```
Di sini, kamu membuat ```list_B``` yang berisi dua elemen pertama dari ```list_A```, yaitu ```10```dan ```20```.
Bagian yang diambil adalah dari indeks 0 hingga 1 (indeks 2 tidak disertakan).

Hasilnya adalah:
```phython
[10, 20]
```
hasil yang di tampilkan:
```phython
List B dari list A: [10, 20]
```
```phython
list_B.append("Hello")
print("List B setelah menambah string:", list_B)
```
Dengan menggunakan metode ```append()```, kamu menambahkan elemen ```"Hello"``` ke dalam ```list_B```. List ```list_B``` sebelumnya adalah ```[10, 20]```,
dan setelah penambahan ```"Hello"```, menjadi:
```phython
[10, 20, "Hello"]
```
hasil yang di tampilkan:
```phython
List B setelah menambah string: [10, 20, 'Hello']
```
```phython
list_B.extend([60, 70, 80])
print("List B setelah menambah 3 nilai:", list_B)
```
Metode ```extend()``` digunakan untuk menambahkan beberapa elemen ke dalam list.
Di sini, ```[60, 70, 80]``` ditambahkan ke l```ist_B```. Sebelumnya list_B adalah ```[10, 20, "Hello"]```, setelah penambahan elemen-elemen tersebut menjadi:
```phython
[10, 20, "Hello", 60, 70, 80]
```
hasil yang dii tampilkan:
```phython
List B setelah menambah 3 nilai: [10, 20, 'Hello', 60, 70, 80]
```
```phython
list_combined = list_A + list_B
print("List gabungan A dan B:", list_combined)
```
Di sini, kamu menggabungkan ```list_A``` dan ```list_B``` menggunakan operator ```+```. 
Sebelumnya, ```list_A``` adalah ```[10, 20, 30, 200, 300]``` dan ```list_B``` adalah ```[10, 20, "Hello", 60, 70, 80]```, jadi setelah penggabungan, hasilnya adalah:
```phthon
[10, 20, 30, 200, 300, 10, 20, 'Hello', 60, 70, 80]
```
hasil yang di tampilkan:
```phython
List gabungan A dan B: [10, 20, 30, 200, 300, 10, 20, 'Hello', 60, 70, 80]
```
### - hasil
![foto](https://github.com/azkaa-pixel/praktikum-4/blob/6fb0b79cff5cc4efc10afcc033cad813705af152/lat%20praktikum%204%20.jpg)

## praktikum 4

### - flowchart
![foto](https://github.com/azkaa-pixel/praktikum-4/blob/be0d4e9b32a6c73ca8703de02034ac54c359730e/praktikum%204.png)
### - code program
#### fungsi ```tambah_data```
```phython
def tambah_data():
  nama = input("Nama: ")
  nim = int(input("NIM: "))
  nilai_tugas = int(input("Nilai Tugas: "))
  nilai_uts = int(input("Nilai UTS: "))
  nilai_uas = int(input("Nilai UAS: "))
  data = {"Nama": nama, "NIM": nim, "Nilai Tugas": nilai_tugas, "Nilai UTS": nilai_uts, "Nilai UAS": nilai_uas}
  return data
```
Fungsi ini digunakan untuk meminta input data mahasiswa. Program akan meminta user untuk memasukkan:

~ Nama (tipe data string)

~ NIM (tipe data integer)

~ Nilai Tugas (tipe data integer)

~ Nilai UTS (tipe data integer)

~ Nilai UAS (tipe data integer)

Data yang dimasukkan kemudian akan dimasukkan ke dalam dictionary (```data```) dengan key-value pasangan seperti ```Nama: nama```, ```NIM: nim```, dll.
Fungsi ini akan mengembalikan dictionary tersebut sebagai output.
```
fungsi ```hitung_akhir(data)```
```phython
def hitung_akhir(data):
  nilai_akhir = (data["Nilai Tugas"] + data["Nilai UTS"] + data["Nilai UAS"]) / 3
  return nilai_akhir
```
Fungsi ini menerima parameter ```data``` (yang berisi dictionary dengan data mahasiswa). Fungsi ini menghitung nilai akhir mahasiswa dengan rumus rata-rata dari nilai tugas, UTS, dan UAS.

Rumus perhitungan nilai akhir adalah:


Nilai Tugas + Nilai UTS + Nilai UAS : 3
​
 
Nilai akhir ini kemudian akan dikembalikan dalam bentuk angka desimal.

#### Fungsi ```tampilkan_data(data_list)```
```python
def tampilkan_data(data_list):
  print("| No | Nama | NIM | Tugas | UTS | UAS | Akhir |")
  for i, data in enumerate(data_list):
    print(f"| {i+1} | {data['Nama']} | {data['NIM']} | {data['Nilai Tugas']} | {data['Nilai UTS']} | {data['Nilai UAS']} | {hitung_akhir(data):.2f} |")
```
Fungsi ini digunakan untuk menampilkan semua data yang telah dimasukkan ke dalam ```data_list```.
Data mahasiswa yang ada di dalam list akan ditampilkan dalam bentuk tabel dengan format sebagai berikut:

| No | Nama | NIM | Tugas | UTS | UAS | Akhir |

Fungsi ini menggunakan ```enumerate(data_list)``` untuk mengakses setiap item dalam ```data_list``` beserta nomor urutnya (```i```).
Dalam setiap baris tabel, data mahasiswa ditampilkan, termasuk nilai tugas, UTS, UAS, dan nilai akhir yang dihitung menggunakan fungsi ```hitung_akhir(data)```.

Nilai akhir akan ditampilkan dengan dua angka di belakang koma menggunakan format ```:.2f```.
#### bagian utama program 
```phython
data_list = []
while True:
  print("\n-- Tampilan Program --")
  print("Tambah data(y/t)?", end="")
  pilihan = input()
  if pilihan.lower() == "y":
    data_list.append(tambah_data())
    tampilkan_data(data_list)
  elif pilihan.lower() == "t":
    break
  else:
    print("Pilihan tidak valid.")
```
Di bagian ini, program akan berjalan dalam loop yang memungkinkan pengguna untuk menambah data mahasiswa secara berulang-ulang.

1. data_list = []: Membuat list kosong yang akan menampung data mahasiswa.

2. while True: Memulai loop yang akan terus berjalan hingga pengguna memilih untuk keluar.

3. Tambah data(y/t)?: Program meminta input dari pengguna untuk menentukan apakah mereka ingin menambah data mahasiswa lagi (```y``` untuk ya, ```t``` untuk tidak).

4. Jika pengguna memilih 'y', program akan memanggil fungsi ```tambah_data()```, yang meminta input data mahasiswa dan menambahkannya ke dalam ```data_list```. Setelah itu, fungsi ```tampilkan_data(data_list)``` akan dipanggil untuk menampilkan semua data yang sudah dimasukkan.

5.Jika pengguna memilih 't', program akan keluar dari loop dan berhenti.

6.Jika pengguna memasukkan pilihan selain 'y' atau 't', program akan menampilkan pesan "Pilihan tidak valid." dan meminta input lagi.
#### alur program
1. Program dimulai dan menampilkan pilihan untuk menambah data.

2. Jika pengguna memilih untuk menambah data, maka fungsi tambah_data() dipanggil untuk meminta input data mahasiswa dan menyimpannya dalam data_list.

3. Program kemudian menampilkan semua data mahasiswa yang sudah dimasukkan beserta nilai akhir setiap mahasiswa.

4. Program akan terus meminta input untuk menambah data sampai pengguna memilih untuk berhenti dengan memasukkan 't'.
#### contoh penggunaan 
``` phython
-- Tampilan Program --
Tambah data(y/t)? y
Nama: John Doe
NIM: 123456
Nilai Tugas: 80
Nilai UTS: 85
Nilai UAS: 90

| No | Nama     | NIM     | Tugas | UTS  | UAS  | Akhir |
| 1  | John Doe | 123456  | 80    | 85   | 90   | 85.00 |
```
Jika pengguna memilih 't', program akan berhenti.

### - hasil
![foto](https://github.com/azkaa-pixel/praktikum-4/blob/6fb0b79cff5cc4efc10afcc033cad813705af152/tugas%20praktikum%204.jpg)
