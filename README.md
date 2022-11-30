# Writing-Test-Week3
Week 3
**Senin, 3 Oktober 2022**
### JavaScript - Array, JavaScript - Multidimensional Array


#### JavaScript - Array dan Multidimensional Array

Array adalah tipe data list order yang dapat menyimpan tipe data apapun di dalamnya
Array dapat menyimpan tipe data String, Number, Boolean, dan lain2

contoh dari array multidemensi adalah sebagai berikut let inventory = [ ['kaos ',18], ['Jaket',14], ['Sepatu',12], ['Celana',5] ];
Adapun jika kita ingin memanggill jaket hodie dapat memakai codingan console.log(inventory[3][0]);
Jika kita ingin melakukan push ke array multidemensi sama dengan array biasa yaitu inventory.push(['Sandal',40])
sama seperti array kita bisa membaca semua isi multiarray dengan menggunakan forEach adapun contoh codenya sebagai berikut inventory.forEach((baris)=> { baris.forEach((column) => { console.log(column); }) })

**Selasa, 4 Oktober 2022**
### JS Intermediate - Object

Object dalam programming adalah sebuah tipe data pada variabel yang menyimpan properti dan fungsi(method)
Properti adalah data lengkap dari sebuah object
Method adalah action dari sebuah object seperti apa saja yang dapat dilakukan dari suatu object

Cara membuat Object let nama_objt = { key1 : "value", key2 : "value2" }
Cara akses Object
objt.key1 (memakai dot notation)
objt["key2"] (memakai bracket)
Cara menambahkan key ke object / mengganti value di obj
Objct.key3 = value / objt["key4"] = value


log() adalah property yang berupa function dari object console, sehingga memanggilnya dengan cara `console.log()`

#### Nested Object
Pada real application akan menemukan data object yang kompleks, yang berasal dari turunan object lainnya.



#### Looping Object
Jika ingin menampilkan seluruh object properti bisa menggunakan looping






#### Array of Object
Array object berfungsi untuk menyimpan beberapa nilai dalam satu variabel adapun cara mendeklarasi dan membuar array object seperti dibawah ini let users = [ {
`nama: "Dea Oktavia",`
` umur: 21,`
` alamat: "surabaya",`
`},`
 `  {`
   `   nama: "Dafiq",`
  `    umur: 21,`
 `     alamat: "Surabaya",`
`    },`
 `   {`
`      nama: "Ega",`
     ` umur: 27,`
  `    alamat: "Surabaya",`
  `  },`
`  ];`

**Rabu, 5 Oktober 2022*
### JS Intermediate - Recursive

#### Recursive
Rekursif adalah function yang memanggil dirinya sendiri sampai kondisi tertentu
Rekursif kebanyakan digunakan untuk case matematika, fisika, kimia, dan yang berhubungan dengan calculation
Ciri dari rekursif :
Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti. Kondisi ini harus dapat dibuktikan akan tercapai, karena jika tidak maka kita tidak dapat membuktikan bahwa fungsi akan berhenti, yang berarti algoritma kita tidak benar
Fungsi rekursif selalu memanggil dirinya sendiri sambil mengurangi atau memecahkan data masukan setiap panggilannya

Contoh kasus rekursif 








**Kamis, 6 Oktober 2022**
### JS Intermediate Asynchronous - Introduction and Promise

#### Asynchronous
JS sendiri merupakan bahasa yang :
Single-thread merupakan sistem yang hanya mempunyai 1 jalur(1 kasir)
Non-blocking artinya proses dapat disela oleh proses lain
Asynchronous adalah proses yang dilakukan secara tidak berurutan,misal A baru berjalan 70% setelah itu di sela B dan >Kembali lagi ke A 30%
#### Callback
function yang dijadikan sebagai argumen,contoh code sebagai berikut : setTimeout(() => {
   console.log("A");
  }, 1200);

  setTimeout(() => {
    console.log("B");
  }, 1000);

  console.log("C");
 
#### Promises
objek JS yang menautkan kode dan menghasilkan(kode yang memakan waktu lama) dan mengkonsumsi(kode yang menunggu hasilnya) kode,adapun contoh codenya sebagai berikut : let nontonPromise = new Promise((resolve,reject) => {
 resolve("Nonton terpenuhi")

          reject("gagal")
 
})
console.log("A"); nontonPromise.then(result => {
 console.log(result)
 
})
.catch((err) => { console.log(err); })
console.log("C");
#### async await
Merupakan salah satu fitur ES mulai 2017,fitur ini mempermudah dalam menangani proses asynchronous adapun contoh codingannya sebagai berikut async function myFunction() { // This is an async function }










**Jum’at, 7 Oktober 2022**
### JS Intermediate - Web Storage

#### Web Storage
web storage adalah untuk menyimpan data dari aplikasi ke browser dan bersifat local,adapun perbedaan antara session storage,local storage dan cookie sebagai berikut Local storage
Capacity 10 MB
Expired (never)
Penyimpanan hanya dapat dilakukan di browser
Tidak melakukan sent with request
#### Session storage
Capacity 5 MB
Expired ketika Tab close
Penyimpanan hanya dapat dilakukan di browser
Tidak dapat melakukan sent with request
#### Cookies
Capacity 4 KB
Expired dapat diset secara manual
Penyimpanan dapat dilakukan di browser dan server
Dapat melakukan sent with request
Meskipun penyimpanan web storage besar tetapi jangan menyimpan data sensitive seperti otentikasi,password dan data lainnya adapun study case jika 
Belajar web storage adalah dark mode,todo dan detail page sebagai informasi Local storage hanya dapat menerima bentuk string.
adapun code jika kita ingin menyimpan ke local storange adalah `localStorange.setItem("key”,[“value1”,”value2”])`
Sedangkan jika kita ingin mendapatkan data dari local storange dapat melakukan localStorange.getItems(“key”)


