## 1. Karakteristik Memori dan Akses Data

Array memiliki akses O(1) karena disimpan secara kontinu di memori, sehingga alamat elemen bisa langsung dihitung menggunakan indeks. Sedangkan singly linked list bersifat non-kontinu, sehingga untuk mengakses elemen tertentu harus menelusuri node dari awal hingga posisi yang diinginkan, yang membuat kompleksitasnya O(n).

## 2. Analisis Efisiensi Operasi Manipulasi

Linked list lebih unggul saat melakukan insertion dan deletion, terutama di awal atau tengah data. Hal ini karena hanya perlu mengubah pointer tanpa menggeser elemen lain. Sebaliknya, array memerlukan proses shifting yang memakan waktu O(n), sehingga kurang efisien untuk operasi tersebut.

## 3. Konsep Doubly Linked List

Node pada doubly linked list memiliki data, pointer next, dan pointer prev. Pointer tambahan memungkinkan traversal dua arah (maju dan mundur), sehingga lebih fleksibel. Namun, penggunaan memori menjadi lebih besar dan pengelolaan pointer lebih kompleks dibanding singly linked list.


## 4. Mekanisme Circular Linked List

Circular linked list adalah linked list di mana node terakhir menunjuk kembali ke node pertama, sehingga membentuk lingkaran. Perbedaannya dengan linked list biasa adalah tidak ada NULL di akhir. Contoh penggunaannya adalah pada round-robin scheduling dapat diulang terus tanpa kembali ke awal.


## 5. Array Dinamis di Python

Python list menggunakan dynamic array. Saat kapasitas penuh dan dilakukan append, sistem akan mengalokasikan memori baru yang lebih besar, menyalin data lama, lalu menambahkan elemen baru. Walaupun resizing membutuhkan O(n), secara rata-rata append tetap O(1) (amortized).


