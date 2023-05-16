`grep` merupakan [[Useful programs]] untuk melakukan filter dari sebuah inputan. `grep`  melakukan filter menggunakan [[regular expression]]. `grep` biasa digunakan bersamaan dengan program lain dalam sebuah [[pipeline]].

Berbeda dengan regex di find, regex menggunakan `grep` terasa lebih *benar* karena terdapat fitur extended regex.

Contoh penggunaan `grep`

```
find . | grep -E "regexp"
```

note: `-E` merupakan flag untuk menggunakan extended regex

