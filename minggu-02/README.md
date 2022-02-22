# 5. Struktur Data
## 5.1. Membuat List
Tipe data list memiliki beberapa metode, antara lain :

list.**append**(*x*)

Menambahkan item ke akhir list. Setara dengan `a[len(a):] = [x]`
	
list.**extend**(*iterable*)

Memperluas list dengan menambahkan semua item dari iterable. Setara dengan `a[len(a):] = iterable`

list.**insert**(*i, x*)
Memasukan item pada posisi tertentu. Argumen pertama adalah indeks elemen yang akan disisipkan sebelumnya, setara dengan `a.insert(0,x)a.insert(len(a), x)a.append(x)`

list.**remove**(*x*)

Menghapus item pertama dari daftar yang nilainya sama dengan *x*. Hal ini menimbulkan [ValueError](https://docs.python.org/3/library/exceptions.html#ValueError) jika item tidak ditemukan.

list.**pop**([*i*])
	

list.**clear**()
	

list.**index**(*x[, start[, end]]*)
	

list.**count**(*x*)
	

list.**sort**(*, key=None, reverse=False)
	

list.**reverse**()
	

list.**copy**()
	
