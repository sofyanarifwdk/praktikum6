### PRAKTIKUM 5

### Dictionary Input Nilai Mahasiswa

### <b>Penjelasan Program<b>

### Code program
![scrip1](https://user-images.githubusercontent.com/79274212/204124760-5cb61073-e4cc-414a-b806-b0fcd27fedea.png)

1.  Pertama kita ketik l pada menu pilihan untuk melihat daftar nilai :
<img src="img/output1.PNG" alt="img1" width="578" height="267">

2.  Kedua kita ketik 't' pada menu untuk menambahkan data baru :
<img src="img/output2.PNG" alt="img2" width="578" height="267">

    #   gambar inputan yang telah di tambahkan sebanyak 2 kali :
<img src="img/output3.PNG" alt="img3" width="600" height="280">

3.  Ketiga kita ketik 'c' pada menu untuk mencari data :
<img src="img/outputCari.PNG" alt="imgcari" width="600" height="163">

4.  Empat kita ketikan 'u' pada menu untuk mengubah data yang ada :
<img src="img/outputUbah.PNG" alt="imgubah" width="650" height="442">

5.  Kelima kita ketikan 'h' pada menu untuk menghapus data :
<img src="img/outputHapus.PNG" alt="imghapus" width="600" height="205">

### Flowchart
![flowchart](https://user-images.githubusercontent.com/79274212/204124752-d8a8672b-b6eb-475b-99d6-99b97012397b.png)

    # Note flowchart
    1   while True:
    2   c = input("(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar: ")
    3   if c.lower() == 'k':
    4   elif c.lower() == 'l':
    5   print daftar nilai i=0
    6   for x in data.items(): i+=1
    7   print (" | {6:2} | {0:9s} | {1:11} | {2:6d} | {3:6d} | {4:6d} | {5:6.2f} |"
    .format(x[0], x[1][0], x[1][1], x[1][2], x[1][3], x[1][4], i))
    8   elif c.lower() == 't':
    9   input nama = input(" Nama : ") nim = input(" NIM : ") nilaiuts = int(input(" Nilai UTS : ")) nilaiuas = int(input(" Nilai UAS : ")) nilaitgs = int(input(" Nilai TUGAS : "))
    10  akhir = (nilaitgs * 30/100 + nilaiuts * 35/100 + nilaiuas * 35/100) data[nama] = nim, nilaitgs, nilaiuts, nilaiuas, akhir
    11  elif c.lower() == 'u':
    12  input nama :
    13  if nama in data.keys(): nim = input("NIM : ") nilaiuts = int(input("Nilai UTS : ")) nilaiuas = int(input("Nilai UAS : ")) nilaitgs = int(input("Nilai TUGAS : ")) akhir = (nilaitgs * 30/100 + nilaiuts * 35/100 + nilaiuas * 35/100) data[nama] = nim, nilaitgs, nilaiuts, nilaiuas, akhir
    14  else: print("Data {0} tidak ada".format(nama))
    15  elif c.lower() == 'h':
    16  input nama :
    17  if nama in data.keys():
    18  del data[nama]
    19  else: print("Data {0} tidak ada".format(nama))
    20  elif c.lower() == 'c':
    21  input nama :
    22  if nama in data.keys(): print (" daftar nilai ") print (" | {0:9s} | {1:11} | {2:6d} | {3:6d} | {4:6d} | {5:6.2f} |"
    .format(nama, nim, nilaitgs, nilaiuts, nilaiuas, akhir))
    23  else: print("Data {0} tidak ada".format(nama))
    24  else: print("Pilih menu yang tersedia")

