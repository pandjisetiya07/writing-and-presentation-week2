# TUGAS WRITING-AND_PRESENTATION-WEEK2

__PANDJI SETIYA BUDHI ARTHA__ -- _Tugas writing minggu kedua_

| __No__ | __Materi untuk minggu kedua__ | 
|----|-----------------------------|
|  1 | JavaScript - Introduction |
|  2 | JavaScript - Conditional  |
|  3 | JavaScript - Looping      |
|  4 | JavaScript - Scope        |
|  5 | JavaScript - Function     |
|  6 | JavaScript - DOM          |

--------------------------------------------------------------------------------------------

## __1. JAVASCRIPT - INTRODUCTION__ <br>
Javascript adalah bahasa pemograman yang saat ini sering digunakan untuk membuat website. Dengan ditambahkan javascript akan membuat website menjadi lebih interaktif dan dinamis

__- Tipe data pada JavaScript__ <br>

| __No__ | __Tipe Data__ | __Penjelasan__ |
|--------|---------------|----------------|
|   1    | Number        | Merupakan tipe data berupa angka yang bernilai bulat maupun desimal. Tipe data Number dibagi lagi menjadi 2 yaitu : <br> 1.  Integer -> untuk bilangan bulat yang bernilai _Positif atau Negatif_ <br> 2. float / desimal -> untuk bilangan yang bernilai _Desimal_ |
|   2    | String        | Kumpulan karakter yang bernilai __huruf, angka, spasi, dan symbol yang diawali dengan tanda "......"__ |
|   3    | Boolean       | Merupakan tipe data yang mempunyai 2 nilai yaitu __TRUE atau FALSE__ | 
|   4    | Null          | Tipe data yang diartikan bahwa sebuah variable/data tidak memiliki nilai. | 
|   5    | Undefined     | Tipe data yang merepresentasikan varibel/data yang tidak memiliki nilai. Undefined didapat dari hasil berikut: <br> - Nilai dari pemanggilan variabel yang belum didefinisikan. <br> - Nilai dari pemanggilan element array yang tidak ada. <br> - Nilai dari pemanggilan property objek yang tidak ada. <br> - Nilai dari pemanggilan fungsi yang tidak mengembalikan nilai (return). <br> - Nilai dari parameter fungsi yang tidak memiliki argumen. |
|   6    | Object        | Tipe data yang dapat menyimpan data dengan tipe apapun seperti, Number, String, Boolean, dan lainnya | 

--------------------------------------------------------------------------------------------

__- Variabel JavaScript__ <br>
Variabel yaitu tempat atau wadah yang digunakan untuk menyimpan sebuah nilai. 3 hal yang dapat dilakukan sebuah Variabel : <br>
1. Membuat Variabel dengan __nama yang jelas__. <br>
2. Dapat menyimpan dan mengupdate informasi atau data yg disimpan.
3. Mendapatkan data yang disimpan. 

---------------------------------------------------------------------------------------------

## __2. JavaScript - Conditional__ <br>
Merupakan __percabangan__ yang menggambarkan suatu __kondisi__.  Conditional statement akan mengecek kondisi spesifik dan menjalankan perintah berdasarkan kondisi tersebut, yang di cek apakah kondisi tersebut sudah __TRUE(benar)__. <br>

---------------------------------------------------------------------------------------------

__- Contoh Conditional__ <br>
1. __IF Statement__ -  memungkinkan untuk membuat perbandingan logis antara nilai dan apa yang diharapkan dengan menguji kondisi dan mengembalikan hasil jika True atau False contohnya. <br>
```
let variabel = 10
if (variabel === 10){
    console.log('Ini benar variabel bernilai 10')
} 
// apa bila value pada let bukan nilai 10 maka tidak akan muncul / undefined
```

2. __IF...ELSE IF Statement__ - digunakan untuk menentukan kondisi kedua, apabila setelah pengujian pada kondisi yang pertama salah, dan akan di eksekusi jika kondisinya benar.
```
let buah = 'apel';

if(buah == 'jeruk') {
	console.log('Ini bukan buah apel');
} else if(buah == 'apel') {
	console.log('Ini adalah apel');
} else {
    console.log('Ini bukan buah');
}
```
3. __IF...ELSE Statement__ - digunakan apabila semua kondisi sebelumnya salah, maka ELSE adalah opsional dari kondisi-kondisi lainnya dan akan di eksekusi.
```
var jam = 18;

if(jam > 18) {
	console.log('Selamat malam');
} else {
	console.log('Selamat siang');
}
```
--------------------------------------------------------------------------------------------
__- Truthy and Falsy Assignment__ <br>
Sebuah website yang memiliki inputan, tetapi tidak diniputkan maka dapat dapat mengisinya dengan nilai default yang di buat, contohnya :
```
let pekerjaan = ""
let dataPekerjaan = pekerjaan || "belum bekerja"
console.log(dataPekerjaan)
```

__- Switch Case__ <br>
