

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



OOP (Object-Oriented Programming) adalah paradigma pemrograman yang menggunakan objek sebagai pusat dari program. Terdapat empat komponen OOP, yaitu:

1. Encapsulation (Pengkapsulan)
Encapsulation adalah teknik untuk menyembunyikan data dari pengguna dan mencegah akses langsung ke data tersebut dari luar. Objek dapat mengatur akses ke data atau metode mereka dengan menggunakan tingkatan akses, seperti public, private, dan protected. Contohnya, dalam sebuah kelas "Mobil", atribut "warna" bisa di-set sebagai private dan hanya dapat diakses dengan menggunakan method "setWarna" dan "getWarna".

Contoh kode dalam Python:

```
class Mobil:
    def __init__(self):
        self.__warna = ''

    def setWarna(self, warna):
        self.__warna = warna

    def getWarna(self):
        return self.__warna
```

2. Inheritance (Pewarisan)
Inheritance adalah kemampuan untuk membuat kelas baru dengan mewarisi sifat-sifat dan perilaku dari kelas yang sudah ada sebelumnya. Kelas yang baru ini disebut sebagai kelas turunan atau subclass, sedangkan kelas yang diwarisi sifat-sifatnya disebut sebagai kelas induk atau superclass. Contohnya, dalam kelas "Mobil", dapat dibuat kelas turunan seperti "Sedan" atau "SUV" yang mewarisi sifat-sifat dari kelas "Mobil".

Contoh kode dalam Python:

```
class Sedan(Mobil):
    def __init__(self):
        super().__init__()
        self.__jenis = 'Sedan'

    def getJenis(self):
        return self.__jenis
```

3. Polymorphism (Polimorfisme)
Polymorphism adalah kemampuan objek untuk memiliki banyak bentuk. Dalam OOP, ini berarti bahwa objek dari kelas yang sama dapat berperilaku berbeda tergantung pada konteks di mana mereka digunakan. Contohnya, dalam kelas "Mobil", dapat didefinisikan metode "kemudi" yang berbeda untuk mobil-mobil berbeda, seperti mobil sport dan mobil keluarga.

Contoh kode dalam Python:

```
class Mobil:
    def kemudi(self):
        print("Kendaraan ini bisa dikemudikan")

class MobilSport(Mobil):
    def kemudi(self):
        print("Kendaraan sport memerlukan kemampuan khusus untuk dikemudikan")

class MobilKeluarga(Mobil):
    def kemudi(self):
        print("Kendaraan keluarga mudah dikemudikan dan nyaman")
```

4. Abstraction (Abstraksi)
Abstraction adalah kemampuan untuk menyembunyikan detail implementasi dari pengguna dan hanya menampilkan fitur-fitur yang relevan dengan pengguna. Dalam OOP, ini berarti bahwa pengguna hanya perlu mengetahui cara menggunakan objek tanpa harus tahu bagaimana objek tersebut dibuat atau diimplementasikan. Contohnya, dalam kelas "Mobil", hanya metode "kemudi" dan "isiBensin" yang perlu ditampilkan kepada pengguna, tanpa harus mengetahui detail implementasi dari mobil.

Contoh kode dalam Python:

```
class Mobil:
    def __init__(self):
        pass

    def kemudi(self
