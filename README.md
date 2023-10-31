# **Lab 5 Web**

```
Nama    : Dimas adi nugraha
NIM     : 312210409
Kelas   : TI.22.A4
```

## **Instruksi Praktikum**

1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama lab5_javascript.
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## **Langkah-langkah Praktikum**

1. membuat dokumen HTML dengan nama file lab5_javascript.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Mengenal JavaScript</title>
  </head>
  <body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
      document.write("Hello World");
      console.log("Hello World");
    </script>
  </body>
</html>
```

2. Pemakaian Alert sebagai property window.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>alert box</title>
  </head>
  <body>
    <script language="JavaScript">
      <!--
      window.alert("ini merupakan pesan untuk anda");
      //-->
    </script>
  </body>
</html>
```

3. Pemakaian method dalam objek

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>skrip javascript</title>
  </head>
  <body>
    percobaan memakai javascript:<br />
    <script language="javascript">
      <!--
      document.write("selamat mecoba javascript<br>");
      document.write("semoga sukses!");
      //-->
    </script>
  </body>
</html>
```

4. Pemakaian Prompt

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>pemasukan data</title>
  </head>
  <body>
    <script language="javascript">
      <!--
      var nama = prompt("siapa nama anda?", "masukan nama anda");
      document.write("hai, " + nama);
      //-->
    </script>
  </body>
</html>
```

5. Pembuatan fungsi dan cara pemanggilannya

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Contoh program javascript</title>
    <script language="javascript">
      function pesan() {
        alert("memanggil javascript lewat body onload");
      }
    </script>
  </head>
  <body onload="pesan()"></body>
</html>
```

6. Operasi dasar aritmatika

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Contoh program javascript</title>
    <script language="javascript">
      function test(val1, val2) {
        document.write("<br>" + "perkalian : val1*val2 " + "<br>");
        document.write(val1 * val2);
        document.write("<br>" + "pembagian : val1/val2 " + "<br>");
        document.write(val1 / val2);
        document.write("<br>" + "pengurangan : val1-val2 " + "<br>");
        document.write(val1 - val2);
        document.write("<br>" + "modulus : val1%val2 " + "<br>");
        document.write(val1 % val2);
      }
    </script>
  </head>
  <body>
    <input
      type="button"
      name="button1"
      value="arithmetic"
      onclick="test(9,4)"
    />
  </body>
</html>
```

7. Seleksi kondisi (if..else)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>contoh if-else</title>
  </head>
  <body>
    <script language="javascript">
      <!--
      var nilai = prompt("nilai (0-100): ", 0);
      var hasil = " ";
      if (nilai >= 60) hasil = "lulus";
      else hasil = "tidak lulus";
      document.write("hasil: " + hasil);
      //-->
    </script>
  </body>
</html>
```

8. Penggunaan operator switch untuk seleksi kondisi

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>contoh program javascript</title>
    <script language="javascript">
      function test() {
        val1 = window.prompt("input nilai (1-5):");
        switch (val1) {
          case "1":
            document.write("bilangan satu");
            break;
          case "2":
            document.write("bilangan dua");
            break;
          case "3":
            document.write("bilangan tiga");
            break;
          case "4":
            document.write("bilangan empat");
            break;
          case "5":
            document.write("bilangan lima");
            break;
          default:
            document.write("bilangan lainnya");
        }
      }
    </script>
  </head>
  <body>
    <input type="button" name="button1" value="switch" onclick="test()" />
  </body>
</html>
```

9. Form Input

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>contoh program javascript</title>
    <script language="javascript">
      function test() {
        var val1 = document.kirim.T1.value;
        if (val1 % 2 == 0) document.kirim.T2.value = "bilangan genap";
        else document.kirim.T2.value = "bilangan ganjil";
      }
    </script>
  </head>
  <body>
    <form method="POST" name="kirim">
      <p>
        BIL <input type="text" name="T1" size="20" /> MERUPAKAN BIL
        <input type="text" name="T2" size="20" />
      </p>
      <p><input type="button" value="TEBAK" name="B1" onclick="test()" /></p>
    </form>
  </body>
</html>
```

10. Form Button

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Object document</title>
  </head>
  <body>
    <script language="javascript">
      <!--
      function ubahWarnaLB(warna) {
        document.bgColor = warna;
      }
      function ubahWarnaLD(warna) {
        document.fgColor = warna;
      }
      //-->
    </script>
    <h1>tes</h1>
    <form>
      <input
        type="button"
        value="Latar Belakang Hijau"
        onclick="ubahWarnaLB('GREEN')"
      />
      <input
        type="button"
        value="Latar Belakang Putih"
        onclick="ubahWarnaLB('WHITE')"
      />
      <input
        type="button"
        value="Teks Kuning"
        onclick="ubahWarnaLD('YELLOW')"
      />
      <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')" />
    </form>
    <script language="javascript">
      <!--
      document.write("Dimodifikasi terakhir pada " + document.lastModified);
      //-->
    </script>
  </body>
</html>
```

11. HTML DOM (Pilihan menggunakan checkBox dengan perhitungan otomatis)

```html
<!DOCTYPE html>
<!--
    File: daftar_menu.html
//-->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;

            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }

            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);"/> Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);"/> Tempe Goreng Rp. 500</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);"/> Telur Dadar Rp. 2.500</label><hr />
    <strong>Total Bayar: Rp. <input id="total" type="text" /></strong>
</body>
</html>
```

# [SCREENSHOT](https://github.com/dimasadinugrahaaa634/LAB5WEB/tree/7c3689a4d062401eee41f542a5513c736f143847/img)

## **Tugas**

![img](img/TUGAS.png)

# [OUTPUT](https://github.com/NurAkbarr/Lab5Web/blob/bfc35c39bf434c0fc182f812d2b21b82283a15e7/img/tugas.1.png,)