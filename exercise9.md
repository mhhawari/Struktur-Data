# Exercise 9 Struktur Data
## Introduction Section
1. Jelaskan definisi object dalam Paradigma Object-Oriented!\
Objek merupakan peran utama dalam object-oriented

2. Jelaskan tiga tujuan dalam Paradigma Object-Oriented!
* Robutness\
Mampu menangani input yang tidak terduga
* Adaptability\
Menjalankan dengan perubahan minimal pada perangkat keras dan platform sistem operasi yang berbeda 
* Reusability\
Kode yang sama harus dapat digunakan sebagai komponen

3. Jelaskan tiga prinsip dalam Paradigma Object-Oriented!
* Modularity\
Kumpulan fungsi dan kelas yang terkait erat yang didefinisikan
bersama-sama dalam satu file kode sumber
* Abstraction\
Model struktur data
  + Jenis data yang disimpan
  + Operasi didukung pada mereka
  + Jenis parameter operasi
* Encapsulation\
Diasumsikan beberapa struktur data menjadi publik atau yang dianggap detail internal

4. Sebutkan contoh design pattern dalam Paradigma Object-Oriented!
Iterator Class

## Class and Object
1. Jelaskan definisi Class!\
Kelas adalah tipe data dari data dan metode
untuk jenis objek tertentu (cetak biru) Kelas berfungsi sebagai sarana utama untuk
abstraksi dalam pemrograman berorientasi objek. Kelas memiliki atribut dan metode.

2. Jelaskan perbedaan Attribute dengan Method!
* Attribute\
Informasi negara untuk masing-masing
* Method\
satu himpunan perilaku dalam bentuk fungsi anggota dengan implementasi yang umum untuk semua contoh dari kelas itu.

3. Jelaskan apa itu instansiasi Object!\
Proses membuat objek dari kelas menggunakan () setelah className dapat berisi parameter.

4. Jelaskan apa itu identifier!\
Sebuah pengenal atau pengidentifikasi yang kita deklarasikan agar kompiler dapat mengenalinya.

## Implementing Class
```
class Kendaraan:
  def __init__(self, nomorPlat, merk, jenis, warna, tanggalBeli, bulanBeli, tahunBeli, berat, harga):
    self.nomorPlat = nomorPlat
    self.merk = merk
    self.jenis = jenis
    self.warna = warna
    self.tanggalBeli = tanggalBeli
    self.bulanBeli = bulanBeli
    self.tahunBeli = tahunBeli
    self.berat = berat
    self.harga = harga
    
  def showTanggalPembelian(self):
    print(f" {self.tanggalBeli}/{self.bulanBeli}/{self.tahunBeli}")
```

## Main OOP Concept
1. Jelaskan konsep encapsulation dalam Paradigma Object-Oriented!\
Dapat membatasi akses ke metode dan variabel. Ini mencegah data dari modifikasi langsung. Dalam Python, kami menunjukkan atribut pribadi menggunakan garis bawah sebagai awalan yaitu satu _ atau dua kali __.

2. Jelaskan konsep inheritance dalam Paradigma Object-Oriented!\
Mekanisme untuk modular dan hierarki organisasi adalah teknik yang dikenal sebagai pewarisan.

3. Jelaskan perbedaan public method dan private method dalam encapsulation!\
* public method
```
def addentry(self, entry):
  self.entries.append(entry)
```
* private method
```
def lastentry(self):
  return self.entries[-1]
```

4. Jelaskan perbedaan superclass dan subclass dalam inheritance!
* Superclass (Polygon)
* Subclass (Triangle)

## Programming Exercise

```
class Koordinat:
	def __init__(self,x,y):
		self.z = 0
		self.x = x
		self.y = y
	def set_x(self,x):
		self.x = x
	def increment_x(self):
		self.x+=1
	def __str__(self):
		return f"x : {self.x} , y:{self.y} , z:{self.z}"
```
