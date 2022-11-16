# Variabel

## Apa itu Variabel?

Variabel adalah suatu wadah untuk menyimpan suatu informasi/data di dalam memori. Variabel terdiri dari 3 hal, yaitu nama, tipe, dan isi dari variabel itu sendiri.

## Membuat Variabel

Variabel dapat dibuat dengan cara menuliskan tipe data, diikuti dengan nama variabel. Proses ini sering disebut dengan **Deklarasi Variabel**.

```
[tipe data] [nama variabel];
```

Contoh:

```csharp
string nama;
int umur;
float nilai;
bool sukaKucing;
```

### Membuat Banyak Variabel Sekaligus

Jika ada banyak variabel dengan tipe data yang sama.

```csharp
int panjang;
int lebar;
int tinggi;
```

Pembuatan variabel dapat disingkat menjadi

```csharp
int panjang, lebar, tinggi;
```

## Mengisi Variabel

Variabel dapat diisi dengan cara menuliskan nama variabel, diikuti dengan tanda sama dengan `(=)` dan nilai yang akan diberikan.
Nilai yang akan digunakan untuk mengisi variabel harus sesuai dengan tipe data dari variabel itu sendiri.

```csharp
[nama variabel] = [nilai];
```

Contoh:

```csharp
nama = "Fafa";
umur = 22;
nilai = 6.9;
sukaKucing = true;
```

### Mengisi Variabel pada saat Deklarasi

Variabel dapat diisi kapan saja, namun terkadang ada suatu keadaan dimana suatu variabel harus diisi tepat setelah variabel itu dideklarasi.

```csharp
string planet;
planet = "Bumi";
```

Pembuatan dan pengisian variabel dapat disingkat menjadi

```csharp
string planet = "Bumi";
```

### Mengisi Banyak Variabel Sekaligus

Jika ada banyak variabel yang diisi dengan nilai yang sama.

```csharp
panjang = 10;
lebar = 10;
tinggi = 10;
```

Pengisian variabel dapat disingkat menjadi

```csharp
panjang = lebar = tinggi = 10;
```

## Mengakses Isi dari Variabel

Nilai dari variabel dapat digunakan untuk berbagai hal tergantung keadaan dalam program itu sendiri.

### Menampilan Isi dari Variabel ke Console

```csharp
string nama = "Fafa";
Console.WriteLine(nama);
```

Hasilnya

```
Fafa
```

### Mengisi Variabel menggunakan Variabel Lainnya

```csharp
string nama = "Fafa";
string nama2 = nama;
Console.WriteLine(nama);
Console.WriteLine(nama2);
```

Hasilnya

```
Fafa
Fafa
```

### Melakukan Operasi yang Melibatkan Variabel

```csharp
int panjang = 10;
int lebar = 5;
int luas = panjang * lebar;
Console.WriteLine(luas);
```

Hasilnya

```
50
```

## Konstan

Secara default nilai dari suatu variabel dapat diubah terus menerus, namun terkadang ada suatu keadaan dimana nilai dari suatu variabel itu tidak boleh diubah, misalnya variabel untuk menyimpan π.
Hal tersebut dapat dilakukan dengan cara menambahkan kata `const` pada saat pembuatan dan pengisian variabel.

```csharp
const [tipe data] [nama variabel] = [nilai];
```

Contoh:

```csharp
const double pi = 3.14;
pi = 3; // Error
```
