# Web5Lab5

**Nama    : Aning Kinanti** <br>
**NIM     : 312010364** <br>
**Kelas   : TI.20.A2** <br>
**Matkul  : Pemrograman Web** <br>

# Belajar Javascript

## A. Pengenalan Javascript
### 1. Membuat File HTML
Buatlah dokumen HTML dengan nama lab5_javascript.html seperti contoh dibawah ini : <br>
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>MENGENAL JAVASCRIPT</title>
    </head>
    <body>
        <h1>Pengenalan JavaScript</h1>
        <h3>Contoh document.write dan console.log</h3>
        <script>
            document.write("Hello Sunshine !");
            console.log("Hello World !");
        </script>
    </body>
    </html>
```
<br>


Ini adalah hasil dari sintaks diatas :
![Gambar 1](screenshot/ss1.PNG) <br>

## B. Javascript Dasar
### 1. Membuat Alert
Membuat alert sebagai property window menggunakan `window.alert()` seperti contoh dibawah ini : <br>
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>ALERT BOX</title>
    </head>
    <body>
        <script language = "Javascript">
            window.alert ("Ini pesan untuk anda");
        </script>
    </body>
    </html>
```
<br>


Ini adalah hasil dari sintaks diatas :
![Gambar 2](screenshot/ss2.PNG) <br>

### 2. Penggunaan Method
Cara penggunaan method dalam objek menggunakan `document.write()` seperti contoh dibawah ini : <br>
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>SKRIP JAVASCRIPT</title>
    </head>
    <body>
        percobaan memakai javascript : <br>
        <script language = "javascript" type="text/javascript">
            document.write("Selamat Belajar Javascript");
            document.write("<br>");
            document.write("GoodLuck !");
        </script>
    </body>
    </html>
```
<br>


Ini adalah hasil dari sintaks diatas :
![Gambar 3](screenshot/ss3.PNG) <br>

### 3. Penggunaan Prompt
Cara penggunaan prompt seperti contoh dibawah ini : <br>
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>PEMASUKAN DATA</title>
    </head>
    <body>
        <script language="javascript">
            var nama = prompt("Siapa nama anda ?", "Masukan nama anda");
            document.write("hai, " + nama);
        </script>
    </body>
    </html>
```
<br>


Ini adalah hasil awal dari sintaks diatas : <br>
![Gambar 4a](screenshot/ss4a.PNG) <br>

Masukan nama contoh seperti dibawah ini : <br>
![Gambar 4b](screenshot/ss4b.PNG) <br>

Lalu klik tombol OK, maka akan menjadi seperti dibawah ini : <br>
![Gambar 4c](screenshot/ss4c.PNG) <br>

### 4. Penggunaan Javascript dengan Body Onload
Cara penggunaan javascript dengan body onload seperti contoh dibawah ini : <br>
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>PENGGUNAAN ONLOAD</title>
        <script language="javascript">
            function pesan(){
                alert ("memanggil javascript lewat body onload")
            }
        </script>
    </head>
    <body>
        <body onload=pesan()>
    </body>
    </html>
```
<br>


Ini adalah hasil dari sintaks diatas : <br>
![Gambar 5](screenshot/ss5.PNG) <br>

## C. Dasar Pemrograman Pada Javascript
### 1. Operasi Dasar Aritmatika
Contoh operasi dasar aritmatika seperti contoh dibawah ini : <br>
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Operasi Dasar Aritmatika</title>
        <script language="javascript">
            function test (val1, val2) {
                document.write("<br>"+"Perkalian : val1*val2"+"<br>")
                document.write(val1*val2)
                document.write("<br>"+"Pembagian : val1/val2"+"<br>")
                document.write(val1/val2)
                document.write("<br>"+"Penjumlahan : val1+val2"+"<br>")
                document.write(val1+val2)
                document.write("<br>"+"Pengurangan : val1-val2"+"<br>")
                document.write(val1-val2)
                document.write("<br>"+"Modulus : val1%val2"+"<br>")
                document.write(val1%val2)
            }
        </script>
    </head>
    <body>
        <input type="button" name="button1" value="arithmetic" onclick=test(12,4)>
    </body>
    </html>
```
<br>


Ini adalah hasil awal dari sintaks diatas :
![Gambar 6a](screenshot/ss6a.PNG) <br>

Apabila button arimatika diklik, maka akan muncul seperti dibawah ini :
![Gambar 6b](screenshot/ss6b.PNG) <br>

### 2. Penggunaan IF-ELSE
Cara penggunaan If-Else seperti contoh dibawah ini : <br>
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>IF-ELSE</title>
    </head>
    <body>
        <script language="javascript">
            var nilai = prompt("nilai (0-100) : ", 0);
            var hasil = "";
            if (nilai >= 60)
            hasil = "lulus !";
            else
            hasil = "tidak lulus";
            document.write("hasil : "+hasil);
        </script>    
    </body>
    </html>
```
<br>


Ini adalah hasil awal dari sintaks diatas : <br>
Misalkan pada kolom input diisi 75 <br>
![Gambar 7a](screenshot/ss7a.PNG) <br>

Maka, akan muncul hasil seperti dibawah ini : <br>
![Gambar 7b](screenshot/ss7b.PNG) <br>

Lalu, dicoba lagi misalkan pada kolom input diisi 55 <br>
![Gambar 7c](screenshot/ss7c.PNG) <br>

Maka, akan muncul hasil seperti dibawah ini : <br>
![Gambar 7d](screenshot/ss7d.PNG) <br>