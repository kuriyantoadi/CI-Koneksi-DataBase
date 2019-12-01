# CodeIgniter-Koneksi
Menghubungkan CI dengan Database

**1. Extrak Framework CI**

**2. Import database ci-koneksi.sql**

**3. application/config/autoload.php**
  <br>Awal Baris 92 :
  <br>`$autoload['helper'] = array('');`
  <br>Edit :
  <br>`$autoload['helper'] = array('url');`

  <br>Awal Baris 61 :
  <br>`  $autoload['libraries'] = array('');`
  <br>Edit :
  <br>`  $autoload['libraries'] = array('database');`


**4. application/config/database.php ubah baris 78-81**
  <br>`'hostname' => 'localhost',`
  <br>`'username' => 'root',`
  <br>`'password' => '',`
  <br>`'database' => 'ci-koneksi',`

  **5. Tambahkan beberapa file berikut**
  - application/controllers/Belajar.php
  - application/view/v_user.php
  - application/models/M_data.php


  **6. Buka dengan Link berikut**
  <br>`localhost/ci-koneksi/index.php/belajar/user`
