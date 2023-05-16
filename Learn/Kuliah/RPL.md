# Pertemuan 9

## Intro

Masih awal, refresh tentang sebelum uts, apa saja buku yang dipakai yada yada yada.

Pertemuan 9 - 13


| [[Analisis]]    | [[Design]]      | ???               |
| ----------- | ----------- | ----------------- |
| [[ERD]]     | [[PDM]]         | [[DBMS]]              |
| [[DFD]]     | [[Algoritma]]   | [[Fungsi / Prosedur]] |
|             | [[Arsitektur]]  | [[Komponen]]          |


PBO
Class -> Class
Komponen -> Package


## Objek
Entitas yang memiliki [[state]], [[behaviour]], dan [[identity]]. Berbeda dengan class, jika class adalah templatenya, objek adalah bentuk nyatanya.

### State
State akan jadi data di PBO

### Behavior
Bagaimana objek beraksi dan bereaksi 

## Metode Berorientasi Objek
- Kita memandang masalah yang akan diselesaikan sebagai objek objek
- Objek yang berhubungan dan berinteraksi akan dibuatkan sebuah use case diagram
- 
## Metode Terstruktur vs Berorientasi Objek

| Pembeda     | Structured      | PBO               |
| ----------- | --------------- | ----------------- |
| Fokus       |                 |             |
| Pemodelan   |                 | |
| Reusing     |  |      |
| Metodologi  |                 | Iteratif & inkremental|
| Dekomposisi | Algoritmik      | Object oriented|

## Elemen Model Objek
### Abstraction
### Encapsulation
### Modularity
### Hierarchy
## Analisis Berorientasi Objek
## Desain Berorientasi Objek
"How"


# Pertemuan 10
## Intro
[Kotak](https://www.dropbox.com/sh/gv51wxoqfb4iflj/AAD7xEChrUtC6awcYl-ODdBIa?dl=0&preview=10-OO+Requirement+Elicitation-upload.pdf) ini disebut dengan fase

Dalam analisis:
- Fase: Analisis
- Activity: membuat [[ERD]]
- Task: menentukan [[Entitas]]

Contoh tahap maintaining
- Bug fixing
- Penambahan fitur baru
- Adaptasi dengan lingkungan baru

## Requirement Elicitation

- Sering disebut dengan *requirement specification*
- Fokus: *apa* tujuan membuat sistem
- Yang terlibat: client, developer, dan end-user
- Hasil: *requirement specification* (berupa bahasa alamai / natural language) diwujudkan functional dan non-functional requirement

Note: non-functional merupakan requirement yang tidak ada fungsinya terhadap sistem
		\* mostly tidak bisa diuji
		\* juga termasuk quality point

Contoh non-functional
- Usability
- Reliability
- Perfoma
- Security
- Accessibility / a11y / Supportability

Requirement sebaiknya bisa diuji dan bisa di automatisasi

### Functional dan Non-functional requirement

Functional Requirement 
>mendefinisikan interaksi antara sistem dengan *lingkungannya’* lepas dari bagaimana sistem tersebut diimplementasikan

Non-Functional Requirement
>mendefinisikan aspek-aspek yang mendukung kerja sistem diluar functional  requirement

## Activity
- Identifikasi aktor
- Identifikasi skenario
- Identifikasi use case
- Refine use case
- Identifikasi hubungan antar use case
- Identifikasi kebutuhan non-fungsional

### Identifikasi aktor

- Aktor: representasi entitas luar yang berinteraksi dengan sistem (sekelompok pengguna / sistem luar yang akan ikut berinteraksi). 
- Aktor merupakan abstraksi peranan, tidak menunjuk ke orang tertentu. 
- Simbol aktord alamUML use case diagram : stick figure.

### Identifikasi skenario
### Identifikasi use case

Class --> objek
Use case --> skenario

Simbol use case adalah lingkaran/elips dengan nama use case kata kerja aktif

```
# anggap elips hehe

|-------------|
| autentikasi |
|-------------|

```

### Refine use case

- Proses 'refine' dilakukan untuk mengevaluasi use case yang telah dibuat sebelumnya
- Evaluasi bisa dilakukan dengan mengkomunikasikan use case yang dibentuk dengan customer.
- Hasil evaluasi tersebut bisa tetap, bisa berubah maupun bertambah.
- Refining --> Iteration

### Identifikasi hubungan antar use case

Untuk include, dua duanya di eksekusi

Untuk extend, tip akan diprioritaskan

Untuk generalisasi, tip yang lebih umum

### Identifikasi kebutuhan non-fungsional


# Pertemuan 12 - Design
**Fokus**: bagaimana sistem melakukan fungsinya
Mengarah ke hal teknis implementasi
Mapping model analisis -->  model desain
Mendekomposisi sistem (membagi sistem yang besar menjadi komponen komponen)
komponen/package: sekumpulan class
