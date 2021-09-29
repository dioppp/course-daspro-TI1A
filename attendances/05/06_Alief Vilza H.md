## JOBSHEET 5

## PEMILIHAN 1

### Tujuan

Mahasiswa mampu menyelesaikan permasalahan/studi kasus menggunakan sintaks pemilihan 1 dan mengimplemantasikannya dalam bahasa pemrogaman java.

### Alat dan Bahan
+ PC/laptop
+ Browser(chrome, firefox, safari)
+ Koneksi internet

### Praktikum

#### Percobaan 1 : Penggunaan if

#### Waktu percobaan : 40 menit

1. Perhatikan flowchart dibawah ini!

    <p align="left">
    <img width="351" height="460" src="images/01.png">
    </p>
    

> Flowchart diatas digunakan untuk menentukan bilangan ganjil/genap, selanjutnya kita akan membuat programnya berdasarkan
> flowchart di atas!

2. Tambahkan library Scanner, deklarasi Scanner, dan buat variabel bil untuk menampung data yang diinput melalui keyboard

    ![](images/03.png)


```Java
Penjelasan kode program yang mempunyai peran mencari data tertentu,supaya bisa di run ke tahap selanjutnya 
```


```Java
// Ketik kode program di atas di bawah sini
import java.util.Scanner;
Scanner input = new Scanner (System.in);
int bil;
System.out.println("Masukkan sebuah bilangan ");
bil = input.nextInt();
```

    Masukkan sebuah bilangan 
    3



```Java
Penjelasannya kode program yang berfungsi sebagai penyeleksi bilangan angka tersebut, agara mempunyai output bilangan genap
ataupun ganjil, tergantung nantii kita membaginya dengan angka berapa 
```

3. Buatlah struktur kondisi untuk mengecek apakah bilangan tersebut merupakan bilangan genap atau ganjil

    ![](images/04.png)


```Java
// Ketik kode program di atas di bawah sini
if(bil%2 == 0){
    System.out.println("Bilanagan Genap");
}else{
    System.out.println("Bilangan Ganjil");
}    

```

    Bilangan Ganjil



```Java
Penjelasannya karena kde program yang tersebut memliki sintaks yang berbeda namun mempunyai konsep kode program yang sama 
jika dibagi 2 contoh outputnya
```

##### Pertanyaan
1. Modifikasi program diatas dibagian struktur pemilihannya sehingga menjadi sebagai berikut:

    ![](images/05.png)


```Java
// Ketik kode program di atas di bawah sini
String output = (bil % 2 == 0) ? "Bilangan Genap":"Bilanagan Ganjil";
System.out.println(output);

```

    Bilanagan Ganjil



```Java
penejlasannya memiliki fungsi yang sama yaitu meyeleksi bilanagan tertentu agar dapat berjalan ke tahap selnajutnya 
```

2. Jalankan dan amatilah hasilnya!
3. Jelaskan mengapa output program yang dimodifikasi sama dengan output program sebelum dimodifikasi!

#### Percobaan 2 : Penggunaan if else

#### Waktu percobaan : 40 menit

+ Buatlah sebuah variabel nilai untuk menyimpan inputan dari keyboard

    ![](images/06.png)


```Java
// Ketik kode program di atas di bawah sini
int nilai;
System.out.print("Masukan sebuah bilanagan: ");
nilai = input.nextInt();
 
```

    Masukan sebuah bilanagan: 5



```Java
penjelesannya program menunjuk bilangan yang bermaksud jika ada bilangan 
```

+ Tambahkan sebuah kondisi untuk mengecek input pada variabel nilai

    ![](images/07.png)


```Java
// Ketik kode program di atas di bawah sini
if(nilai >= 100){
    nilai += 10;
}else{
    nilai -= 10;
}
System.out.println("Hasil akhir nilai adalah "+nilai);

```

    Hasil akhir nilai adalah -15



```Java
penjelasan program tersebut menunjukan untuk menghitung bilangan,yang bermaksud denga tujuan jika ada bilangan yang bernilai diatas 
angak seratus makan akan ditmbah 10 begitupun dengan sebaliknya 
```

