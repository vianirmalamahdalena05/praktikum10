# PERTEMUAN 10

| Variable | Isi |
| -------- | --- |
| **Nama** | Via Nirmala  |
| **NIM** | 312310484 |
| **Kelas** | TI.23.A5 |
| **Mata Kuliah** | Bahasa Pemrograman |

# Latihan
* membuat kontak awal / ```b = {'ari' : '085267888', 'dina' : 087677776}```
* menampilkan kontak ari /  ```print(b['ari'])```
* menambhkan kontak riko /  ```b['riko']= 087888999```
* mengubah kontak dina / ```b['dina]= '089555777```
* menampilkan semua nama / ```print(b.keys())```
* menampilkan semua nomor / ```print(b.values())```
* menampilkan semua nama dan nomor / ```print(b)```
* menghapus kontak dina / ```del b['dina']```

## Berikut adalah codingan programnya
```python


b={'ari':'085267888','dina':'087677776'}
print('Daftar Kontak')
print('==============================')
print('    nama    |   nomor telepon')
print('==============================')
print('1.    ari   |   085267888','\n2.    dina    |   087677776')

# tamprintilkan kontak ari
print('\nTampilkan Kontak Ari')
print('1.    ari      |   ',b['ari'])
# Tambahkan riko ke kontak
print('\nMenambah Kontak Riko')
b['riko']='087654544'
print('1.   ari      |   ',b['ari'])
print('2.   dina     |   ',b['dina'])
print('3.   riko     |   ',b['riko'])
# Ubah Nomor dina ke nomor baru 
print('\nMengubah nomor Dina ke')
b['dina']='088999776'
print('1.   ari      |   ',b['ari'])
print('2.   dina     |   ',b['dina'])
print('3.   riko     |   ',b['riko'])
# Tampilkan semua nama
print('\nMenampilkan semua nama')
print(b.keys())
# Tampilkan semua nomor
print('\nMenampilkan semua nomor')
print(b.values())
# Tampilkan semua nama dan nomor
print('\nMenampilkan semua nama dan nomor')
print(b)
# Hapus kontak dina
print('\nMenghapus kontak dina')
del b['dina']
print(b,'\n')
```

## Berikut adalah hasil perogramnya
<img width="332" alt="Screenshot 2023-11-28 145141" src="https://github.com/vianirmalamahdalena05/praktikum10/assets/147572078/7bec1008-ad62-4add-ac55-b689d8e06c67">
<img width="439" alt="Screenshot 2023-11-28 145111" src="https://github.com/vianirmalamahdalena05/praktikum10/assets/147572078/0214d5e5-b041-4a34-a99e-a6086a2f8a2c">


# Tugas Praktikum
_program sederhana yang akan menampilkan daftar nilai mahasiswa_
## Flowchart
<img width="313" alt="Screenshot 2023-11-28 151511" src="https://github.com/vianirmalamahdalena05/praktikum10/assets/147572078/baebbd85-7004-458d-a8a9-99eeac719b17">

1. membuat lopping agar program terus berjalan:
```python
sh while True :
    c = input("\n(L)ihat, (T)ambah,(U)bah, (C)ari, (K)eluar): ")
```
2. membuat formatif if untuk memasukan pilihan , contoh pilihan (t): \
```python
if (c.lower() == 't'):                                               
     print('\nTambah Data Mahasiswa Baru')
        nama= input("Masukkan Nama\t\t: ")                                        
        nim= input("Masukkan NIM\t\t: ")                                         
        nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))                              
        nilaiUts= int(input("Masukkan Nilai UTS\t: "))                                   
        nilaiUas= int(input("Masukkan Nilai UAS\t: "))                                    
        nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)              
        dataMhs[nama]= nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir                         
        print("\nData Berhasil Ditambahkan!")
```

3. membuat percabangan elif untuk menjalankan pilihan yang lain
```python
elif (c.lower() == 'u'):                                                                    
        print('\nMengedit Data Mahasiswa')
        nama = input("Masukkan Nama: ")                                                         
        if nama in dataMhs.keys():                              
            nim= input("Masukkan NIM Baru\t: ")                              
            nilaiTugas= int(input("Masukkan Nilai Tugas\t: "))                           
            nilaiUts= int(input("Masukkan Nilai UTS\t: "))                           
            nilaiUas= int(input("Masukkan Nilai UAS\t: "))                           
            nilaiAkhir= (0.30 * nilaiTugas) + (0.35 * nilaiUts) + (0.35 * nilaiUas)          
            dataMhs[nama] = nim, nilaiTugas, nilaiUts, nilaiUas, nilaiAkhir                      
            print("\nData Berhasil Di Update!")
```
4. menggunakan else apabila salah memasukan pilihan 
```python
else:
        print("Pilih menu yang tersedia: ")
```
### Output untuk (T) :
<img width="409" alt="Screenshot 2023-11-28 144550" src="https://github.com/vianirmalamahdalena05/praktikum10/assets/147572078/c533a3e8-f557-461e-85c5-4824edbce888">

### Output untuk (U) :
<img width="400" alt="Screenshot 2023-11-28 144603" src="https://github.com/vianirmalamahdalena05/praktikum10/assets/147572078/e9c7169f-acbe-45f2-ad65-3cdfcb2e58b9">

### Output untuk (L) :
<img width="450" alt="Screenshot 2023-11-28 144615" src="https://github.com/vianirmalamahdalena05/praktikum10/assets/147572078/377db7f0-2025-4562-93de-bc0f06f47b31">

### Output untuk (C) :
![image](https://github.com/vianirmalamahdalena05/praktikum10/assets/147572078/19d22645-d6b7-4b9f-8d99-b1c0a25e5c28)

### Output untuk (H) :
<img width="440" alt="Screenshot 2023-11-28 144641" src="https://github.com/vianirmalamahdalena05/praktikum10/assets/147572078/98fa88a9-f3a2-43ab-9200-e1ec8b6d0dd4">


## Terima Kasih
