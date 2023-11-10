Nama  = Riyadh Muhammad Adhim

NIM   = 5311421065

# PERMAINAN TIC TAC TOE
Penyelesaian masalah permainan tic tac toe dapat menggunakan algoritma heuristic untuk mencapai solusi yang optimal. Pada modul ini memperlihatkan bagaimana membuat sebuah permainan tic tac toe. Initial state dari permainan ini adalah puzzle ukuran 8 yang tidak berisikan apaapa. Ketika pemain pertama menekan salah satu ubin, maka ubin tersebut akan diberikan tanda silang. Pemain kedua harus menghalangi pemain pertama untuk membuat tanda silang berjajaran baik secara vertikal, horizontal, atau diagonal. Permainan ini akan berakhir (goal state) ketika salah seorang pemain sudah menderetkan tanda meraka masing-masing baik secara vertikal, horizontal, atau diagonal. 

Solusi dari permasalahan ini dapat dilakukan dengan membuat topologi Tree, kemudian setiap langkah dari pemain pertama atau kedua akan menjadikan initial state selanjutnya, kemudian langkah tersebut akan dijadikan sebagai initial state yang baru sampai menemukan goal statenya. Ilustrasi penyelesaian masalah permainan tic tac toe ini dapat dilihat melalui Gambar dibawah ini
![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/722a16e4-5648-4b52-b7b2-44e675cd76f9)
# Tugas
Melunis ulang dan mempelajari beberapa code pada file tugas kemudian mengubah beberapa bagian utuk melihat perubahannya.
# Menggunakan Graphical User Interface (GUI)
- GameState
  
   ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/779fa39a-db36-42c3-a811-df7a3a05a6b5)
  
  `penjelasan`
  
  Enum GameState adalah tipe data khusus dalam pemrograman Java yang berisi kumpulan konstanta tetap. GameState ini memiliki empat nilai konstanta. Pertama, PLAYING digunakan untuk menunjukkan bahwa permainan sedang berlangsung. Kedua, DRAW digunakan ketika permainan berakhir dengan seri, artinya tidak ada pemain yang menang. Ketiga dan keempat, CROSS_WON dan NOUGHT_WON digunakan untuk menunjukkan bahwa pemain dengan simbol silang (X) atau lingkaran (O) telah memenangkan permainan.
- Seed

  ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/4ed5d63f-f32b-41d6-ab13-20dc07ed5216)

  `penjelasan`
  
  Enum Seed adalah tipe data khusus dalam pemrograman Java yang berisi kumpulan konstanta tetap. Seed ini memiliki tiga nilai konstanta. Pertama, EMPTY digunakan untuk menunjukkan bahwa sel permainan saat ini kosong. Kedua dan ketiga, CROSS dan NOUGHT digunakan untuk menunjukkan bahwa sel permainan saat ini berisi simbol silang (X) atau lingkaran (O).
- State

  ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/347b2587-7bfb-49c9-8ed2-038aa3ddbafe)
  
  `penjelasan`
  
  Enum State adalah tipe data khusus dalam pemrograman Java yang berisi kumpulan konstanta tetap. State ini memiliki empat nilai konstanta. Pertama, PLAYING digunakan untuk menunjukkan bahwa permainan sedang berlangsung. Kedua, DRAW digunakan ketika permainan berakhir dengan seri, artinya tidak ada pemain yang menang. Ketiga dan keempat, CROSS_WON dan NOUGHT_WON digunakan untuk menunjukkan bahwa pemain dengan simbol silang (X) atau lingkaran (O) telah memenangkan permainan.
- Cell

  ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/15ac9001-7553-4507-9049-7eb7a035c85d)

  `penjelasan`
  
  Kelas `Cell` dalam kode Java ini adalah bagian dari implementasi permainan Tic Tac Toe. Kelas ini mendefinisikan sel dalam permainan, yang dapat berisi simbol silang (X), lingkaran (O), atau kosong. Setiap sel memiliki indeks baris dan kolom. Kelas ini juga menyediakan metode untuk mengosongkan isi sel dan menggambar isi sel pada kanvas grafik. Jika isi sel adalah X, maka akan digambar garis silang merah. Jika isi sel adalah O, maka akan digambar lingkaran biru.
- Board
  
  ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/e77160e5-a55f-4538-bb57-2176a4a5eb06)
  ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/fc461852-5fda-45ae-8478-72299c8539b4)

`penjelasan`

  Kelas Board dalam kode Java ini adalah bagian dari implementasi permainan Tic Tac Toe. Kelas ini mendefinisikan papan permainan, yang terdiri dari array 2D dari sel. Setiap sel adalah instance dari kelas Cell yang telah didefinisikan sebelumnya. Kelas ini menyediakan metode untuk menginisialisasi papan permainan, memeriksa apakah permainan berakhir seri (yaitu, tidak ada sel kosong), memeriksa apakah pemain dengan simbol tertentu telah menang, dan menggambar papan permainan pada kanvas grafik.
- GameMain

  ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/bdd8a802-665f-4d6d-aa33-64ea973cfc75)
  ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/b98f5220-2de4-425c-a89c-21a3489bdb67)
  ![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/fe711c1c-e835-440e-8a53-1ba7c88b0653)

  `penjelasan`

  Pada kelas GameMain, konstruktor menginisialisasi elemen-elemen GUI, seperti dimensi papan permainan, status bar, dan mendefinisikan perilaku mouse-click untuk memainkan permainan. Metode initGame digunakan untuk menginisialisasi kondisi awal permainan, sementara metode updateGame mengubah status permainan berdasarkan langkah pemain terakhir. Metode paintComponent digunakan untuk menggambar elemen-elemen GUI dan memperbarui status bar sesuai dengan kondisi permainan. Di dalam metode main, program dijalankan dalam event-dispatching thread untuk keamanan thread. Sebuah objek JFrame dibuat, diisi dengan panel GameMain, dan ditampilkan kepada pengguna sebagai antarmuka grafis permainan Tic-Tac-Toe.

# Hasil
![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/b27faff7-e0b9-427a-a86b-0c0822a69c94)

![image](https://github.com/Riyadh30/Riyadh30/assets/149092819/c90a35a2-6d3a-428d-a857-04bfa585383f)

