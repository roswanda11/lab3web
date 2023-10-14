<table>
  <tr>
    <th colspan="2">DATA MAHASISWA</th>
  </tr>
  <tr>
    <td>Nama</td>
    <td>Roswanda Nuraini</td>
  </tr>
  <tr>
    <td>NIM</td>
    <td>312210328</td>
  </tr>
  <tr>
    <td>Kelas</td>
    <td>TI.22.A3</td>
  </tr>
</table>

# <p align="center">Praktikum3 : Membuat List, Table dan Form</p>

# 1. Membuat Dokumen List

### Langkah-langkah praktikum
- Persiapkan membuat dokumen HTML dengan nama file <b>lab3_list.html</b> seperti berikut:

      <!DOCTYPE html>
      <html lang="en">
          <head>
              <meta charset="UTF-8">
              <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
              <title>HTML Lanjutan</title>
          </head>
          <body>
              <header>
                  <h1>Jadwal Perkuliahan</h1>
              </header>
          </body>
      </html>

- Kemudian jalankan Web Browser dengan mengklik Menu Terminal pada pojok atas pada VS CODE. lihat perubahannya.

![Screenshot (369)](https://github.com/roswanda11/lab3web/assets/115516632/1b062532-79fb-4c5e-bfa4-c39a507a5401)

### Membuat Ordered List

- Kemudian tambahkan kode untuk membuat Ordered List seperti berikut: 

      <section id="order-list">
          <h2>Mata Kuliah Semester 3</h2>
          <ol>
              <li>Pemrograman Web</li>
              <li>Rekayasa Perangkat Lunak</li>
              <li>Jaringan Komputer</li>
              <li>Pemrograman Mobile</li>
          </ol>
      </section>

Order List adalah list yang tersusun secara urut dalam tag nya terdapat ```tag OL dan LI```

- Kemudian lakukan refresh pada web browser, dan lihat perubahannya:

![Screenshot (371)](https://github.com/roswanda11/lab3web/assets/115516632/2dbd8e87-1261-4d3e-8079-5cce5bb4f029)

### Membuat Unordered List

- Kemudian tambahkan kode untuk membuat <i>Unordered List</i>, setelah deklarasi ordered list pada section <b>unordered-list</b>, seperti berikut.

      <section id="unorder-list">
          <h2>Mata Kuliah Tambahan</h2>
          <ul type="square">
              <li>Kalkulus</li>
              <li>Struktur Data</li>
              <li>Algoritma & Pemrograman</li>
              <li>Probabilitas dan Statistika</li>
          </ul>
      </section>

Unordered List adalah list yang tidak terurut atau acak dengan awalan ```tag UL dan LI```

  - Lakukan refresh, dan lihat perubahannya:
 
![Screenshot (372)](https://github.com/roswanda11/lab3web/assets/115516632/f625393f-b9f8-4976-977b-8ad0372845c4)

### Membuat Description List

- Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.

      <section id="unorder-list">
          <h2>Program Studi</h2>
          <dl>
              <dt>Fakultas Teknik</dt>
              <dd>Teknik Industri</dd>
              <dd>Teknik Informatika</dd>
              <dd>Teknik Lingkungan</dd>
              <dt>Fakultas Ekonomi dan Bisnis</dt>
              <dd>Akuntansi</dd>
              <dd>Manajemen</dd>
              <dd>Bisnis Digital</dd>
          </dl>
      </section>

Description list yaitu dengan di awali ```tag DL sebagai pemuat konten``` kemudian ```DT sebagai konten istilah``` dan ```DD sebagai penjelas konten istilah``` tersebut

- Refresh Kembali Web Browser, dan lihat perubahannya: 

![image](https://github.com/roswanda11/lab3web/assets/115516632/fa542ace-1a0b-4e7c-a178-71861e56da0a)

# 2. Membuat Tabel Sederhana

- Buat file baru dengan nama <b>lab3_tabel.html</b> seperti berikut.

      <!DOCTYPE html>
      <html lang="en">
          <head>
              <meta charset="UTF-8">
              <met aname="viewport" content="width=device-width, initial-scale=1.0">
              <title>HTML Lanjutan</title>
          </head>
          <body>
              <header>
                  <h1>Membuat Table</h1>
              </header>
          </body>
      </html lang>

- Kemudian tambahkan kode untuk membuat tabel sederhana seperti berikut ini:
  
      <table border="1" cellpadding="4" cellspacing="0">
          <thead>
              <tr>
                  <th>No.</th>
                  <th>Fakultas</th>
                  <th>Program Studi</th>
              </tr>
          </thead>
          <tbody>
              <tr>
                  <td>1.</td>
                  <td>Teknik</td>
                  <td>Teknik Informatika</td>
              </tr>
              <tr>
                  <td>2.</td>
                  <td>Teknik</td>
                  <td>Teknik Industri</td>
              </tr>
              <tr>
                  <td>3.</td>
                  <td>Teknik</td>
                  <td>Teknik Lingkungan</td>
              </tr>
          </tbody>
          </table>

Dalam membuat table di perlukan tag table dan kemudian ```thead yang di dalamnya ada TR dan TH``` untuk table head dan kemudian ```tbody yang di dalamnya ada TR dan TD```

- Lalu refresh kembali web browser, dan amati lagi perubahannya:

![Screenshot (377)](https://github.com/roswanda11/lab3web/assets/115516632/c67f428d-e0c5-4b51-b58e-d44414fde82f)

### Mengatur Margin dan Padding

- Untuk mengatur margin dan padding pada cel data, tambahkan atribut <i>cellpadding</i> dan <i>cellspacing</i> pada tag table.

      <table border="1" cellpadding="10" cellspacing="2">

![image](https://github.com/roswanda11/lab3web/assets/115516632/36417a55-6f8e-49e0-8156-4fb214335316)

- Sebelumnya Cellpadding 4 Cellspadding 0 yang saya ubah menjadi Cellpadding 10 dan Cellspadding 2 contoh gambar di atas adalah hasilnya

### Menggabungkan Sel Data

- Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut ```rowspan``` untuk menggabungkan baris (secara vertikal) dan ```colspan``` untuk menggabungkan kolom (secara horizontal).

       <table border="1" cellpadding="10" cellspacing="2">
              <thead>
                  <tr>
                      <th>No.</th>
                      <th>Fakultas</th>
                      <th>Program Studi</th>
                  </tr>
              </thead>
              <tbody>
                  <tr>
                      <td>1.</td>
                      <td rowspan="3">Teknik</td>
                      <td>Teknik Informatika</td>
                  </tr>
                  <tr>
                      <td>2.</td>
                      <td>Teknik Industri</td>
                  </tr>
                  <tr>
                      <td>3.</td>
                      <td>Teknik Lingkungan</td>
                  </tr>
              </tbody>
          </table>

- Lakukan Refresh kembali pada web Browser, dan lihat perubahannya: 

![image](https://github.com/roswanda11/lab3web/assets/115516632/e0df028c-cead-4aab-9620-11b226b27d54)

# 3. Membuat Tabel Form

- Buat file baru dengan nama <b>lab3_form.html</b> seperti berikut.

      <!DOCTYPE html>
      <html lang="en">
      <head>
          <meta charset="UTF-8">
          <meta name="viewport" content="width=device-width, initial-scale=1.0">
          <title>HTML Lanjutan</title>
      </head>
      <body>
          <header>
              <h1>Membuat Form</h1>
          </header>
      </body>
      </html>

- Kemudian tambahkan kode untuk membuat tabel sederhana seperti berikut:

      <form action="proses.php" method="post">
              <fieldset>
                  <legend>Data Pelanggan</legend>
                  <p>
                      <label for="nama">Nama</label>
                      <input type="text" id="nama" name="nama">
                  </p>
                  <p>
                      <label for="alamat">Alamat</label>
                      <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
                  </p>
                  <p>
                      <label>Jenis Kelamin</label>
                      <input id="jk_l" type="radio" name="kelamin" value="L" /><label
          for="jk_l">Laki-laki</label>
                      <input id="jk_p" type="radio" name="kelamin" value="P" /><label
          for="jk_p">Perempuan</label>
                  </p>
                  <p><input type="submit" value="Login"></p>
              </fieldset>
      </form>

Dalam membuat form di perlukan tag form yang kemudian yang di tambahkan fieldset yang kemudian di tambahkan tag input sesuai kebutuhan codingan

- Amati perubahannya pada web browser anda:

![Screenshot (381)](https://github.com/roswanda11/lab3web/assets/115516632/a7f53257-489c-426f-854e-c0501c61306e)

### Menambahkan Style pada Form

- Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.

      <style>
          form p > label {
              display: inline-block;
              width: 100px;
          }
          form input[type="text"], form textarea {
              border: 1px solid #ff3794;
          }
          form input[type="submit"] {
              border: 1px solid darkred;
              background-color: pink;
              color: darkred;
              font-weight: bold;
              padding: 5px 15px;
          }
          
          legend {
              font: 50px bold;
              color:darkcyan;
              font-weight: bold;
              padding: 5px 15px;
          }
      </style>

- Lakukan Refresh pada Web Browser, dan Simaklah perubahan yang terjadi setelahnya:

![image](https://github.com/roswanda11/lab3web/assets/115516632/46fdbbe1-52b5-4b46-b78d-fe59bb7552f9)

# Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.

        <!DOCTYPE html>
        <html>
            <head>
                <meta name="viewport" content="width=device-widht, initial-scale=1">
                <style>
                    .dropbtn {
                        background-color: rgb(58, 241, 226);
                        color: rgb(10, 3, 3);
                        padding: 16px;
                        font-size: 16px;
                        border: none;
                        cursor: pointer;
                    }
                    .dropbtn:hover, .dopbtn:focus { 
                        background-color: rgb(241, 134, 255); 
                    }
                    .dropdown {
                        position: relative;
                        display: inline-block;
                    }
                    .dropdown-content {
                        display: none;
                        position: absolute;
                        min-width: 160px;
                        background-color: rgb(255, 34, 170);
                        box-shadow: 0px 8px 16px 0px rgba(23, 189, 201, 8.2);
                        overflow: auto;
                    }
                    .dropdown-content a {
                        color: rgb(1, 2, 0);
                        padding: 12px 16px;
                        text-decoration: none;
                        display: block;
                    }
                    .dropdown a:hover {background-color: rgb(151, 149, 248);}
                    .show {display: block;}
                </style>
            </head>
            <body>
                <h1>Membuat Dropdown</h1>
                <p>Silahkan klik menu untuk memilih.</p>
                <div class="dropdown">
                    <button onclick="myFunction()" class="dropbtn">Menu</button>
                    <div id="myDropdown" class="dropdown-content">
                    <a href="lab3_list.html">Membuat List</a>
                    <a href="lab3_tabel.html">Membuat Tabel</a>
                    <a href="lab3_form.html">Membuat Form</a>
                </div>
            </div>
                <script>
                /* When the user clicks on the button,
                toggle between hiding and showing the dropdown content */
                function myFunction() {
                    document.getElementById("myDropdown").classList.toggle("show");
                }
                // Close the dropdown if the user clicks outside of it
                widow.onclick = function(event) {
                    if (!event.target.matches('.dropbtn')) {
                        var dropdowns = document.getElementsByClassName("dropdown-content");
                        var i;
                        for (i=0; i < dropdowns.length; i++) { 
                            var openDropdown = dropdowns[i];
                            if (openDropdown.classList.contains('show')) { 
                                openDropdown.classList.remove('show');
                            }
                            }
                        }
                    }
                </script>
                <hr>
                <form>
                    <h2>Membuat Listbox</h2>
                    <p>Daftar Menu Food Court Hollywood :</p>
                    <select name="menu" size="4">
                        <option value="1">Ayam Geprek</option>
                        <option value="1">Spaghetti</option>
                        <option value="1">Sushi</option>
                        <option value="1">Seblak</option>
                        <option value="1">Bakso Mozarella</option>
                    </select>
                    <p><input type="submit" value="submit" /></p>
                </form> 
            </body>
        </html>           

- Lakukan Refresh kembali pada web Browser, dan lihat perubahannya:
      
![image](https://github.com/roswanda11/lab3web/assets/115516632/e15706a6-ea43-410f-abb6-11d8e5b44da2)
