`bin`, kependekan dari binary. Directory ini berisi program yang dapat diakses oleh semua user.

Terdapat varian lain dari `bin` yakni `sbin`. `sbin` berisi program yang biasanya digunakan sysadmin saat menggunakan user root. Secara default user biasa hanya memiliki `bin` di dalam variable `PATH` nya.

```
asprak@please-dont-hack-me /bin > ls -lah | head -n 15 
total 397M
drwxr-xr-x  2 root  root     36K May  6 07:12 .
drwxr-xr-x 14 root  root    4.0K Dec  5 04:23 ..
lrwxrwxrwx  1 root  root      28 Jan  6  2021 FileCheck-11 -> ../lib/llvm-11/bin/FileCheck
lrwxrwxrwx  1 root  root       1 Feb 15  2021 X11 -> .
-rwxr-xr-x  1 root  root     59K Sep 24  2020 [
-rwxr-xr-x  1 root  root     31K Apr  3  2021 aa-enabled
-rwxr-xr-x  1 root  root     31K Apr  3  2021 aa-exec
-rwxr-xr-x  1 root  root     59K Apr  2 03:06 ab
-rwxr-xr-x  1 root  root    3.4K Feb 27  2021 activate-global-python-argcomplete3
-rwxr-xr-x  1 root  root     35K Jan 27  2021 addftinfo
-rwxr-xr-x  1 root  root     27K Jan 20  2022 addpart
lrwxrwxrwx  1 root  root      26 Feb 20  2021 addr2line -> x86_64-linux-gnu-addr2line
-rwxr-xr-x  1 root  root    162K Jan 27  2021 afmtodit
-rwxr-xr-x  1 root  root    5.8K Apr 19  2021 ansible
```


