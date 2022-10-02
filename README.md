# Writing-Week-2
## Properties and Method
- Properties adalah ciri/nilai yang berkaitan dengan object 
- Method adalah sebuah fungsi
### Type Data 
type data terbagi menjadi dua : 
- primitiv : string, number, boolean
- non primitiv : array, object
#### string
```js
//string
let hewan = "kAnCIl"
console.log(hewan) //output : kAnCIL

console.log(typeof hewan) //output : string

// properties
console.log(hewan.length); //output : 6 
```
- toUppercase : untuk membuat huruf besar semua
```js
//method
console.log(hewan.toUpperCase()) //output : KANCIL 
```
- toLowerCase : untuk membuat huruf kecil semua
```js
console.log(hewan.toUpperCase()) //output : kancil
```
- charAt : untuk mengembalikan nilai dari string
``js
console.log(hewan.charAt(1)) //output : A
```
- includes : untuk melakukan pencarian. Jika ditemukan mengembalikan nilai true, jika tidak maka akan mengembalikan nilai false
``js
console.log(hewan.includes("s")) //output : true
```
- split 
```js
let kalimat = "dengan menggunakan split(), kita dapat memisahkan sebuah string menjadi data array"
console.log("BEFORE", kalimat)
console.log("AFTER", kalimat.split(" ")); 
//output : BEFORE dengan menggunakan split(), kita dapat memisahkan sebuah string menjadi data array
//output : AFTER (11) ['dengan', 'menggunakan', 'split', 'kita', 'dapat', 'memisahkan', 'sebuah', 'string', 'menjadi', 'data', 'array']
```
- reverse : mengubah kata/kalimat menjadi terbalik
```js
console.log("hallo".reverse()) //output : alloh
```
#### Number
```js
//number
console.log(Number("123")); // 123 in Number
```
- Number.Nan : untuk mengecek apakah itu sebuah number atau bukan
```js
console.log(isNaN(2131)) // false
console.log(isNaN("dawdf")) // true
```
- toString : mengubah angka menjadi sebuah string
```js
let angka = 20 //output : undefined
angka.toString() //output : 20
```
- toFixed : mengambil beberapa angka dibelakang koma, dan berubah menjadi string
```js
let angka = 3.12345
console.log(angka.toFixed(1)) // output : 3.1
```
- math. Abs : membuat minus jadi plus
```js
// properties
console.log(Math.PI)

// method
console.log(Math.abs(-5)) // output : 5
```
- math.pow : pangkat
```js
console.log(Math.pow(3, 2)) //output : 9
```
- math.round : membulatkan angka
```js
console.log(Math.round(5.6)) // output : 6
```
- math.floor : membulatkan kebawah
```js
console.log(Math.floor(5.6)) // output : 5
```
- math.ceil : membulatkan keatas
```js
console.log(Math.ceil(5.2)) // output : 6
```
- math.random : 
```js
console.log(Math.random()) // output : 0.123342
```
#### date
```js
console.log(Date()) // output : 'Tue Sep 27 2022 20:31:20 GMT+0700 (Indochina Time)'
console.log(date.getFullYear()); // output : 2022
```
## DOM (Document Object Model)
- DOM (Document Object Model): jembatan supaya Bahasa pemrograman dapat berinteraksi dengan dokumen html. 
- Dengan DOM, javascript dapat memanipulasi html
- Dom bukan bagian dari JavaScript, melainkan bagian dari web API untuk membuat website.
- Dom dalam bentuk tree structure
![image](https://user-images.githubusercontent.com/114098894/193461394-e2c78305-d2a8-4f3e-ac0b-117ddf854130.png)

- Ada 2 item, ketika mengakses dom :
  1. element : Cuma html element (<span>, <div>)
  2. node : setiap bagian terkecil di html (text, comment, <span>)
- Element2 menggunakan dom -> traversing :
  - Ke bawah : getElementById, getElementsByClassName, getElementByTagName, querySelector family(querySelector, querySelectorAll), children
  - Ke atas : parentElement, closest()
  - Ke samping : nextElementSibling, previousElementSibling
- HTML Collection bukan array, cara aksesnya mirip dgn array
- Property dan method dalam html collection: length, item(), namedItem()
- HTML collection mirip dengan node list, keduanya memiliki length, 
- Html collection : koleksi dlm bentuk dokumen element
- Node list : dokumen dlm bentuk nodes (element nodes, attribute nodes, text nodes)

