## Pertemuan 9

### Intermezzo
refreshing [[Dasar Pemograman]] --> [[Algoritma dan Pemograman]] --> [[Struktur Data]] --> [[Pemograman Berorientasi Objek]]

Yang dipelajari
[[Dasar Pemograman]]: tipedata, fungsi, dan rekursi

[[Algoritma dan Pemograman]]: variable dan iterasi

[[Struktur Data]]: [[Enkapsulasi]], dan [[Polimorphism]]
Dalam [[Struktur Data]] operasi dilakukan diluar objek
operasi(O)

[[Pemograman Berorientasi Objek]]: [[Inheritance]]
Dalam [[Pemograman Berorientasi Objek]] operasi dilakukan didalam objek
O.operasi()

### Polimorphism
Sifat suatu objek yang dapat memiliki peran lebih dari satu.
Contoh:
Sebuah class segitiga dan persegi, sama sama memiliki operasi luas tetapi cara menghitungnya berbeda.

#### Klasifikasi/Konsep Polimorphism

- **Ad hoc**
	Ad hoc berarti sementara
	* Overloading
		Sebuah method yang sama namun memiliki perilaku yang berbeda yang dikarenakan parameter yang berbeda
	* Coercion
		Pemaksaan satu tipe data parameter yang dicast ke tipedata lain yang memungkinan digunakan didalam parameter lain.
* **Universal**
	- Inclusion
		Sifat dimana suatu objek yang meng-"include" beberapa. Satu objek yang dapat diisikan oleh keturunannya
	- Parametric
		...

- Binding type
	- Early (Compile-time)
	- Late (Runtime)




| | |Anabul | ||
|-|-|-|-|-|
|Kucing |Anjing | Kelinci | Marmut||
| Meow   | Guk|  ???| Cit ||

#### Basic Syntax Algoritmik

```
KAMUS
A: Anabul

ALGORITMA
A <- new Kucing()
A.bunyi() {"Meow"}

A <- new Anjing()
A.bunyi() {"Guk"}
```

## Pertemuan 10

### Lanjutan klasifikasi Polimorphism (Parametrik)

Sebuah generic class yang diberikan parameter
The weird way

```
generic class Hewan<T>
	- data: T
	procedure bunyi()
		output data.bunyi()

	constructor Hewan<T>(x: T)
		data <- new T()

```

```
KAMUS
	H: Hewan
	
ALGORITMA
	H <- new Hewan<Kucing>
	H.bunyi()
```

Kinda the java way, idk a lil bit confused

```
generic class Hewan<T>
	- data: T
	procedure bunyi()
		output data.bunyi()

	function getData() -> T
		-> data

	procedure setData(data: T)
		this.data <- data
```

```
KAMUS
	H: Hewan
	K: Kucing
	
ALGORITMA
	H <- new Hewan<Kucing>
	H.getData().bunyi()
```

# JAVA SUCKS

# Pertemuan 11
## Intro

--- Bahas GEMASTIK 2023
--- recap polimorphism

## Koleksi

komponen: bagian/kepemilikan sebuah objek
elemen: bagian dari sebuah himpunan/koleksi

Karakteristik koleksi
- Dapat dalam mengelola objek apapun, dengan urutan sesuai yang dimasukkan
- Dapat menmpung objek tapi unik
- Diproses secara FIFO atau LIFO


Beberapa operasi Koleksi
- add()
- contains()
- remove()

```

					                 Collection<E>

							/              |                \

					List<E>              Queue<E>            Set<E>
			/         |       \  /           |                 |      \
ArrayList<E>     Vector<E>  LinkedList<E>  PriorityQueue<E>  sorted   unsorted
															   |         |
													LinkedHashSet<E> HashSet<E> 
```


# Pertemuan 12 - Persistensi
## Kosakata
### Persistent
>Penyimpanan yang "abadi", disimpan di dalam penyimpanan sekunder. Contohnya adalah penyimpanan data teks di sebuah file. Contoh lainnya adalah penyimpanan data di dalam database.
### Transient
>
### Volatile
>
### Temporer
>

Berhubungan dengan [[RPL]]