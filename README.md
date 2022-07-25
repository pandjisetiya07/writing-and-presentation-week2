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
Salah satu cara untuk menyelesaikan sebuah kondisi / percabangan yang banyak contohnya :
```
let kasus = 2
switch(kasus){
    case 1 :{
        console.log("kasus 1")
        break;
    }
    case 2 :{
        console.log("kasus 2")
        break;
    }
    case 3 :{
        console.log("kasus 3")
        break;
    }
    case 4 :{
        console.log("kasus 4")
        break;
    }
    default  :{
        console.log("TIdak ada Kasus")
    }
}
```
------------------------------------------------------------------------------------------

## __3. JavaScript - Looping__ <br>
Looping adalah statement yang mengulang sebuah instruksi hingga kondisi terpenuhi atau jika kondisi stop/berhenti tercapai. 

| __No__ | __Jenis Looping__ | __Penjelasan__ |
|--------|-------------------|----------------|
|   1    | For Loop          | Jenis Pengulangan yang bisa kita berikan pada program kita. For Loop digunakan apabila kita mengetahui __berapa banyak nilai pasti__ yang akan diulang |
|   2    | While Loop        | Akan menjalankan instruksi pengulangan kondisi bernilai TRUE. |
|   3    | Do While          | Melakukan perulangan terlebih dahulu tanpa melakukan pengecekan kondisi yang diinginkan |
|   4    | Nested Loop       | Kita membuat looping didalam looping.Looping pertama dianalogikan sebagai baris.Looping kedua dianalogikan sebagai kolom | <br>

------------------------------------------------------------------------------------------

## __4. JavaScript - Scope__ <br>
Sebuah Konsep dimana terdapat flow data variabel, yang dapat di akses pada scope tertentu atau tidak. Scope terbagi menjadi 2 yaitu : <br>
1. __Global Scope__ - > yaitu variabel yang dibuat dapat diakses dimanapun dalam satu file, dengan syarat __variabel harus dideklarasikan di __luar Block__.  <br>
```
let scopeGlobal = "Pandji"
function contoh(){
  return scopeGlobal
}

console.log(scopeGlobal)
```
2. __Local Scope__ -> yaitu variabel yang hanya bisa digunakan __didalam Block__ seperi _Function, Conditional, dan Looping_. dan tidak dapat di akses di luar blocks.
```
function contoh(){
  let scopeLocal = "Pandji setiya";
  return scopeLocal
}
console.log(contoh())
console.log(scopeLocal)
```

-------------------------------------------------------------------------------------------------

## __5. JavaScript - Function__ <br>
Sebuah Blok kode untuk menyelesaikan 1 task / 1 fitur, apabila nanti kita membutuhkan bisa kembali digunakan. contoh penulisan function
```
function contoh(){
  return 'contoh Function'
}
```
Dalam _function_ terdiri dari __Function Keyword__ , __Identifier/penamaan fungsi__,dan __Fucntion body__

__- Parameter dan Argumen__ <br>
1. __Parameter Function__ -> function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas.Saat membuat function/fitur, kita harus tahu data-data yang dibutuhkan.
```
function perkalian(a,b){
  return a * b
}
```
dalam contoh kasus diatas saya ingin melakukan perkalian maka dibutuhkan 2 buah nilai / parameter yaitu __(a,b)__ dan diletakkan pada fungsi yang nantinya akan di proses. <br>

2. __Argumen Function__ <br>
Argumen adalah nilai yang digunakan saat memanggil function. Jumlah argumen harus sama dengan jumlah parameternya Jadi jika di function penambahan ada 2 parameter nilai saat membuat function. Saat memanggil function kita gunakan 2 buah nilai argumen.
```
function perkalian(a,b){
  return a * b
}
console.log(perkalian(10, 2))
```
__- Default Parameters__ <br>
Default paramaters digunakan untuk memberikan nilai awal/default pada parameter function. Untuk menghindari eror saat pemanggilan tanpa adanya argumen dalam fungsi tersebut.
```
function defaultParameter(pekerjaan = 'Front End'){
    return 'devisi saya di' + pekerjaan
}
console.log(defaultParameters('IT')) // maka akan muncul "devisi saya di IT"
console.log(defaultParameters()) // maka akan muncul "devisi saya di Front End"
```
------------------------------------------------------------------------------------

## __6. JavaScript - DOM__ <br>
Javascript DOM (Document Object Model) adalah interface yang memungkinkan developer untuk memanipulasi konten, struktur, dan style situs web

__Mencari Element HTML__ <br>
Untuk mencari element HTML seperti __ID__ dan __CLASS__ pada JavaScript dapat menggunakan beberapa cara seperti :
```
//mencari 1 element dengan id tertentu di HTML
console.log = document.getElementById("nama_ID")

//mencari beberapa element dengan class tertentu di HTML
console.log = document.getByClassName("nama_Class")

//pemanggilan menggunakan query selector(satu tag)
console.log = document.querySelector("#nama_id" / ".nama_Class")

//memanggil seluruh Atribut di HTML(semua tag)
console.log = document.querySelectorAll("#nama_Id" / ".nama_Class")
```

__Mengubah Konten Element__
Memungkinkan kita mengubah konten dan style elemen HTML dengan mengubah propertinya.seperti :
```
//penggunaan InnerHTML
//dalam kasus ini dom dapat melakukan manipulasi tampilan.
console.log = document.getElementById("nama_Id").textContent = "rubah isi content"

//penggunaan innerHTML
console.log = document.getElementById("nama_Id").innerHTML = "<h1> Rubah isi content </h1> "
```
Perbedaan yang terdapat di __textContent__ dan __innerHTML__ yaitu saat menggunakan _innerHTML_ dapat menjalankan tag yang ada di HTML dan merubah isi kontennya. sedangkan _textContent_ hanya bisa merubah isi konten tanpa menjalankan tag HTML seperti ``<h1>``, ``<p>``, dll.