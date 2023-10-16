# Praktikum 3 web: Membuat List, Table dan Form

## Langkah-langkah Praktikum
-Persiapan membuat dokumen HTML dengan nama file lab3_list.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```

![prak3_html1](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/1b223529-d7c1-4634-b92e-2919a5d71f88)


### Membuat Ordered List
- Kemudian tambahkan kode untuk membuat Ordered List seperti berikut.
```
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
      <li>Pemrograman Web</li>
      <li>Sistem Informasi</li>
      <li>Basis Data 2</li>
    </ol>
</section>
```
![prak3_html2](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/5cf1dfab-5dbe-424b-b068-a47e8ea5a368)
### Membuat Unorderd List
- Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada section unordered-list, seperti berikut.
```
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
      <li>Jaringan Komputer</li>
      <li>Struktur Data</li>
      <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```
![prak3_html3](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/1cc2d4ce-a090-421e-b1fd-0ae3cbbb068a)
### Membuat Description List
- Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.
```
<section id="unorder-list">
        <h2>Description List</h2>
        <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Industi</dd>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Lingkungan</dd>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akuntasi</dd>
            <dd>Manajemen</dd>
            <dd>BisnIS Digital</dd>
        </dl>
    </section>
```
![prak3_html4](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/66d28fc5-0f94-4b48-8207-d9d993e2eeed)
### Membuat Tabel
- Buat file baru dengan nama lab3_tabel.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML lanjutan</title>
</head>
<body>
  <header>
    <h1>Membuat table</h1>
  </header>
</body>
</html>
```
- Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:
```
<table border="1" cellpadding="4" cellspacing="3">
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
```
![prak3_html5](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/aa692921-0509-4eec-b9ee-73963c092fae)
### Mengatur Margin dan Padding
- Untuk mengatur margin dan padding pada cel data, tambahkan atribut cellpadding dan cellspacing pada tag table.

```
<table border="1" cellpadding="4" cellspacing="0">
```
![prak3_html6](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/d77872f5-01c5-4c1d-8473-133d08989d70)
### Menggabungkan Sel Data
- Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara horizontal).
```
<table border="1" cellpadding="6" cellspacing="0">
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
```
![prak3_html7](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/c314e838-074f-4fba-a7ee-4a9abed187c7)
### Membuat Form
- Buat file baru dengan nama lab3_form.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>Membuat From</header>
</body>
</html>
```
- Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut.

```
form action="proses.php" method="post">
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
```
![prak3_html8](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/38d7c86c-f631-4e3b-855e-ab00b8f318de)
### Menabahkan Style pada Form
- Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.
```
 <style>
        form p > label {
            display: inline-block;
            width: 100px;
        }
        form input[type="text"], form textarea {
            border: 1px solid #197a43;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
```
![prak3_html9](https://github.com/mullf/Lab3_HTML_ProgWeb/assets/115521049/af4d6240-1e06-4b86-956c-914f1a859f23)
### Pertanyaan dan Tugas
- Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.
