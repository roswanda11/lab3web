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

![image](https://github.com/roswanda11/lab3web/assets/115516632/9caf8e95-de58-4e3e-8b8b-7accf76b1bf0)

### 4. Melakukan validasi dokumen html dengan mengakses http://validator.w3.org

![Screenshot (398)](https://github.com/roswanda11/lab3web/assets/115516632/19200869-61ed-42b1-a40c-648ed914b30b)

- Maka hasilnya sebagai berikut :

![image](https://github.com/roswanda11/lab3web/assets/115516632/22e0d1a5-f130-457d-aedd-e3a142d53587)


# Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.

        <!DOCTYPE html>
        <html lang="en">
            <head>
                <meta charset="UTF-8"/>
                <meta name="viewport" content="width=device-widht, initial-scale=1"/>
                <title>Formulir Pendaftaran HIMATIF-2024</title>
                <body>
                    <form action="proses.php" method="post" class="form">
                        <fieldset>
                            <legend>FORMULIR PENDAFTARAN HIMATIF UPB - 2024</legend>
                            <h2> A. Identitas</h2>
                            <p>
                                <label for="nama">Nama Lengkap :</label>
                                <input
                                type="text"
                                id="nama"
                                name="nama"
                                required
                                placeholder="Masukkan Nama Lengkap Anda"/>
                            </p>
                            <p>
                                <label for="nama">Nama Panggilan :</label>
                                <input
                                type="text"
                                id="nama"
                                name="nama"
                                required
                                placeholder="Masukkan Nama Panggilan Anda"/> 
                            </p>
                            <p>
                                <label for="nim">NIM :</label>
                                <input
                                type="text"
                                id="nim"
                                name="nim"
                                required
                                placeholder="Masukkan NIM Anda"/>
                            </p>
                            <p>
                                <label for="pilihan">Jenis Kelamin :</label>
                                <select id="pilihan" name="pilihan">
                                    <option value="opsi1">Pilih</option>
                                    <option value="opsi2">Laki-Laki</option>
                                    <option value="opsi3">Perempuan</option>
                                </select>
                            </p>
                            <p>
                                <label for="tempat_lahir">Tempat Lahir :</label>
                                <input type="text" id="tempat_lahir" name="tempat_lahir"required
                                placeholder="Masukkan Tempat Lahir Anda"/>
                            </p>
                            <p>
                                <label for="tanggal_lahir">Tanggal Lahir :</label>
                                <input type="date" id="tanggal_lahir" name="tanggal_lahir"required/>
                            </p>
                            <p>
                                <label for="multiple">Tahun Angkatan :</label>
                                <select id="multiple" name="multiple[]">
                                    <option value="item1">2021</option>
                                    <option value="item2">2022</option>
                                    <option value="item3">2023</option>
                                    <option value="item4">2024</option>
                                </select>
                            </p>
                            <p>
                                <label for="Alamat">Alamat :</label>
                                <textarea
                                id="alamat"
                                name="alamat"
                                rows="3"
                                required
                                placeholder="Masukkan Alamat Anda"
                                ></textarea>
                            </p>
                            <p>
                                <label for="email">Email :</label>
                                <input
                                type="text"
                                id="email"
                                name="email"
                                required
                                placeholder="Masukkan Email Anda"/>
                            </p>
                            <p>
                                <label for="no_hp">No HP (WhatsApp) :</label>
                                <input
                                type="text"
                                id="no_hp"
                                name="no_hp"
                                required
                                placeholder="Masukkan No WA Anda"/>
                            </p>
                            <h2>B. Motto Hidup</h2>
                            <p>
                                <textarea
                                id="motto_hidup"
                                name="motto_hidup
                                rows="3"
                                required
                                placeholder="Masukkan Motto Hidup Anda"
                                ></textarea>
                            </p>
                            <p>
                                <input type="submit" value="Kirim"/>
                            </p>
                        </fieldset>
                    </form>
                    <style>
                        body{
                         font-family: Arial, sans-serif;
                         background-color: #f5e898;
                         margin: 0;
                         padding: 0;
                        }
             
                         fieldset{
                         border: 2px solid #d1a93e;
                         border-radius: 10px;
                         background-color: #fff;
                         padding: 50px;
                         margin: 20px auto;
                         max-width: 800px;
                        }
             
                        .form{
                         display: flex;
                         flex-direction: column;
                        }
             
                        .form legend{
                         font-weight: bold;
                         font-size: 1.5rem;
                         text-align: center;
                         color: #8c6600;
                        }
             
                        .form h2{
                         margin-top: 20px;
                         font-size: 1.2rem;
                         color: #d1a93e;
                        }
             
                        .form p{
                         margin: 15px 0;
                        }
             
                        label{
                         font-weight: bold;
                         color: #333;
                        }
             
                        input[type="text"],
                        input[type="date"],
                        select,
                        textarea{
                         width: 100%;
                         padding: 10px;
                         margin: 5px 0;
                         border: 1px solid #acc;
                         border-radius: 5px;
                         font-size: 1rem;
                        }
             
                        select[multiple]{
                         height: 100px;
                        }        
             
                        textarea{
                         height: 100px;
                        }
             
                        input[type="submit"]{
                         width: auto;
                         background-color: #d1a93e;
                         color:#fff;
                         border: none;
                         border-radius: 5px;
                         padding: 10px 20px;
                         cursor: pointer;
                         font-size: 1rem;
                        }
                     </style>
                </body>
            </head>
        </html>

- Lakukan Refresh kembali pada web Browser, dan lihat perubahannya:
      
![image](https://github.com/roswanda11/lab3web/assets/115516632/00b947e3-7f78-41b3-91c6-971f130e6ef5)

