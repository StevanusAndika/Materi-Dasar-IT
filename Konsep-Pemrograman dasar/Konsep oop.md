

OOP (Object Oriented Programming) adalah paradigma pemrograman yang didasarkan pada konsep objek. Objek adalah sebuah instansi dari sebuah class, yang memiliki properti dan metode. Berikut adalah beberapa komponen OOP beserta contohnya:

1. Class - adalah blueprint atau template yang digunakan untuk membuat objek. Contohnya, jika kita ingin membuat objek 'Mobil', kita perlu membuat class 'Mobil' terlebih dahulu. Contoh kode:

```
class Mobil:
  def __init__(self, merk, tahun):
    self.merk = merk
    self.tahun = tahun

  def info(self):
    print(f"Mobil {self.merk} tahun {self.tahun}")
```

2. Objek - adalah instansi dari sebuah class. Setiap objek memiliki properti dan metode yang terpisah dari objek lainnya. Contoh kode:

```
mobil1 = Mobil("Toyota", 2020)
mobil2 = Mobil("Honda", 2021)
print(mobil1.merk) # Toyota
print(mobil2.merk) # Honda
mobil1.info() # Mobil Toyota tahun 2020
mobil2.info() # Mobil Honda tahun 2021
```

3. Properti - adalah nilai yang dimiliki oleh sebuah objek. Properti bisa berupa variabel atau atribut. Contoh kode:

```
class Mobil:
  def __init__(self, merk, tahun):
    self.merk = merk
    self.tahun = tahun

  def info(self):
    print(f"Mobil {self.merk} tahun {self.tahun}")

mobil1 = Mobil("Toyota", 2020)
print(mobil1.merk) # Toyota
```

4. Metode - adalah fungsi yang dimiliki oleh sebuah objek. Metode biasanya digunakan untuk memanipulasi properti objek. Contoh kode:

```
class Mobil:
  def __init__(self, merk, tahun):
    self.merk = merk
    self.tahun = tahun

  def info(self):
    print(f"Mobil {self.merk} tahun {self.tahun}")

  def tambah_tahun(self, tahun):
    self.tahun += tahun

mobil1 = Mobil("Toyota", 2020)
mobil1.info() # Mobil Toyota tahun 2020
mobil1.tambah_tahun(1)
mobil1.info() # Mobil Toyota tahun 2021
```

5. Inheritance - adalah konsep dimana sebuah class dapat mewarisi properti dan metode dari class lainnya. Contoh kode:

```
class Kendaraan:
  def __init__(self, merk, tahun):
    self.merk = merk
    self.tahun = tahun

  def info(self):
    print(f"{self.merk} tahun {self.tahun}")

class Mobil(Kendaraan):
  def __init__(self, merk, tahun, warna):
    super().__init__(merk, tahun)
    self.warna = warna

  def info(self):
    print(f"Mobil {self.merk} tahun {self.tahun} berwarna {self.warna}")

mobil1 = Mobil("Toyota", 2020, "merah")
mobil1.info() # Mobil Toyota tahun 2020 berwarna merah
```

6. Polymorphism - adalah konsep dimana sebuah objek dapat memiliki bentuk yang berbeda-beda ketika dipanggil oleh metode yang sama. Contoh kode:

```


class H
