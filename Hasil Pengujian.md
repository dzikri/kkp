1. Hasil Pengujian Program (Aplikasi)
==========================

File yang dibatasi hanya berlaku file `Doc` dan `XLS` dengan kapasitas size `<= 3Mib`.

##1.1 Enkripsi & Dekripsi File Document .doc

###1.1.1 Hasil Enkripsi File Doc

>>> Tampilan Layar File doc

![Alt text](http://yanwarrior.hol.es/kkp/1.JPG)

|Nama File doc|Modulo N|Eksponen E|Ukuran File|Waktu Enkripsi  (Detik)|Ukuran Hasil Enkripsi|
|:---:|:---:|:---:|:---:|:---:|:---:|
|file_doc1.doc   |149557   |47459   |24.5 KiB   |13 Detik   |88.4 KiB   |
|file_doc2.doc   |149557   |47459   |63 KiB   |49 Detik   |226 KiB   |
|file_doc3.doc   |149557   |47459   |151 KiB   |134 Detik   |620 KiB   |
|file_doc4.doc   |149557   |47459   |104 KiB   |90 Detik   |406 KiB   |

###1.1.2 Hasil Dekripsi File Doc

>>> Tampilan Layar File Enkripsi doc

![Alt text](http://yanwarrior.hol.es/kkp/2.JPG)

|Nama File Enkripsi doc|Modulo N|Eksponen D|Ukuran File (KiB)|Waktu Enkripsi  (Detik)|Ukuran Hasil Dekripsi (KiB)|
|:---:|:---:|:---:|:---:|:---:|:---:|
|enkripRSA-file_doc1.doc   |149557   |65479   |88.4 KiB  |16 Detik    |24.5 KiB   |
|enkripRSA-file_doc2.doc   |149557   |65479   |226 KiB   |49 Detik    |63 KiB   |
|enkripRSA-file_doc3.doc   |149557   |65479   |620 KiB   |202 Detik   |151 KiB   |
|enkripRSA-file_doc4.doc   |149557   |65479   |406 KiB   |159 Detik   |104 KiB   |

##1.2 Enkripsi & Dekripsi File Spreadsheet .xls

###1.2.1 Hasil Enkripsi File Xls

>>> Tampilan Layar File xls

![Alt text](http://yanwarrior.hol.es/kkp/3.JPG)

|Nama File xls|Modulo N|Eksponen E|Ukuran File (KiB)|Waktu Enkripsi  (Detik)|Ukuran Hasil Enkripsi (KiB)|
|:---:|:---:|:---:|:---:|:---:|:---:|
|file_xls1.xls   |149557   |47459   |259 KiB   |247 Detik   |1 MiB   |
|file_xls2.xls   |149557   |47459   |28 KiB     |15 Detik   |111 KiB   |
|file_xls3.xls   |149557   |47459   |35 KiB    |18 Detik   |128 KiB   |
|file_xls4.xls   |149557   |47459   |33 KiB    |19 Detik   |134 KiB   |

###1.2.2 Hasil Dekripsi File Xls

>>> Tampilan Layar File Enkripsi xls

![Alt text](http://yanwarrior.hol.es/kkp/4.JPG)

|Nama File Enkripsi xls|Modulo N|Eksponen D|Ukuran File (KiB)|Waktu Enkripsi  (Detik)|Ukuran Hasil Enkripsi (KiB)|
|:---:|:---:|:---:|:---:|:---:|:---:|
|enkripRSA-file_xls1.xls   |149557   |65479   |1 MiB     |241 Detik    |259 KiB  |
|enkripRSA-file_xls2.xls   |149557   |65479   |111 KiB   |174 Detik    |28 KiB   |
|enkripRSA-file_xls3.xls   |149557   |65479   |128 KiB   |243 Detik   |35 KiB   |
|enkripRSA-file_xls4.xls   |149557   |65479   |134 KiB   |199 Detik   |33 KiB   |
