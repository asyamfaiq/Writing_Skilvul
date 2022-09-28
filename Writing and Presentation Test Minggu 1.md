Asyam Faiq
FEBE - 27
Politeknik Elektronika Negeri Surabaya

# Writing and Presentation Test Minggu 1

### Unix Command Line 
- *Shell* adalah perantara yang digunakan user dan sistem operasi dalam berkomunikasi menggunakan perintah-perintah.
- Contoh terminal basic pada Windows adalah *powershell* dan *command prompt* (CMD).
- *Command Line* merupakan sebutan untuk shell yang berbasis teks.
- *Command Line* interface merupakan tampilan dari sebuah terminal yang digunakan untuk menjalankan suatu program, mengelola file, dan berinteraksi dengan komputer.

Beberapa command line yang dipelajari adalah sebagai berikut:

#### 1. Navigation, Files, and Directory
- *<strong>cd</strong>*: berpindah dari directory ke directory lain
- *<strong>pwd</strong>*: mengetahui posisi direktori
- *<strong>ls</strong>*: menampilkan isi dari posisi directory
- *<strong>ls - la</strong>*: menampilkan seluruh isi dari suatu directory termasuk *hidden files*
  
#### 2. File Manipulation
- *<strong>touch</strong>*: membuat file baru
- *<strong>mkdir</strong>*: membuat directory baru  
- *<strong>cp</strong>*: menyalin file
- *<strong>mv</strong>*: memindahkan file atau directory dan dapat merename
```mv [source] [destination]```
- *<strong>rm</strong>*: menghapus file 
- *<strong>rmdir</strong>*: menghapus directory

### Git dan Github 
- Git merupakan tools untuk mengontrol dan mengatur versi suatu   file. Selain digunakan sebagai *version control system*, git dapat digunakan untuk menyimpan log segala perubahan pada suatu file, folder, hingga source code.
- Beberapa contoh *version control* terutama git yaitu Github, Gitlab, dan Bitbucket.

Beberapa contoh command line pada git melalui terminal:
- *<strong>git config</strong>*: mengkonfigurasi git
- *<strong>git status</strong>*: menampilkan adanya perubahan baru pada git
- *<strong>git branch -b [nama branch]</strong>*: membuat branch baru
- *<strong>git checkout</strong>*: masuk atau berpindah ke suatu branch
- *<strong>git merge</strong>*: menggabungkan branch cabang ke branch master
  - ```git merge origin/"namaBranch"```

Urutan umum untuk *push* ke suatu repository baru:

- *<strong>git init</strong>*: membuat repository
- *<strong>git add. </strong>*: untuk menambah file baru/file yang telah diubah pada Git
- *<strong>git commit -m "commit message"</strong>*: menyimpan perubahan pada Git
- *<strong>git remote add origin "link repository.git"</strong>*: menghubungkan remote repository dengan local project
- *<strong>git push -u origin master</strong>*: mengirimkan/perubahan file ke remote repository 

### HTML
- HTML atau *Hypertext Markup Language* berfungsi untuk membuat kerangka sebuah website dan menampilkan konten di browser.
- Tools yang dibutuhkan untuk untuk membuat HTML secara dasar yaitu web browser dan code editor.
- HTML Element terdiri atas opening tag, content, dan closing tag.
  ```
  Opening Tag : <p>, <head>, <div>
  Content     : Hello World
  Closing Tag : </p>, </head>, </div>
  ```
- Ada dua macam HTML tag, yaitu:
  
  - Single Tag<br/>
    ``<br/>``  <br/>
    `` <hr/> `` <br/>
    `` <img src= " " alt= " "/>``

  - Paired Tag<br/>
    ``<div> ... </div>``

- Struktur dasar pada HTML:
  ``` 
  <!DOCTYPE html>
  <html>

    <head>
      <title>Page Title</title>
    </head>

    <body>
      <h1>My First Heading</h1>
      <p>My first paragraph.</p>
    </body>

  </html>
  ```

