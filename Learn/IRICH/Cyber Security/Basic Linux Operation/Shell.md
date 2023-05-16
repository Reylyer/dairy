Ini merupakan bagian paling penting dari penggunaan [[Linux]]. Berbeda dari [[Windows]] yang navigasinya lebih mengutakaman GUI, Linux lebih mengutamakan menggunakan shell. Bukan berarti semua aktivitas dilakukan di dalam shell, tapi banyak aktivitas di linux yang wajib if not lebih baik dilakukan lewat shell.

Sebelum mengenal apa itu shell, kita sebaiknya membedakan beberapa kosakata yang sering disamakan. Diluar dari ini, kita boleh saja menukar nukar kosakata tersebut, asal lawan bicaramu juga paham apa yang kamu maksud.
| Kosakata | Arti |
|----------|------|
| Terminal | Device yang digunakan untuk berinteraksi dengan komputer, e.g. mouse dan keyboard|
| Terminal Emulator | Software yang mengemulasikan fungsi dari terminal |
| Shell    | Software yang menyediakan antarmuka antara sistem operasi dengan usernya|

## Terminal Emulator dan Shell

Terminal emulator merupakan `GUI` dari sebuah shell. Shell tidak dapat berdiri sendiri, shell hanyalah software yang menghubungkan sistem operasi dengan user tetapi tidak secara langsung. Shell membutuhkan antarmuka `GUI` untuk menampilkan teks input outputnya. Shell dapat mencapai tujuan tersebut dengan menggunakan perantara sebuah terminal emulator.

Jika kalian di windows membuka cmd atau powershell dari search maka popup window akan muncul. Itu adalah sebuah terminal emulator. Contoh lain adalah Xterm, st, kitty, gnome-shell, dan lain lain.


## Alur Data dari User ke Sistem Operasi

Jika kita ringkas, kita sebagai manusia berinteraksi dengan terminal (mouse dan keyboard).  Inputan tersebut akan diterima oleh terminal emulator dan akan diberikan kepada shell. Shell akan menginterpret masukan tersebut menjadi command yang akan diberikan kepada sistem operasi

## Hubungan antara Terminal Emulator dan Shell

Untuk Linux sendiri tiap user akan memiliki shell default. Pada umumnya shell default ini [[BASH]] atau [[sh]]. Kita bisa mengganti shell default menggunakan command `chsh` (stands for change shell). Sementara untuk terminal emulator user dapat memilih dan membuka layaknya sebuah aplikasi. 

Jika kita ingin mengganti tampilan windownya, kita perlu mengonfigurasi terminal emulatornya. Jika kita ingin mengganti teks apa yang di tampilkan di terminal, menambah fitur tab completion atau suggestion, maka kita perlu mengonfigurasi shellnya.