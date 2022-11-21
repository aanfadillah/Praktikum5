## Nama : Aan fadillah putra

## NIM : 312210327

## Kelas: TI.22.A3

# praktikum 5

## Tugas Praktikum 

Flowchart 





Gunakan _While_ untuk memasukkan data secara berulang berulang dan masukkan ```input()```

```
data = []
stop = False

while(not stop):
    nama = input("Nama : ")
    nim = input("NIM : ")
    tugas = int(input("Nilai Tugas : "))
    uts = int(input("Nilai UTS : "))
    uas = int(input("Nilai UAS : "))
    akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)
```

Gunakan ```.append()``` untuk menambahkan elemen ke list

    data.append([nama,nim,tugas,uts,uas,int(akhir)])

Untuk menetapkan 't' menjadi stop gunakan 

```
tanya = input('Tambahkan Data (y/t) ?')
    if (tanya == 't'):
        stop = True
```

lalu tampilkan elemen elemennya
    
```
print("==================================================================")
print("| No |     Nama     |    NIM    | Tugas |  UTS  |  UAS  |  Akhir |")
print("==================================================================")

i = 0

for nilai in data:
    i += 1
    print("| {no:2d} | {nama:12s} | {nim:5s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |".format(no=i, nama=nilai[0], nim=nilai[1], tugas=nilai[2],uts=nilai[3],uas=nilai[4],akhir=nilai[5]))

print("==================================================================") 
```

maka hasilnya akan menjadi 

![img.png](Picture/img2.0.png)
