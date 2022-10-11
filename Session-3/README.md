# DOCUMENT TYPE DEFINITIONS (DTD)
- DTD berfungsi untuk mendefinisikan tipe dokumen XML. 
- DTD ditulis untuk menjelaskan elemen dan entitas yang memungkinkan muncul di dalam dokumen dan elemen isi serta atributnya.
---

## A. Validation
DTD digunakan unttuk menddeklarasikan semua elemen, atribut, dan entitas yang akan digunakan di dalam dokumen. Semua elemen, atribut, dan entitas yang akan digunakan harus di dalam DTD. Contoh pada **example-3.1.xml**

## B. Deklarasi Elemen
- **#PCDATA**   -> tipe data (teks) ->
<code><ELEMENT telp(#PCDATA)></code>
- **Element Child** -> ditulis di dalam tanda kurung.
<code>ELEMENT fax (phone_number)></code>
- **Sequence** -> Sequence ini dimaksudkan dapat menuliskan elemen anak lebih dari satu deklarasi.
<code><`!`ELEMENT nama(nama_depan, nama_belakang)></code>

## C. Jumlah Child
dapat dituliskan dengan menambahkan tanda berikut pada akhir nama element.
  
<table>
<tr>
<th>Character</th>
<th>Penjelasan</th>
</tr>
<tr>
<td>+</td>
<td>Muncul satu kali atau lebih</td>
</tr>
<tr>
<td>*</td>
<td>Muncul 0 kali atau lebih</td>
</tr>
<tr>
<td>?</td>
<td>Boleh tidak muncul,tapi jika muncul maksimal 1 kali</td>
</tr>
<tr>
<td>|</td>
<td>Fungsi ATAU</td>
</tr>
</table>
***

<nocode> < ! ELEMENT karyawan(telp+)></nocode> **Elemen karyawan memiliki 1 atau lebih elemen telp**


## D. Elemen Kosong
- Elemen Kosong adalah sebuah tag yang tidak memiliki elemen nilai.

## E. Any
Any ini mengizinkan apapun dapat beradda pada suatu element.
