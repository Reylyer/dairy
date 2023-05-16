# Pertemuan 9 (Transaction)
## Intermezzo
Trigger, assertion
Indexing

akan belajar tentang bagaimana dbms bekerja
mirip dengan sistem operasi

Akan menggunakan lagi B+ tree

## Transaction
jika di sistem operasi transaction adalah proses
transaksi di database selalu unik
\* not so make sense tbh

### Jenis Transaction
- Read
>
- Write
>

### Properti Transaction (ACID)
- Atomic
  >Transaksi hanya bisa sampai selesai atau tidak sama sekali (COMMIT adn ROLLBACK)
- Consistency
  >contoh kasus: jika saldo org1 1jt dan saldo org2 2jt, org1 mengirim 100k ke org2 maka 
  >-- wip
- Isolation
  >Tiap transaksi tidak dipengaruhi transaksi lain
- Durability
  >Database tetap menyimpan keadaan terakhir COMMIT
  
### Schedule (Penjadwal)

Penjadwalan bagaimana proses atau transaksi dapat dilakukan secara *interleaved* atau *parallel*.

### Transaction term
- Throughput: Banyak proses/transaksi yang diselesaikan dalam satuan waktu
- Response time: Rata rata satuan waktu yang diselesaikan sebuah proses/transaksi

### Serilizable
Penjadwal yang dilakukan secara paralel harus bisa dilakukan secara serial

### Anomalies in Interleaved Execution
### WR Conflict (Reading Uncommitted Data)
- Melakukan dirty read (membaca data yang sudah dimodifikasi namun belum selesai(COMMIT))

### RW Conflict (Unrepeatable Reads)
- Situasi dimana suatu transaksi membaca data namun diubah oleh transaksi lain ditengah transaksi

### WW Conflict (Overwriting Uncommitted Data)
- Blind write
- Situasi dimana transaksi T2 merubah data yang sudah dimodifikasi oleh T1. Namun T1 masih berlangsung

# Pertemuan 10
## Recoverable Schedule
## Unrecoverable Schedule
## Lock Based Control
Usaha DBMS agar menghindari Unrecoverable Schedul/anomali

### Strict Two-Phase Locking (Strict 2-PL)
Saat ada transaksi T yang ingin melakukan operasi read, T akan diberikan shared key S(A).
^^^ masuk akal karena tidak akan ada perubahan data selama proses. Sehingga key bisa diberikan ke transaksi lain

Saat ada transaksi T yang memiliki operasi write, T akan diberikan key exclusive X(A).

## Sneek peek
Deadlock 