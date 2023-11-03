Nama = Riyadh Muhammad Adhim
NIM  = 5311421065

TUGAS 5 TEKNIK HEURISTIC SEARCH

1. Pelajari class EightPuzzleSearch, EightPuzzleSpace, dan Node.

   
2. Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.8. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 5.1.
```
int ex[] = {3, 1, 2, 4, 7, 5, 6, 8, 0}; // initial state
int goal[] = {1, 2, 3, 4, 0, 8, 5, 6, 7}; // goal state
```
Untuk menentukan langkah-langkah yang diperlukan agar puzzle mencapai goal state, dapat dilakukan dengan menggunakan algoritma heuristic search. Berikut adalah langkah-langkah yang dapat dilakukan:

1. Inisialisasi initial state dan goal state.
2. Buat sebuah node yang merepresentasikan initial state.
3. Hitung nilai fungsi heuristik dari node tersebut.
4. Tambahkan node tersebut ke dalam open list.
5. Selama open list tidak kosong, lakukan langkah-langkah berikut:
   a. Ambil node dengan nilai fungsi heuristik terkecil dari open list.
   b. Jika node tersebut merupakan goal state, maka proses pencarian selesai dan kembalikan path dari initial state ke goal state.
   c. Jika node tersebut bukan goal state, ekspansi node tersebut dan tambahkan semua successor node ke dalam open list.
6. Jika open list kosong dan goal state belum ditemukan, maka pencarian tidak berhasil.

Perbedaan dengan solusi pada program awal adalah pada langkah-langkah pencarian. Pada program awal, digunakan algoritma breadth-first search (BFS) yang tidak memperhitungkan nilai heuristik. Sedangkan pada algoritma heuristic search, nilai heuristik digunakan untuk memperkirakan jarak dari suatu node ke goal state, sehingga dapat mempercepat proses pencarian.

3. Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.9. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1 dan 2.
4. Ubahlah initial dan goal state dari program di atas sehingga bentuk initial dan goal statenya Gambar 5.10. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state. Analisa dan bedakan dengan solusi pada point 1, 2, dan 3.
5. Ubahlah initial dan goal state dari program dan class-class di atas sehingga bentuk initial dan goal statenya Gambar 5.11. Kemudian tentukan langkah-langkah mana saja sehingga puzzlenya mencapai goal state
