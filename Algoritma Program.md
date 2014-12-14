Algoritma Program
=================
Tulisan ini ditulis untuk menambahkan bagian `Bab 3` Pada Algoritma Program. List penambahan Algoritma Program Bisa terangkum dalam :

* Algoritma `Menu Utama`
* Algoritma `Form Generate Kunci`
* Algoritma `Form Log Aktivitas`
* Algoritma `Form Enkripsi`
* Algoritma `Form Dekripsi`
* Algoritma `Form User`
* Algoritma Proses `Generate Kunci`
* Algoritma Proses `Enkripsi`
* Algoritma Proses `Dekripsi`

##1. Algoritma Menu Utama
Algoritma ini menjelaskan proses Menu Utama yang terdiri dari `Generate Kunci`, `Aktivitas`, `Enkripsi`, `Dekripsi`, `User` dan `Bantuan`. Apabila memilih Menu Enkripsi maka akan muncul Form Enkripsi. Begitu juga menu Dekripsi, jika dipilih akan menampilkan Menu Form Dekripsi. Apabila memilih menu Aktivitas maka akan tampil Form Aktivitas, Apabila memilih menu User maka akan tampil Form User. Namun, bila yang dipilih Bantuan maka akan tampil Form Bantuan.

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

##2. Algoritma Form Generate Kunci
Algoritma Form Generate Kunci ini akan menjelaskan penggunaan untuk melakukan pembuatan kunci oleh user.

```
1.	Tampil Form Generate Kunci
2.	Input Direktori
3.	Input Id Kantor Cabang
4.	Input Id Kantor Pusat
5.	Input Pilih
6.	If Pilih == Generate Kunci Then:
7.		If Lengkap ? Then:
8.			Proses Generate Kunci RSA
9.			Pesan Sukses
10.		Else:
11.			Pesan Error
12.	Elif Pilih == Bersih Then:
13.		Bersihkan Form
14.	End If
```

##3. Algoritma Form Log Aktivitas
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

##4. Algoritma Form Enkripsi
Algoritma ini menjelaskan penggunaan form Enkripsi untuk melakukan Enkripsi dokumen dengan format xls dan doc.

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

##5. Algoritma Form Dekripsi
Algoritma ini menjelaskan penggunaan form dekripsi. Penggunaan form dekripsi yaitu kebalikan dari penggunaan form Enkripsi.

```
1.  Tampil Form Dekripsi
2.  Input File
3.  Input Direktori
4.  Input File Kunci Private
5.  Input Pilih
6.  If Pilih == Dekripsi Then:
7.  	If File != Kosong Then:
8.			Status = Lengkap
9.		Elif Direktori != Kosong Then:
10.			Status = Lengkap
11.		Elif File Kunci Private != Kosong Then:
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

##6. Algoritma User
Algoritma Form User ini menjelaskan bagaimana User menambahkan nilai identitas karyawan pada kantor cabang dan kantor pusat.

```
1.  Tampil Form User
2. 	Baca File Kantor.conf
3.	Tampilkan isi File Kantor.conf saat ini ke List
4.  Input Identitas
5.  Input Pilihan
6.  If Pilihan == Tambah Then:
7.		If Identitas == Kosong Then:
8.			Tampil Warning
9.			Kembali ke Baris 2
10.		Else:
11.   		Tambahkan Identitas Ke List
12.		End If
13.	End If
14.	Input Pilih
15.	If Pilih == Simpan Then:
16.		If List == Kosong Then:
17.			Tampil Pesan Error
18.			Kembali ke Baris 2
19.		Else:
20.			Baca File Kantor.conf
21.			Ambil Data List
22.			Tulis Ulang File Kantor.conf dengan Data List
23.			Simpan File Kantor.conf
24.		End If
25.	End If

```

##7. Algoritma Proses Generate Kunci
Algoritma proses `generate kunci` ini menjelaskan cara kerja `Algoritma RSA` untuk melakukan proses pembuatan `kunci publik` dan `kunci private`.

```
1.	Proses Generate Kunci RSA
2.	Inisialisasi P = Random Prima
3.	Inisialisasi Q = Random Prima
4.
5.	If P == Q Then:
6.		Kembali ke Baris 1
7.	End If
8.
9.	N 	= P * Q
10.	PHI = (P - 1) (Q - 1)
11.	cari E dimana GCD(E, PHI) = 1
12.	cari D 	dimana (D * E) mod PHI == GCD(E, PHI)
13.
14.	Kunci Publik 	= E dan N
15.	Kunci Private 	= D dan N
```

##8. Algoritma Proses Enkripsi
Algoritma proses enkripsi ini menjelaskan cara kerja Algoritma RSA untuk melakukan proses enkripsi dari file berformat xls dan doc.
```
1.	Proses Enkripsi
2.	Inisialisasi E = 0
3.	Inisialisasi N = 0
4.	Inisialisasi data = []
5.	Inisialisasi Chiper = []
6.
7.	Open Kunci Publik RSA mode Read:
8.		 N = Modulo N
9.		 E = Eksponen E
10.	Close File
11.
12.	Open File XLS atau DOC mode Read:
13.		data = File Byte XLS or DOC
14.	Close File	
15.
16.	For I in range data Then:
17.		Chiper Append To data ke I ^ E mod N
18.	End For
19.
20.	Open File XLS atau DOC mode Write:
21.		Mencoba:
22.			For I in data:
23.				Tulis XLS or DOC dengan data ke I
24.			End For
25.     Message Box Sukses
26.		Mengalihkan:
27.			Pesan Box Error
28.	Close File
```

##9. Algoritma Proses Dekripsi
Algoritma proses dekripsi ini menjelaskan bagaimana mengembalikan data yang sudah dienkripsi menjadi file asli dengan metode Algoritma RSA menggunakan kunci private. dimana untuk memulai proses dekripsi, user wajib menyertakan file kunci rahasia sebagai kunci private.
```
1.	Proses Dekripsi
2.	Inisialisasi D = 0
3.	Inisialisasi N = 0
4.	Inisialisasi data = []
5.	Inisialisasi Plain = []
6.
7.	Open Kunci Private RSA mode Read:
8.		 N = Modulo N
9.		 D = Dksponen D
10.	Close File
11.
12.	Open File XLS atau DOC mode Read:
13.		data = File Byte XLS or DOC
14.	Close File	
15.
16.	For I in range data Then:
17.		Plain Append To data ke I ^ D mod N
18.	Dnd For
19.
20.	Open File XLS atau DOC mode Write:
21.		Mencoba:
22.			For I in data:
23.				Tulis XLS or DOC dengan data ke I
24.			Dnd For
25.     Message Box Sukses
26.		Mengalihkan:
27.			Pesan Box Drror
28.	Close File
```