+ Jalankan program. Amati apa yang terjadi!

##### Pertanyaan
1. Jelaskan fungsi kode program berikut:
    
    ```
    nilai+=10;
    nilai-=10;
    ```

2. Modifikasilah program diatas dimana inputannya yang awalnya hanya satu kemudian diganti 2 inputan (misal : nilai1 dan nilai2), lakukan perhitungan rata-rata kedua nilai tersebut jika nilainya lebih dari sama dengan 100 maka dikurangi 5, sedangkan jika nilai rata-rata tersebut kurang dari 100 maka akan langsung dicetak!


```Java
Penjelasa fungsi program tersebut untuk menambah dan mengurangi bilangan dengan angka sepuluh
```

#### Percobaan 3 : Penggunaan if else-if else

#### Waktu percobaan : 40 menit

+ Tambahakan library `Scanner`
+ Buatlah deklarasi `Scanner`
+ Buat variabel umur bertipe `int`

    ![](images/08.png)


```Java
// Ketik kode program di atas di bawah sini
int umur;
System.out.print("Masukan umur anda: ");
umur = input.nextInt();

```

    Masukan umur anda: 19



```Java
prgram tersebut untuk menginput umur 

```

+ Kode untuk melakukan pengecekan variabel `umur`

    ![](images/09.png)


```Java
// Ketik kode program di atas di bawah sini
if(umur > 60)
    System.out.println("Lansia");
else if (umur > 45)
    System.out.println("Tua");
else if (umur > 17)
    System.out.println("Dewasa");
else if (umur > 5)
    System.out.println("Anak-anak");
else
    System.out.println("Balita");
```

    Dewasa



```Java
penejelasannya tipe data yang digabung menggunakan scanner system sehingga digunakan dalam 
menyeleksi atau melihat umur 
```

+ Jalankan program dan amati apa yang terjadi!

##### Percobaan 4 : Penggunaan switch-case

#### Waktu percobaan : 40 menit

1. Deklarasikan Scanner
1. Buatlah variabel-variabel berikut

    ![](images/10.png)


```Java
// Ketik kode program di atas di bawah sini
Scanner sc = new Scanner (System.in);
double angka1, angka2, hasil;
char operator;

```


```Java
untuk membuat varibael 
```

3. Kode program untuk meminta inputan dari keyboard

    ![](images/11.png)


```Java
// Ketik kode program di atas di bawah sini
System.out.print("Masukan angka pertama: ");
angka1 = sc.nextDouble();
System.out.print("Masukkan angka kedua: ");
angka2 = sc.nextDouble();
System.out.print("Masukkan operator (+ - * /): ");
operator = sc.next().charAt(0);
```

    Masukan angka pertama: 12
    Masukkan angka kedua: 6
    Masukkan operator (+ - * /): (+ - * /) :


4. Kode di bawah ini untuk melakukan pengecekan operator yang digunakan sebelum dilakukan operasi aritmatika

    ![](images/12.png)


```Java
// Ketik kode program di atas di bawah sini
switch (operator){
    
case '+':
hasil = angka1 + angka2;
System.out.println(angka1 + " + " + angka2 + " = " + hasil);
break;
case '-':
hasil = angka1 - angka2;
System.out.println(angka1 + " - " + angka2 + " = " + hasil);
break;
case '*':
hasil = angka1 * angka2;
System.out.println(angka1 + " * " + angka2 + " = " + hasil);
break;
case '/':
hasil = angka1 / angka2;
System.out.println(angka1 + " / " + angka2 + " = " + hasil);
break;
default:
System.out.println("Operator yang anda masukan salah");
    
}
```

    Operator yang anda masukan salah



```Java
untuk menghitung suatau bilanga entah itu pengurangan ataupun penjumlahan
```

5. Jalankan program. Amati apa yang terjadi!

##### Pertanyaan
1. Jelaskan fungsi dari break dan default pada percobaan 4 diatas!
penjelasannya untuk mngetahui sebuah kasuh perhitungan 


