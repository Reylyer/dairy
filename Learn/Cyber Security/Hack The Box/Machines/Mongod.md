Mesin Tier 0 Starting point

Mesin yang simple yang mengenalkan service [[mongodb]] yang dapat diakses secara umum. 

## Enum

[[nmap]] jagoan saya mumpung ini starting point dan T5 diperbolehkan

```
nmap -p - -T5 -sC -sV 10.129.172.43
```

Result:
```
...
Not shown: 65533 closed tcp ports (reset)

PORT      STATE SERVICE VERSION

22/tcp    open  ssh     OpenSSH 8.2p1 Ubuntu 4ubuntu0.5 (Ubuntu Linux; protocol 2.0)

| ssh-hostkey: 

|   3072 48add5b83a9fbcbef7e8201ef6bfdeae (RSA)

|   256 b7896c0b20ed49b2c1867c2992741c1f (ECDSA)

|_  256 18cd9d08a621a8b8b6f79f8d405154fb (ED25519)

27017/tcp open  mongodb MongoDB 3.6.8 3.6.8

| mongodb-databases: 

|   ok = 1.0
...
```

Dari informasi diatas kita bisa menjawab beberapa task

**How many TCP ports are open on the machine?**
>`2`

**Which service is running on port 27017 of the remote host?**
>`MongoDB 3.6.8`

**What type of database is MongoDB? (Choose: SQL or NoSQL)**
Dari sepengetahuanku [[mongodb]] bukan database SQL karena menggunakan js object
>`NoSQL`

**What is the command name for the Mongo shell that is installed with the mongodb-clients package?**
Sebenarnya aku menebak dari clue tapi dengan googling sedikit memang `mongo`
>`mongo`

**What is the command used for listing all the databases present on the MongoDB server? (No need to include a trailing ;)**
Setelah melakukan googling tentang shell mongo tentang basic usage kita menemukan command `show` dengan argumen `dbs`
>`show dbs`

**What is the command used for listing out the collections in a database? (No need to include a trailing ;)**
Jika `show dbs` menunjukan database maka untuk collections kita `show collections` (menebak dari clue)
>`show collections`

**What is the command used for dumping the content of all the documents within the collection named flag in a format that is easy to read?**
Baru ditahap ini aku mencoba coba. Karena aku lagi di windows, aku install [[mongodb]] versi gui saja (compass). Hasil dari googling menemukan `db.COLLECTION_NAME.find()` untuk mengoutput semua isi collection. Di gui sudah ada semua databasenya beserta collectionnya. Kita menemukan flag berada di dalam database `sensitive_information`. Kita tinggal mengganti `COLLECTION_NAME` dengan `flag`. [Jawaban](https://stackoverflow.com/a/29778560) ini ada yang berkomentar untuk menambahkan `.pretty()` diakhir maka jawaban adalah
>`db.flag.find().pretty()`

**Submit root flag**
```json
{
  _id: ObjectId("630e3dbcb82540ebbd1748c5"),
  flag: '1b6e6fb359e7c40241b6d431427ba6ea'
}
```
