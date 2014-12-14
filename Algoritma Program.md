Algoritma Program
=================

##1. Algoritma Menu Utama
Algoritma ini menjelaskan proses Menu Utama yang terdiri dari Generate Kunci, Aktivitas, Enkripsi, Dekripsi, User dan Bantuan. Apabila memilih Menu Enkripsi maka akan muncul Form Enkripsi. Begitu juga menu Dekripsi, jika dipilih akan menampilkan Menu Form Dekripsi. Apabila memilih menu Aktivitas maka akan tampil Form Aktivitas, Apabila memilih menu User maka akan tampil Form User. Namun, bila yang dipilih Bantuan maka akan tampil Form Bantuan.

```
1.  Start
2.  Tampilkan Form Utama
3.  Input Pilih
4.  If Pilih == Generate Keys Then:
5.		Tampil Form Generate Key
6.  Elif Pilih == Aktivitas Then:
7.		Tampil Form Aktivitas
8.  Elif Pilih == Enkripsi Then:
9.		Tampil Form Enkripsi
10. Elif Pilih == Dekripsi Then:
11.		Tampil Form Dekripsi
12. Elif Pilih == User Then:
13. 	Tampil Form User
14. Elif Pilih == Bantuan Then:
15.		Tampil Form Bantuan
16. Else Then:
17.		Keluar
18. End If 
```

##2. Algoritma Form Log Aktivitas
Algoritma Form Log Aktivitas akan menampilkan semua aktivitas-aktivitas yang dilakukan user kepada Aplikasi, mulai dari proses Generate Kunci, Enkripsi hingga proses Dekripsi. Form Aktivitas memungkinkan user melihat serangkaian aktivitas yang dicatat oleh program dan bisa di ekspor ke dalam sebuah file berformat html.

```
1.  Tampil Form Log Aktivitas
2.  Tampil Data Log Aktivitas dalam bentuk tabel
3.  Input Pilih
4.  If Pilih == Ekspor Then:
5.		Input Direktori
6.		Mencoba:
7.			Ambil semua data List Tabel Log Aktivitas
8.			Tanggal = Tanggal Saat Ini
9.			Tulis Isi Data Log ke File HTML 
10.			Simpan File HTML dengan Nama File dari Tanggal saat ini
11.			Tampil Pesan Berhasil
12.		Mengalihkan:
13.			Tampil Pesan Error
14. Else:
15.		Kembali ke Baris 1		
16. End If		
```

##3. Algoritma Form Enkripsi
Algoritma ini menjelaskan penggunaan form Enkripsi untuk melakukan Enkripsi dokumen dengan format xls dan doc.
Algoritma proses enkripsi ini menjelaskan cara kerja Algoritma RSA untuk melakukan proses enkripsi dari file berformat xls dan doc.

```
1.  Tampil Form Enkripsi
2.  Input File
3.  Input Direktori
4.  Input File Kunci Publik
5.  Input Pilih
6.  If Pilih == Enkripsi Then:
7.  	If File != Kosong Then:
8.			Status = Lengkap
9.		Elif Direktori != Kosong Then:
10.			Status = Lengkap
11.		Elif File Kunci Publik != Kosong Then:
12.			Status = Lengkap
13.		Else:
14.			Status = Tidak Lengkap
15.		If Status == Lengkap Then:
16.			Proses Enkripsi
17.		Else:
18.			Tampil Pesan Data Tidak Lengkap
19.			Kembali ke Baris 1
20. End If
```

##4. Algoritma Dekripsi
Algoritma ini menjelaskan penggunaan form dekripsi. Penggunaan form dekripsi yaitu kebalikan dari penggunaan form Enkripsi.

Algoritma proses dekripsi ini menjelaskan bagaimana mengembalikan data yang sudah dienkripsi menjadi file asli dengan metode Algoritma RSA menggunakan kunci private. dimana untuk memulai proses dekripsi, user wajib menyertakan file kunci rahasia sebagai kunci private.

##5. Algoritma User
Algoritma User ini menjelaskan bagaimana User menambahkan nilai identitas karyawan pada kantor cabang dan kantor pusat.

##6. Algoritma 
