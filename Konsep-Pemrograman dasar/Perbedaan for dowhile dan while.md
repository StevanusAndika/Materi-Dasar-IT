

For loop, do-while loop, dan while loop adalah jenis struktur kontrol aliran program dalam pemrograman yang digunakan untuk melakukan iterasi atau perulangan.

Perbedaan antara ketiganya terletak pada cara mereka mengatur iterasi dan kondisi penghentian.

1. For loop

For loop digunakan untuk melakukan perulangan dengan jumlah iterasi yang sudah diketahui sebelumnya. Bentuk umum dari for loop adalah:

```
for (inisialisasi; kondisi; perubahan) {
   // pernyataan yang akan diulang
}
```

- inisialisasi: digunakan untuk menginisialisasi nilai variabel kontrol iterasi
- kondisi: merupakan ekspresi boolean yang dievaluasi pada setiap iterasi, jika bernilai true, maka pernyataan dalam loop dijalankan, jika false, maka loop berhenti.
- perubahan: pernyataan yang dieksekusi setelah blok pernyataan dalam loop dijalankan pada setiap iterasi.

Contoh penggunaan for loop:

```
for (int i = 1; i <= 10; i++) {
   System.out.println(i);
}
```

Pada contoh di atas, variabel `i` diinisialisasi dengan nilai 1, kemudian kondisi `i <= 10` dievaluasi, jika true, pernyataan `System.out.println(i)` akan dijalankan dan nilai `i` akan bertambah 1 setiap iterasi hingga kondisi menjadi false.

2. Do-while loop

Do-while loop juga digunakan untuk melakukan perulangan dengan jumlah iterasi yang tidak diketahui sebelumnya. Bentuk umum dari do-while loop adalah:

```
do {
   // pernyataan yang akan diulang
} while (kondisi);
```

- pernyataan: merupakan pernyataan yang dieksekusi dalam loop
- kondisi: merupakan ekspresi boolean yang dievaluasi setelah pernyataan dijalankan pada setiap iterasi, jika true, maka loop akan berlanjut, jika false, loop akan berhenti.

Perbedaan antara do-while loop dengan while loop terletak pada kondisi, pada do-while loop, pernyataan dalam loop akan dieksekusi minimal satu kali sebelum kondisi dievaluasi.

Contoh penggunaan do-while loop:

```
int i = 1;
do {
   System.out.println(i);
   i++;
} while (i <= 10);
```

Pada contoh di atas, pernyataan `System.out.println(i)` akan dijalankan minimal satu kali sebelum kondisi `i <= 10` dievaluasi.

3. While loop

While loop digunakan untuk melakukan perulangan dengan jumlah iterasi yang tidak diketahui sebelumnya. Bentuk umum dari while loop adalah:

```
while (kondisi) {
   // pernyataan yang akan diulang
}
```

- kondisi: merupakan ekspresi boolean yang dievaluasi pada setiap iterasi, jika true, maka pernyataan dalam loop dijalankan, jika false, loop berhenti.

Perbedaan antara while loop dengan do-while loop terletak pada kondisi, pada while loop, kondisi dievaluasi sebelum pernyataan dalam loop dieksekusi.

Contoh penggunaan while loop:

```
int i = 1;
while (i <= 10) {
  
