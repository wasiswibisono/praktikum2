# praktikum2
|Nama|NIM|Kelas|Mata Kuliah|
|----|---|-----|------|
|**Wasis Wibisono**|**312310661**|**TI.23.A6**|**Pemrograman Orientasi Objek**|

![gambar](latihan2/ss2.png)

# Input Code :
## • Deklarasi kelas Person
```java
public class Person {
    private String nama;
    private int umur;
```
### Penjelasan :
```
- public class Person: Menyatakan deklarasi kelas Person yang bersifat publik, artinya bisa diakses dari mana saja.
- private String nama;, private String jenisKelamin;, dan private int umur;: Mendeklarasikan tiga variabel instance (nama, jenisKelamin, umur) yang bersifat privat. Karena variabel ini privat, mereka hanya bisa diakses melalui metode getter dan setter dalam kelas Person.
```

## • Constructor Kelas Person
```java
 public Person(String nama, String jenisKelamin, int umur) {
        this.nama = nama;
        this.jenisKelamin = jenisKelamin;
        this.umur = umur;
    }
```
### Penjelasan :
```
- public Person(String nama, String jenisKelamin, int umur): Ini adalah constructor kelas Person. Constructor digunakan untuk menginisialisasi nilai nama, jenisKelamin, dan umur ketika objek 'Person' dibuat.
- this.nama = nama;, this.jenisKelamin = jenisKelamin, dan this.umur = umur;: this digunakan untuk membedakan antara variabel instance (yang ada dalam kelas) dan parameter yang diberikan pada constructor. Kode ini mengisi variabel instance dengan nilai yang diberikan saat objek dibuat.
```

## • Getter dan Setter
### Getter dan Setter untuk nama :
```java
public String getNama() {
        return nama;
    }

    public void setNama(String nama) {
        this.nama = nama;
    }
```
### Penjelasan :
```
- getNama(): Mengembalikan nilai nama.
- setNama(String nama): Mengubah nilai nama dari objek Person.
```

### Getter dan Setter untuk JenisKelamin :
```java
public String getJenisKelamin() {
        return jenisKelamin;
    }

    public void setJenisKelamin(String jenisKelamin) {
        this.jenisKelamin = jenisKelamin;
    }
```
### Penjelasan :
```
- getJenisKelamin(): Mengembalikan nilai jenisKelamin.
- setJenisKelamin(String jenisKelamin): Mengubah nilai jenisKelamin dari objek Person.
 
```

### Getter dan Setter untuk umur :
```java
public int getUmur() {
        return umur;
    }

    public void setUmur(int umur) {
        this.umur = umur;
    }
```
### Penjelasan :
```
- getUmur(): Mengembalikan nilai umur.
- setUmur(int umur): Mengubah nilai umur dari objek Person.
```

##  • Method main
```java
public static void main(String[] args) {
        Person Anton = new Person("Anton", "Laki-laki", 25);
        Person Riko = new Person("Riko", "Laki-laki", 30);
```
### Penjelasan :
```
- 'public static void main(String[] args)': Ini adalah method utama yang menjadi titik awal eksekusi program. Pada method ini, objek 'Anton' dan 'Riko' dari kelas 'Person' dibuat.
- 'Person Anton = new Person("Anton", "Laki-laki", 25);': Membuat objek 'Anton' dari kelas 'Person', dengan nilai 'nama' = '"Anton"', 'jenisKelamin' = '"Laki-laki"', dan 'umur' = '25''.
- 'Person Riko = new Person("Riko", "Laki-laki", 30);': Membuat objek 'Riko' dari kelas 'Person', dengan nilai 'nama' = '"Riko"', 'jenisKelamin' = '"Laki-laki"', dan 'umur' = '30'.
```

## • Mencetak informasi ke konsol
### Menampilkan informasi Anton :
```java
        System.out.println("Nama Anton: " + Anton.getNama());
        System.out.println("Jenis Kelamin Anton: " + Anton.getJenisKelamin());
        System.out.println("Umur Anton: " + Anton.getUmur());
```
### Menampilkan informasi Riko :
```java
        System.out.println("Nama Riko: " + Riko.getNama());
        System.out.println("Jenis Kelamin Riko: " + Riko.getJenisKelamin());
        System.out.println("Umur Riko: " + Riko.getUmur());
    }
}
```
### Penjelasan :
```
- System.out.println("Nama Anton: " + Anton.getNama());: Mengambil nilai nama dari objek Anton dengan menggunakan metode getter getNama() dan mencetaknya ke konsol.
- System.out.println("Jenis Kelamin Anton: " + Anton.getJenisKelamin());: Mengambil nilai jenisKelamin dari objek Anton dengan metode getJenisKelamin().
- System.out.println("Umur Anton: " + Anton.getUmur());: Mengambil nilai umur dari objek Anton dengan metode getUmur().
```

### Penjelasan :
```
Anton dan Riko adalah dua objek yang dibuat dari class Person.

- Anton memiliki nilai "Anton", "Laki-laki", dan 25 untuk atribut nama, jenisKelamin, dan umur.
- Riko memiliki nilai "Riko", "Laki-laki", dan 30 untuk atribut nama, jenisKelamin, dan umur.
```
