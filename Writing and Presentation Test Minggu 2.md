Asyam Faiq
FEBE - 27
Politeknik Elektronika Negeri Surabaya

# Writing Minggu 2

### JavaScript Dasar
- *Javascript* adalah bahasa pemrograman populer yang digunakan untuk membuat situs dengan konten website yang dinamis

- Javascript dapat digunakan menggunakan browser seperti chrome atau mozila

- *Syntax* javascript sesuatu yang dapat diibaratkan sebagai kamus dan berperan dalam mengatur tata cara dalam bahasa pemrograman. Syntax digunakan untuk membuat statement program, instruksi untuk dijalankan atau dieksekusi oleh web browser dan compiler.

- Contoh syntax javascript : confirm, prompt, alert

- *Console Log* adalah tempat untuk melakukan pengecekan logic pemrograman serta pemeriksaaan apakah terdapat error atau tidak pada pemrograman.

- *Comments* adalah tanda untuk memberikan suatu baris agar tidak dibaca pada saat dijalankan. 2 jenis comments adalah Single comment dan Multiline Comments

- Tipe Data, 6 macam tipe data fundamaental pada javascript: 
  - Number : tipe data berupa angka.
  - String : tipe data berupa kalimat
  - Boolean: tipe data berupa true atau false
  - Null   : tipe data yang tidak memiliki nilai
  - Undefined : tipe data presentasi ke tidak adanya sebuah nilai
  - Object : tipe data berupa hal tertentu

- *Variabel* merupakan container atau wadah yang digunakan untuk menyimpan data atau nilai. cara mendeklarasikan variabel ada 3 yaitu var, let, dan const 

- Assignment Operator (=) digunakan untuk menyimpan sebuah nilai pada variabel

- *Mathematical Assignment Operator* adalah sebuah lambang untuk menentukan sebuah operasi matematika. 
contoh :<br/>
    ``let x = 20 ; ``  <br/>
    ``  x *= 2 ; `` <br/>
    `` console.log(x) // Output: 40``

- Increment dan Decrement digunakan untuk menambah atau mengurangi sebesar 1 nilai
contoh : <br/>
    ``let a = 20;``  <br/>
    ``  a-- `` <br/>
    `` console.log(a) // Output: 19``

- Arithmetic Operator digunakan apabila melibatkan operasi matematika. Seperti :
  - tambah (+)
  - kurang (-)
  - kali (*)
  - bagi (/)
  - modulus (%)

- Comparism Operator digunakan untuk membandingkan suatu nilai
  - Lebih Besar (>)
  - Lebih Kecil (<)
  - Lebih kecil atau samadengan (<=)
  - Lebih besar atau samadengan (>=)
  - Samadengan (===)
  - Tidak Samadengan (!==)

- *Logical Operator* digunakan untuk sebuah kondisi
  - AND operator (&&)
  - OR operator (||)
  - NOT operator (!)

### Conditional

- *Conditional* merupakan *statement percabangan* yang menggabarkan suatu *kondisi*
- Conditional statement akan melakukan pengecekan pada kondisi fisik dan menjalankan perintah berdasarkan kondisi tersebut
- Contoh Conditional
- IF Statement
- contoh conditional **if statement** :
  - Jika cuaca hari ini cerah, maka kita akan pergi keluar
  - jika saya lapar, maka saya makan
- contoh if statement 
  ```
  let nilai = 10;
  if (nilai === 10){
    console.log('variabel nilai yang disimpan adalah benar 10');
  }
  ```
- IF ... ELSE Statement
- contoh conditional **if else statement**
  ```
  let angka = 12;
  if (angka %2 == 0){
    console.log(angka + " adalah angka genap");
  } else {
    console.log(angka + " adalah angka ganjil")
  }
  ```
- IF ... ELSE IF Statement
- contoh conditional **if else if statement**
  ```
  let num1 = 10
  let num2 = 20

  if (num1 = num2){
      console.log(num1)
  } else if (num1 > num2){
      console.log(num1)
  } else {
      console.log(num2)
  }
  ```

- Switch Case Conditional digunakan jika kondisi percabangan terlalu banyak
- contoh conditional **switch case**

  ```
	let warna = "kuning";
 
		switch (warna){
			case "hitam":
				console.log ("warna hitam");
				break;
			case "merah":
				console.log ("warna merah");
				break;
			case "hijau":
				console.log ("warna hijau");
				break;
			default:
			    console.log ("warna tidak terdeteksi");
		}
  ```
- Ternary Operator merupakan short-syntax dari statement if ... else
- contoh ternary operator
  ```
  let isNowSale = true;
  isNowSale ? console.log('Let's shopping now) : console.log('Shopping later);
  ```

### Looping
- *Looping* merupakan statement yang mengulang suatu instruksi hingga kondisi terpenuhi atau jika kondisi stop atau berhenti
- Ada 3 macam looping yaitu :
  - For Loop 
  - While Loop
  - Nested Loop
- For Loop : digunakan jika kita tahu pasti seberapa banyak pengulangan yang ingin dilakukan pada program yang akan dikembangkan
- contohnya :
```
    let nilai = 1 ; 
    for (nilai; nilai <= 10 ; nilai++){
        console.log(nilai) 
    } 
```
- While Loop : akan menjalankan instruksi pengulangan bernilai TRUE
  Ada 2 macam while loop yaitu while dan do while