- HTML Attributes : properties dari sebuah element HTML. Contohnya yaitu id, class, name.
  ```
  <p id="hello" class="flex" name="greet"> Hello World! </p>
  ```
- HTML Comment `` <!--  --> ``, sering digunakan untuk memberi keterangan pada suatu line code atau untuk menonaktifkan baris code.
  ``` 
    <!-- <p> Hello World </p> -->
  ```
- HTML Table:
  ``` 
  <table>
      <thead>
          <tr>
              <td>Nama</td>
              <td>NRP</td>
              <td>Jurusan</td>
          </tr>
      </thead>
      <tbody>
          <tr>
              <td>Faiq</td>
              <td>2110191027</td>
              <td>Teknik Informatika</td>
          </tr>
      </tbody>
  </table>
  ```
- Semantic HTML yaitu elemen HTML yang digunakan sesuai dengan fungsi sebenarnya. Contoh yaitu:
  - tag header digunakan untuk header
  - tag footer digunakan untuk footer
  - tag nav digunakan untuk navbar
  - tag section digunakan untuk section

### CSS

- CSS atau *Cascading Style Sheets* digunakan untuk mendesain halaman website dengan peran mengubah warna, customisasi font, editing text format, hingga mengatur tata letak.
- Struktur CSS
  ```
  .namaElement{  
    property: value 
  } 
  ```
  - . (titik) diawal nama elemen merupakan selector yg menuju pada tag html yg memiliki properti kelas. Selector bisa menggunakan *#* untuk attribut *id*.
- Ada 3 cara menggunakan CSS yaitu: 
  - *<strong>Inline</strong>*: css ditempatkan di atribute element HTML.
  - *<strong>Internal</strong>*: css ditempatkan tag style di bagian tag *head*.
  - *<strong>External</strong>*: css ditempatkan dalam file terpisah dengan format *<strong>file.css</strong>*.
- Sifat CSS berdasarkan selector:
  
  - Global<br/>
    Global berarti seluruh element tersebut akan terdampak CSS.
    ``` 
    h1 {
        color: blue; 
    }
    ```
    Berdasarkan code css diatas, seluruh tag h1 akan terdampak *color: blue*
  - Class Only<br/>
    Class Only atau element tertentu berarti hanya element tersebut saja yang akan terdampak CSS.
    ``` 
    .namaLengkap{
      color: red;
    }
    ```
    Berdasarkan code css diatas, hanya class bernama *namaLengkap* saja yang akan terdampak *color: red*
- *<strong>!important</strong>* pada CSS artinya styling CSS yang memiliki tingkat paling atas dan akan diprioritaskan lebih dulu.

### Flexbox

Flexbox adalah suatu cara untuk mengatur layout atau tata letak secara box per box.

- Beberapa contoh flex adalah sebagai berikut:
  - *<strong>Flex direction*</strong>: mengatur letak child
  - *<strong>Flex wrap*</strong>: tata letak akan berpindah kebawah (*wrapping*) jika melebihi lebar maksimum element.
  - *<strong>Flex flow*</strong>: yaitu digunakan sebagai shortcut untuk set up flex-direction dan flex-wrap secara bersamaan
  - *<strong>Order*</strong>: digunakan untuk ordering item yang ingin diatur posisinya
  - *<strong>Justify content*</strong>: mengatur tata letak antar item child secara horizontal.
    Beberapa contoh value untuk justify yang sering digunakan:
      - *<strong>flex-start*</strong> : Child akan berposisi di awal container.	
      - *<strong>flex-end*</strong> : Child akan berposisi di akhir container.
      - *<strong>center*</strong> : Child akan berposisi di tengah container.
      - *<strong>space-between*</strong> : Child akan memiliki space diantara mereka.
      - *<strong>space-around*</strong> : Child akan memiliki space pada di awal, diantara, dan di akhir container.
      - *<strong>space-evenly*</strong> : Child akan memiliki space yang seukuran diantara mereka.
  - *<strong>Align items*</strong> : mengatur tata letak antar item child secara vertikal
    Beberapa contoh value untuk align yang sering digunakan:
      - *<strong>center*</strong> : Items akan diposisikan di tengah container.
      - *<strong>flex-start*</strong> : Items akan diposisikan di awal container.
      - *<strong>flex-end*</strong> : Items akan diposisikan di akhir container.
      - *<strong>stretch*</strong> : Items akan di-stretchkan seukuran container.
  - *<strong>Flex-grow*</strong>: mengatur size suatu item child pada flexbox
  - *<strong>Flex-shrink*</strong>: memperkecil size suatu item child secara relatif terhadap item child lainnya


