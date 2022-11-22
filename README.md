Nama  : Dhea Dwi Adelia

NIM   : 312210116

Kelas : TI.22.A.1

## Latihan
Buat sebuah list sebanyak 5 elemen dengan nilai bebas

#### Akses list :
- Tampilkan elemen ke 3
- Ambil nilai elemen ke 2 sampai elemen ke 4
- Ambil elemen terakhir
#### Ubah elemen list :
- Ubah elemen ke 4 dengan nilai lainnya
- Ubah elemen ke 4 sampai dengan elemen terakhir
#### Tambah elemen list :
- Ambil 2 bagian dari list pertama (A) dan jadikan list ke 2 (B)
- Tambah list B dengan nilai string
- Tambah list B dengan 3 nilai
- Gabungkan list B dengan list A

#### Langkah-langkah :
1. Buat programnya terlebih dahulu.

   # Latihan
print("Nama: Dhea Dwi Adelia")
print("NIM : 312210116")

print("Membuat List sebanyak 5 elemen dengan nilai bebas")
# akses list
a = [6, 9, 5, 8, 2]
print(a) #Menampilkan semua elemen
print(a[2]) #Menampilkan elemen ke 3
print(a[1:3]) #Menampilkan elemen ke 2 sampai dengan ke 4
print(a[4]) #Menampilkan elemen terakhir

print("==========================================")
# ubah elemen list
a[3] = 5 # Mengubah elemen ke 4 dengan nilai lainnya
print(a[3]) # Menampilkan elemen ke 4 yang sudah diubah nilainya
a[3:4] = 5, 8 # Mengubah elemen ke 4 sampai dengan elemen terakhir
print(a[3:5]) # menampilkan elemen ke 4 sampai dengan elemen terakhir

print("==========================================")
# tambah elemen list
b = a[0:2] # Mengambil 2 bagian dari list pertama (a) dan jadikan list kedua (b)
print(b)
b.append(10) # Menambah list dengan nilai string
print(b)
b.extend([1, 4, 11]) # Menambah list b dengan 3 nilai
print(b)
c = a+b # Menggabungkan list b dengan list a
print(c)
    ![Screenshot (110)](https://user-images.githubusercontent.com/115794875/203252664-ef3e1f91-2f60-4963-9003-7780741d6327.png)
    ![Screenshot (111)](https://user-images.githubusercontent.com/115794875/203252885-8b77e0a9-6b68-44c9-8130-9d31a467871c.png)

2. Hasil Run

![Screenshot (112)](https://user-images.githubusercontent.com/115794875/203253517-7275b06b-3156-447a-8f63-4ad80fc95212.png)

 
## Praktikum 5
Buat program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut :

- Program meminta memasukkan data sebanyak-banyaknya (gunakan perulangan)
- Tampilkan pertanyaan untuk menambah data (y/t?), apabila jawaban   
"t", maka program akan menampilkan daftar datanya.
- Nilai akhir diambil dari perhitungan 3 komponen nilai (tugas: 35%, uts: 25%, uas: 40%)
- Buat flowchart dan penjelasan programnya pada README.md.
- Commit dan push repository ke github.

#### Langkah-langkah :
1. Buat programnya terlebih dahulu

    # Membuat Tugas Praktikum
    data =[]
    while True :
        nama       = input    ("Nama        : ")
        nim        = input    ("NIM         : ")
        tugas      = int(input("Nilai Tugas : "))
        uts        = int(input("Nilai UTS   : "))
        uas        = int(input("Nilai UAS   : "))
        nilaiakhir = float(tugas)*35/100+(uts)*25/100+(uas)*40/100
        data.append([nama,nim,tugas,uts,uas,nilaiakhir])
        lagi= input("Tambah data (y/t)? ")
        if lagi.lower() =="t":
            break


    print("=====================================================================================");
    print("|  No  |     Nama     |     NIM     |   Tugas   |   UTS   |   UAS   |  Nilai Akhir  |");
    print("=====================================================================================");
    i=0
    for x in data:
        i+=1
        print("|  {6:2}  |  {0:10}  |  {1:9}  |  {2:7}  |  {3:5}  | {4:6}  |  {5:11.2f}  |"\
              .format (x[0][:9] , x[1][:9],x[2],x[3],x[4],x[5], i))
    print("=====================================================================================");
    
    ![Screenshot (115)](https://user-images.githubusercontent.com/115794875/203254753-7fe9e881-bbca-4d46-ac29-6aeb1f7afaad.png)

    
2. Hasil Run

![Screenshot (116)](https://user-images.githubusercontent.com/115794875/203254835-160cdd8c-e206-4cb0-9496-bd9cff83786d.png)


### Penjelasan Program :
1. Buatlah list berupa Nama, NIM, Nilai Tugas, Nilai UTS, Nilai UAS.
2. Lalu inputlah Nama, NIM, Nilai Tugas, Nilai UTS, Nilai UAS.
3. Lalu mencari nilai akhir dengan perhitungan nilai tugas 35%, nilai uts 25% dan uas 40% , dengan perintah float
4. Gunakan perintah append pada Nama, NIM, Nilai tugas, Nilai UTS, Nilai UAS untuk menambahkan 1 item ke elemen terakhir.
5. Jika ingin menambah list data ketik "y" dan jika tidak ingin menambahkan list data ketik "t". Dengan perintah while jawab =="y" dan if jawab =="t". Jawab input("Tambah data (y/t)").
6. Gunakanlah perulangan for, dengan perintah for i in range(len(Nama)):. Fungsi "len" ialah untuk mengembalikan panjang (jumlah anggota) dari suatu objek.
7. Lalu cetak dengan perintah print
8. Selesai

### Flowchart Praktikum 5


### Sekian, Terima kasih 