- contoh perulangan while :
```
    let count = 1 ; 
    while (count < 10){
        console.log(count);
        count ++ ;
    } 
```
- contoh perulangan do while :
```
    count = 1 ;
    do {
        console.log(count);
        count ++ ;
    } while (count <= 10)
```     
- Nested Loop : digunakan jika ingin membuat perulangan di dalam perulangan

### Scope dan Function
- *Scope* merupakan konsep dalam flow data varaiabel. 
Menentukan suatu variabel apakah bisa diakses pada scope atau tidak.
- Scope ada 2 macam yaitu global scope dan local scope
- contoh global scope :
```
    let myName = "chaca" ; 
    function greeting()
        return myName;
    {
        console.log(myName);
```
- contoh local scope :

- *Blocks* merupakan code yang berada dalam curly braces {}. Conditional, function dan looping menggunakan blocks.

- *Function* adalah sebuah code blok dalam sebuah grup untuk menyelesaikan 1 task
- Membuat function 
```
   function greeting() {
      return 'Hello World' ;
   };
```
- Cara memanggil function : 
```
 greeting()
 console.log(greeting()); 
 
 ```
- *Argumen dan Parameter*
- Argumen adalah nilai yang digunakan daat memanggil function. Jumlah argumen harus sama dengan jumlah parameternya. <br />
- contoh argumen :
```
  function penambahan(a,b){
   return a + b;
}
  console.log(penambahan(5,5))
```
- Parameter berfungsi untuk menerima sebuah inputan data yang digunakan untuk melakukan task. <br />
- contoh parameter :
```
function calculateArea(width,height){
  console.log(width * height);
}
```
- *Arrow Function* merupakan cara lain menuliskan function. ini adalah fitur terbaru yang ada pada ES6.
- contoh penulisan arrow function :
```
 const greeting = (a,b) => {
    return a + b;
}
```
- Short Syntax Function
- **Single Line Block** 
- ``const sumNumbers = number => number + number ; ``
- **Multi Line Block
```
  const sumNumbers = number => {
    const sum = number + number;
    return sum;
  }
```

### Data Type

### *DOM HTML*
- DOM merupakan cara memanipulasi html agar website lebih dinamis dan interaktif
- Cara memanggil DOM Value yaitu :
  - Memanggil tag HTML berdasarkan ID
  `` console.log(document.getElementByID("header))``
  - Memanggil tag HTML berdasarkan Class Name 
  `` console.log(document.getElementByClassName("text-color-blue"))``
  - Memanggil tag html berdasarkan query selector
  `` console.log(document.querySelector("#header "))`` 
  `` console.log(document.querySelector(".text-color-blue"))``
- Memanipulasi content
  Cara memanipulasi content :
  1. Deklarasi varible header sebagai wadah untuk menyimpan tag HTML
  `` let header = document.getElementById("header"); ``
  2. Memanipulasi Content pada Header Content dari pemilik element dengan ID Header dengan text.Content
  `` document.getElementById("header").textContent = "Teks Heading" `` <br />
     Memanipulasi Content didalam sebuah element dengan .innerHTML
  ```
  <ul id= "list"></ul>

  document.getElementById("list").innerHTML = "<li> item1 </li> <li> item2 </li>"
  ```
- Membuat Element HTML
- Contoh :
  ```
  <div id ="header"></div>

  //untuk membuat sebuah elemnt heading
  const heading = dosument.createElement("h1)
  heading.textContent = "Ini Heading"

  document.getElemntByID("header").appendChild(heading)
  ```

- *DOM Events* merupakan object model yang bertugas untuk membantu interaksi user dengan document HTML
- Contoh HTML DOM events
  - Click
  - Scroll
  - Change
  - Focus
  - Hover
  - Submit
  - Blur
- Menangkap Interaksi User
  - Element.addEventListener("event)
  - Element.onevent
- EventListener <br />
  Dengan menggunakan Element.addEventListener("event") dapat menerapkan beberapa hal yaitu :
  - Bisa dihilangkan
  - Bisa ada beberapa event listener yang sama untuk 1 element
  - Memiliki argument tambahan {options}
- Contoh EventListener :
  - EventListener - Click 
    `` <input id="user-input"/> ``
    `` <button id="alert-button">show</button> ``
    Memanggil element berdasarkan id
    `` const input = document.getElementById("user-input") ``
    `` const button = dosument.getElementById("alert-button") ``

    ```
     button.addEventListener("click", function()) {
      alert(input.value)
    } 
    ```
- EventListener - Blur : event dimana sebuah element kehilangan fokus dari user 
- Contoh EventListener - Blur <br />
  Misalkan saat ingin memvalidasi isi dari ``<input id = "username" />`` agar panjangnya minimal 6 karakter

  `` const input = document.getElementById("username") ``

  ```
  input.addEventListener("blur", () => {
    if(input.value.length < 6) alert("Panjang username minimal 6")
  })
  ```
- EventListener - Form Submission
- Contoh EvenListener - Form Submission <br />
  Misalkan terdapat beberapa input dalam sebuah form `` <input name="email"/> `` dan ``<input type="password" name="password"/>`` <br />
  Untuk mendapatkan isi dari kedua inputan tersebut terdapat 2 cara :
  - Memasang event listener di kedua input dan tombol submit, lalu saat tombol diklik, baca value dari kedua input tersebut
  - Memasang event listener di form, lalu gunakan FormData untuk menggambil data dari masing-masing input
  ``` 
    const form = document.getElementById("form")

    form.addEventListener("submit", function(event)){
    event.preventDefault()

    const formData = new FormData(form)
    const values = Object.fromEntries(formData) {
      email: ....
    }
  })
  ```