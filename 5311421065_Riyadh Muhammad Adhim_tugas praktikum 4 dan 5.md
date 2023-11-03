Nama  : Riyadh Muhammad Adhim

NIM  : 5311421065

TUGAS TEKNIK PENCARIAN BLIND SEARCH

1. Tentukan bagaimana algoritma BFS di atas dapat menentukan node ke 8, 6, dan 7.
   
   algoritma BFS dapat menemukan node 8, 6, dan 7 dari node awal 1 dengan mencari semua tetangga dari setiap node secara berurutan dan menandai node yang sudah dikunjungi. Setelah itu, algoritma BFS akan menemukan node yang dicari dan proses BFS berhenti.
   
3. Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.5. Tree 1 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 5.
```
public static void main(String[] args) {
    Node n0 = new Node(0);
    Node n1 = new Node(1);
    Node n2 = new Node(2);
    Node n3 = new Node(3);
    Node n4 = new Node(4);
    Node n5 = new Node(5);
    Node n6 = new Node(6);
    Node n7 = new Node(7);
    Node n8 = new Node(8);

    Graph graph = new Graph();

    graph.addEdge(n0, n1);
    graph.addEdge(n0, n2);

    graph.addEdge(n1, n3);
    graph.addEdge(n1, n4);

    graph.addEdge(n2, n5);
    graph.addEdge(n2, n6);

    graph.addEdge(n4, n7);
    graph.addEdge(n4, n8);

    graph.bfs(n0);
}
```
Untuk menemukan node 5 menggunakan algoritma BFS, kita dapat menjalankan method bfs dengan parameter node 0 sebagai node awal. Algoritma BFS akan menjelajahi semua node pada level yang sama terlebih dahulu sebelum melanjutkan ke level selanjutnya. Dalam kasus ini, node 5 berada pada level kedua, sehingga algoritma BFS akan menemukan node 5 setelah menjelajahi node 1 dan node 2.
3. Ubahlah method static void main sehingga bentuk tree seperti Gambar 4.6. Tree 2 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node 9.
```
public static void main(String[] args) {
    Node n1 = new Node(1);
    Node n2 = new Node(2);
    Node n3 = new Node(3);
    Node n4 = new Node(4);
    Node n5 = new Node(5);
    Node n6 = new Node(6);
    Node n7 = new Node(7);
    Node n8 = new Node(8);
    Node n9 = new Node(9);

    Graph graph = new Graph();

    graph.addEdge(n1, n2);
    graph.addEdge(n1, n3);

    graph.addEdge(n2, n4);
    graph.addEdge(n2, n5);

    graph.addEdge(n3, n6);
    graph.addEdge(n3, n7);

    graph.addEdge(n5, n8);
    graph.addEdge(n5, n9);

    graph.bfs(n1);
}
```
   Untuk menemukan node 9 menggunakan algoritma BFS, kita dapat menjalankan method bfs dengan parameter node 1 sebagai node awal. Algoritma BFS akan menjelajahi semua node pada level yang sama terlebih dahulu sebelum melanjutkan ke level selanjutnya. Dalam kasus ini, node 9 berada pada level ketiga, sehingga algoritma BFS akan menemukan node 9 setelah menjelajahi semua node pada level kedua terlebih dahulu.

4. Ubahlah kode program di atas sehingga bentuk tree seperti Gambar 4.7. Tree 3 dapat dibentuk. Kemudian tentukan bagaimana algoritma BFS dapat menemukan node C.
```
public static void main(String[] args) [
    Node nA = new Node("A");
    Node nB = new Node("B");
    Node nC = new Node("C");
    Node nD = new Node("D");
    Node nE = new Node("E");
    Node nF = new Node("F");
    Node nG = new Node("G");
    Node nH = new Node("H");
    Node nI = new Node("I");
    Node nJ = new Node("J");
    Node nK = new Node("K");
    Node nL = new Node("L");
    Node nM = new Node("M");
    Node nN = new Node("N");
    Node nO = new Node("O");

    Graph graph = new Graph();

    graph.addEdge(nA, nB);
    graph.addEdge(nA, nC);

    graph.addEdge(nB, nD);
    graph.addEdge(nB, nE);

    graph.addEdge(nC, nF);
    graph.addEdge(nC, nG);

    graph.addEdge(nD, nH);
    graph.addEdge(nD, nI);

    graph.addEdge(nE, nJ);

    graph.addEdge(nF, nK);
    graph.addEdge(nF, nL);

    graph.addEdge(nG, nM);
    graph.addEdge(nG, nN);

    graph.addEdge(nK, nO);

    graph.bfs(nA);
]
```
Untuk menemukan node C menggunakan algoritma BFS, kita dapat menjalankan method bfs dengan parameter node A sebagai node awal. Algoritma BFS akan menjelajahi semua node pada level yang sama terlebih dahulu sebelum melanjutkan ke level selanjutnya. Dalam kasus ini, node C berada pada level kedua, sehingga algoritma BFS akan menemukan node C setelah menjelajahi node B dan node C.
