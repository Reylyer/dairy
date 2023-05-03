---
tags:
    - Machine
    - Metasploit
---

[[Machine]] mengenai [CVE-2014-6287]() tentang [[HFS]] 2.3.x.

## Enum
Aku akan sering menggunakan flag level 2 verbosity agar tidak cemas saat nmap tidak memberikan output apapun

```
nmap -sC -sV -T5 -Pn -vv 10.10.10.8
```


Terlihat ada service di port 80, mari kita buka browser dan menuju ip mesin tersebut. Kita disambut dengan sebuah website dengan nama tab HFS. Apa itu HFS? saya juga tidak tahu. 

> Untuk mesin ini saya akan fokus untuk mem-pwn mesin ini tanpa fokus apa itu HFS. Saya akan memperlajari HFS seiring dengan waktu nge-pwn mesin ini

Dari sedikit searching dengan keyword `HFS Vulnerability` langsung muncul suggestion untuk versi 2.3.x. Saya akan mencoba mengikuti [guide ini](https://subscription.packtpub.com/book/networking-&-servers/9781786463166/1/ch01lvl1sec20/vulnerability-analysis-of-hfs-23) yang menggunakan metasploit.

## Exploit
Menggunakan `windows/http/rejetto_hfs_exec` kita dapat mengexploit vulnerability hfs dan mendapatkan user kostas

dengan flag user kostas
`b98c9b0e61eb15d797913eb315e99c9a`

## Privilege escalation

flag root
`238886930a61c480ab65133cab80c96b`