### Algoritma
- Algoritma adalah metode atau langkah yang direncanakan secara tersusun dan berurutan untuk menyelesaikan atau memecahkan permasalahan dengan sebuah intruksi atau kegiatan
- Kualitas suatu algoritma dapat dilihat dari:
  - Input & output yang jelas dan didefinisikan terlebih dahulu dengan tepat.
  - Setiap step harus benar -benar clear dan tidak bermakna banyak.
  - Algoritma tidak boleh mengandung suatu bahasa pemrograman tertentu.
- Contoh Algoritma biasa ditemukan dalam *Flowchart*.

### Pseudocode
- Pseudocode merupakan sarana yang digunakan untuk menulis algoritma dengan bahasa yang mudah dipahami (bukan bahasa pemrograman).
- Aturan menulis Pseudocode:
  - Huruf kapital digunakan untuk menulis perintah
  - 1 statement hanya terdiri dari 1 baris
  - Menggunakan indentasi
  - Harus bersifat spesifik dan simple

- Contoh Pseudoce
  -  Menentukan_Keliling_Persegi
      ```
      Deklarasi
        sisi, keliling

      Implementasi
        Read(sisi);
        Keliling ← sisi * 4;
        Write(keliling);
      ```
- Beberapa jenis Pseudocode:
  - *<strong>Procedural*</strong> : alur berpikir berurutan
  - *<strong>Conditional*</strong> : alur berpikir dengan suatu percabangan masalah (if else)
  - *<strong>Looping*</strong> : perintah yang diulang
  - *<strong>Recursive*</strong> : sebuah perintah yang memanggil function di dalam sebuah function (*rekursi*).

### Looping Javascript

- Looping *<strong>For*</strong>
  - Digunakan saat tahu jumlah perulangan dan kapan harus berhenti.
    - Code
      ```
      for (let i = 0; i < 4; i++) {
        console.log('Hello World');
      }
      ```
    - Output
      ```
      Hello World
      Hello World
      Hello World
      Hello World
      ```

- Looping *<strong>While*</strong>
  - Digunakan saat tidak tahu jumlah perulangan tetapi tahu kapan harus berhenti.
    - Code
      ```
      let i = 0
      while (i < 2) {
        console.log('Hello World');
        i++;
      }
      ```
    - Output
      ```
      Hello World
      Hello World
      ```

### Conditional Javascript

- Ada dua macam kondisi dalam Javascript yang sering dipakai:
  - If Else
    ```
    let nama = 'Faiq'

    if (nama == 'Faiq') {
      console.log('Halo Faiq')
    } else {
      console.log('Siapa kamu')
    }
    ```
  - Ternary Operator
    ```
    const nama = 'Faiq';
    const isFaiq = nama == 'Faiq ? "Benar Faiq" : "Bukan Faiq";
    console.log(isFaiq); // "Benar Faiq"
    ```

### Console in Javascript

- Console digunakan untuk menampilkan output dalam console. Biasa digunakan untuk mengecek nilai suatu variabel.
  
- Code
  ```
  let nama = Faiq
  console.log(nama);
  console.log('namaku ', nama);
  ```
- Output dalam <strong>console</strong>
  ```
  Bimo
  nama saya Faiq
  ```