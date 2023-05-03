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