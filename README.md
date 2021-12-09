# tugas-pertemuan-10
# soal latihan 1
![soal tugas 10](https://user-images.githubusercontent.com/93035757/145330134-898c625c-1d42-4c3e-9cc8-7dcdbddf322c.png)
# coding dan output
![Capture tugas 1 pertemuan 10](https://user-images.githubusercontent.com/93035757/145330613-ed3ab907-9d38-4783-8e1a-dcaa90a05fee.PNG)


# soal tugas praktikum
![soal praktikum](https://user-images.githubusercontent.com/93035757/145330909-59ee0a9e-ba7e-4c4f-9a73-4fadb1494db6.png)
langkah pertama saya membuat looping agar program terus berjalan

while True:
    c = input("\n(L)ihat, (T)ambah, (U)bah, (H)apus, (C)ari, (K)eluar: ")                                

lalu saya membuat format if untuk memasukan pilihan , sebagai contoh apabila memilih (t) akan menambah data

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

kemudian saya juga melakukan percabangan if (elif) untuk melaksanakan pilihan yang lain

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

yang terakhir saya juga menggunakan else untuk apabila salah memasukan pilihan inputan
    else:
    print("Pilih menu yang tersedia: ")
    
   # output dan coding
   ![Capture 1](https://user-images.githubusercontent.com/93035757/145332109-2f9479dc-c50f-473a-96e9-c78835687140.PNG)

![Capture 2](https://user-images.githubusercontent.com/93035757/145332423-39eee87a-ed59-47db-b05b-1ab8405b8277.PNG)

