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

Menghapus item pada pada posisi yang diberikan dari daftar dan dikembalikan. Jika tidak ada indeks yang ditentukan, `a.pop()` akan menghapus dan mengembalikan item terakhir dari daftar.

list.**clear**()

Menghapus semua item dari dafta. Setara dengan `del a[:]`.

list.**index**(*x[, start[, end]]*)

Mengembalikan indeks berbasis nol dalam daftar item pertama yang nilainya sama dengan *x*. Muncul [ValueError](https://docs.python.org/3/library/exceptions.html#ValueError) jika tidak ditemukan item.

list.**count**(*x*)

Mengembalikan jumlah *x* yang muncul pada daftar.

list.**sort**(*, key=None, reverse=False)

Mengurutkan item dari daftar di tempat ( argumen dapat digunakan untuk penyesuaian pengurutan, penjelasan lebih dalam lihat [sorted()](https://docs.python.org/3/library/functions.html#sorted) ).

list.**reverse**()

Membalikan elemen dari daftar tempat.

list.**copy**()

Mengembalikan salinan daftar. Setara dengan `a[:]`.

Contoh penggunaan sebagian besar metode list :
```python
>>> fruits = ['orange', 'apple', 'pear', 'banana', 'kiwi', 'apple', 'banana']
>>> fruits.count('apple')
2
>>> fruits.count('tangerine')
0
>>> fruits.index('banana')
3
>>> fruits.index('banana', 4)  # Find next banana starting a position 4
6
>>> fruits.reverse()
>>> fruits
['banana', 'apple', 'kiwi', 'banana', 'pear', 'apple', 'orange']
>>> fruits.append('grape')
>>> fruits
['banana', 'apple', 'kiwi', 'banana', 'pear', 'apple', 'orange', 'grape']
>>> fruits.sort()
>>> fruits
['apple', 'apple', 'banana', 'banana', 'grape', 'kiwi', 'orange', 'pear']
>>> fruits.pop()
'pear'
```