2. Jelaskan fungsi perintah kode program dibawah ini pada percobaan 4!

dilakukan untuk melakka stop jika perintah yang diberikan sudah dirasa cukup untuk case tersebut

    ```
    operator = sc.next().chartAt(0);
    ```


```Java
Digunakan untuk mengambil sebuah karakter 
```

### Tugas

#### Waktu pengerjaan Tugas: 140 menit

1. Buatlah program untuk menginputkan dua buah bilangan bulat, kemudian mencetak salah satu bilangan yang nilainya terbesar.
```Java
import java.util.Scanner;
public class inputduabilangan {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        int a, b;
        System.out.println("Masukan angka a: ");
        a = sc.nextInt();
        System.out.println("Masukan angka b: ");
        b = sc.nextInt();

        if (a>=b){
            System.out.println("a merupakan yang terbesar dengan nilai :" +a);
        }
        else {
            System.out.println("b merupakan yang terbesar dengan nilai :" +b);
        }

    }


}


2. Perhatikan flowchart berikut ini:

![](images/02.png)

> Buatlah program sesuai dengan flowchart diatas!
```Java
import java.util.Scanner;
public class berkendara {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);
        int umur;

        System.out.println("Masukkan umur anda: ");
        umur = input.nextInt();

        if (umur>=17){
            System.out.println("Boleh berkendara");
        }
        else {
            System.out.println("Tidak Bisa Berkendara");
        }
    }
}


3. Pada akhir semester seorang dosen menghitung nilai akhir dari mahasiswa yang terdiri dari nilai uas, uts, kuis, dan tugas. Nilai akhir didapatkan dari 40% nilai uas, 30% nilai uts, 10% nilai kuis, dan 20% nilai tugas. Jika nilai akhir dari mahasiswa dibawah 65 maka mahasiswa tersebut akan mendapatkan remidi. Buatlah program untuk membantu mengetahui mahasiswa yang mendapatkan remidi berdasarkan nilai akhir yang didapatkannya!
```Java
import java.util.Scanner;
public class nilairemidi {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double uas, uts, kuis, tugas, nilaiAkhir;

        System.out.println("Nilai Uas: ");
        uas = sc.nextDouble();
        System.out.println("Nilai Uts: ");
        uts = sc.nextDouble();
        System.out.println("Nilai Kuis: ");
        kuis = sc.nextDouble();
        System.out.println("Nilai Tugas: ");
        tugas = sc.nextDouble();
        uas = 0.4;
        uts = 0.3;
        kuis = 0.1;
        tugas = 0.2;
        nilaiAkhir = uas + uts + kuis + tugas;

        if (nilaiAkhir<=65){
            System.out.println("Maaf silahkan mengikuti Remidi: "+nilaiAkhir);
        }
        else{
            System.out.println("Selamat Anda Lulus");
        }
    }
}


4. Sebuah toko memberikan diskon kepada pelanggannya dengan ketentuan sebagai berikut:

| Total Belanja     | Potongan |
|-------------------|----------|
| >Rp. 200.000,00   | 2%       |
| >Rp. 500.000,00   | 5%       |
| >Rp. 1.000.000,00 | 10%      |

> Total belanja diperoleh dari pembelian tiga barang yaitu barang A, barang B, dan barang C. Ketika menginputkan harga barang juga menginputkan jumlah barang yang dibeli.

Contoh outputnya
```
Masukkan harga barang A   :100000
Masukkan jumlah barang A  :10
Masukkan harga barang B   :250000
Masukkan jumlah barang B  :5
Masukkan harga barang C   :150000
Masukkan jumlah barang C  :1
---------------------------------------------
                Struk total
---------------------------------------------
Nama Barang 	| 	Harga 	| 	Jumlah 	| 	Total
Barang A            100000         10        1000000   
Barang B            250000         5         1250000   
Barang C            150000         1         150000    
Total       :2400000
Diskon      :240000.0
Total Bayar :2160000.0
```