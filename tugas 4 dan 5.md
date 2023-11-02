Nama  : Riyadh Muhammad Adhim

NIM  : 5311421065

TUGAS TEKNIK PENCARIAN BLIND SEARCH

1. Tentukan bagaimana algoritma BFS di atas dapat menentukan node ke 8, 6, dan 7.
   
   Untuk menentukan node 8, 6, dan 7 menggunakan algoritma BFS pada kode yang diberikan, perlu memulai pencarian dari node 3, yang merupakan root node. Algoritma BFS dimulai dengan menuju ke root node dan kemudian menuju ke semua bagian nya. Dalam hal ini, samping dari node 3 adalah node 2 dan 4. Oleh karena itu, algoritma akan menuju ke node 2 dan 4 selanjutnya.

   Setelah menuju ke node 2, algoritma akan menuju ke node 1 dan 3. Namun, node 3 sudah dikunjungi, sehingga akan dilewati. Selanjutnya, algoritma akan menuju ke node 4 dan tetangganya, yaitu node 3, 5, 6, dan 7. Node 3 sudah dikunjungi, sehingga akan dilewati. Algoritma kemudian akan mengunjungi node 5, 6, dan 7 secara berurutan.

   Oleh karena itu, algoritma BFS akan menuju ke node dalam urutan berikut: 3, 2, 4, 1, 5, 6, 7, 8. Node 8 akan dikunjungi terakhir karena jaraknya paling jauh dari root node dan memiliki jarak terjauh dari itu. Secara ringkas, algoritma BFS pada kode yang diberikan akan menentukan node 8, 6, dan 7 dengan menuju ke mereka dalam urutan 3, 2, 4, 1, 5, 6, 7, 8.

2. Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.4 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 5.

   
