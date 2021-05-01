# Pemograman Web
~~~
Nama  : Arif Samsudin
NIM   : 311910255
Kelas : TI 19 C1
~~~
# 1.Membuat dokumen HTML
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
~~~
<!DOCTYPE  html>
<html  lang="en">
<head>
<title>Mengenal  JavaScript</title>
</head>
<body>
<h1>Pengenalan  JavaScript</h1>
<h3>Contoh  document.write  dan  console.log</h3>
<script>
document.write("Hello  World"); console.log("Hello  World");
</script>
</body>
</html>
~~~
![1  Persiapan](https://user-images.githubusercontent.com/81839328/116779559-26a90600-aaa1-11eb-9663-3e937167d72b.JPG)
![1  Pengenalan Java Script](https://user-images.githubusercontent.com/81839328/116779561-2872c980-aaa1-11eb-92c9-243dba456a3f.JPG)
# 2. Javascrip Dasar
Pemakaian Alert sebagai property window.
~~~
<!DOCTYPE  html>
<html>
<head>
<title>alert box</title>
</head>
<body>
<script language = "javascript">
<!--
    window.alert("ini merupakan pesan untuk anda");
    //-->
</script>
</body>
</html>
~~~
![2  Javascript dasar alert](https://user-images.githubusercontent.com/81839328/116779582-4a6c4c00-aaa1-11eb-9eaa-22a840eebfdc.JPG)
Pemakaian method dalam objek
~~~
<!DOCTYPE  html>
<html>
<head>
<title>skrip javascript</title>
</head>
<body>
Percobaan Memakai Javascript<br> 
<script language = "javascript">
<!--
    document.write("selamat mencoba javasript<br>");
    document.write("semoga sukses!");
    //-->
</script>
</body>
</html>
~~~
![3  Metod dalam objek](https://user-images.githubusercontent.com/81839328/116779598-7daedb00-aaa1-11eb-9828-83de0f7fe130.JPG)
Pemakaian Prompt
~~~
<!DOCTYPE  html>
<html>
<head>
<title>pemasukan data</title>
</head>
<body>
<script language = "javascript">
<!--
    var nama = prompt("siapa nama anda?","Masukan Nama Anda");
    document.write("hai ", nama);
    //-->
</script>
</body>
</html>
~~~
![4  Pemakaian prompt](https://user-images.githubusercontent.com/81839328/116779617-a3d47b00-aaa1-11eb-8ad7-a1febabda54e.JPG)
Pembuatan fungsi dan cara pemanggilannya
~~~
<!DOCTYPE  html>
<html>
<head>
    <title>Contoh program javascript</title>
    <script language = "javascript">
    function pesan(){alert ("Memanggil javascript lewat body onload")
    }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
~~~
![5  Penggunaan Fungsi](https://user-images.githubusercontent.com/81839328/116779637-b9e23b80-aaa1-11eb-95a3-6a69faa59882.JPG)
# 3. Dasar Pemrograman Di Javascript
Operasi dasar aritmatika
~~~
<html>
<head>
    <title>Contoh program javascript</title>
    <script language = "javascript">
    function test (val1,val2)
    {   
        document.write("<br>"+"perkalian : val1*val2 "+"<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2 "+"<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
        document.write(val1-val2)
        document.write("<br>"+"modulus : val1%val2 "+"<br>")
        document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="aritmatika" onclick=test(9,4)>
</body>
</html>
~~~
![6  Dasar Pemograman](https://user-images.githubusercontent.com/81839328/116779671-de3e1800-aaa1-11eb-8240-6bea058df553.JPG)
Seleksi kondisi (if..else)
~~~
<html>
<head>
    <title>Contoh if-else</title>
</head>
<body>
    <script language = "javascript">
    <!--
    var nilai = prompt("nilai (0-10): ", 0);
    var hasil = "";
    if (nilai >=60)
    hasil = "lulus";
    else
    hasil = "tidak lulus";
    document.write("hasil: " + hasil);
    //-->    
    </script>
</body>
</html>
~~~
![7  Seleksi Kondisi](https://user-images.githubusercontent.com/81839328/116779685-f150e800-aaa1-11eb-8874-a8beb69d737e.JPG)
![7  Hasil](https://user-images.githubusercontent.com/81839328/116779687-f31aab80-aaa1-11eb-8834-0d41a4a19349.JPG)
Penggunaan operator switch untuk seleksi kondisi
~~~
<html>
<head>
    <title>Contoh program javascript</title>
    <script language = "javascript">
    function test ()
    {
        vall=window.prompt("input nilai (1-5):")
        switch (vall)
        {
            case "1" :
                document.write("bilangan satu")
                break
            case "2" :
                document.write("bilangan dua")
                break
            case "3" :
                document.write("bilangan tiga")
                break
            case "4" :
                document.write("bilangan empat")
                break            
            case "5" :
                document.write("bilangan lima")
                break
            default :
                document.write("bilangan lainnya")
        }
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
~~~
![8  operator switch](https://user-images.githubusercontent.com/81839328/116779696-04fc4e80-aaa2-11eb-83dd-6658abc407e3.JPG)
![8  Hasil](https://user-images.githubusercontent.com/81839328/116779700-06c61200-aaa2-11eb-9b0b-5cf6cb734045.JPG)
# 4. Pembuatan Form
Form Input
~~~
<html>
<head>
    <title>Contoh program javascript</title>
    <script language = "javascript">
    function test ()
    {
        var val1=document.kirim.T1.value
        if (val1%2==0)
            document.kirim.T2.value="bilangan genap"
        else
            document.kirim.T2.value="bilangan ganjil"
    }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
~~~
![9  Pembuatan form input](https://user-images.githubusercontent.com/81839328/116779721-2826fe00-aaa2-11eb-8da9-4629e8a06ee1.JPG)
Form Button
~~~
<html>
<head>
    <title>Contoh program javascript</title>
</head>
<body>
    <script language = "javascript">
    <!--
    function ubahWarnaLB(warna) {
        document.bgColor = warna;
    }
    function ubahWarnaLD(warna) {
        document.fgColor = warna;
    }   
        -->
    </script>
    <h1>Tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onClick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onClick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onClick="ubahWarnaLD('YELLOW')">
        <input type="button" value="Teks Biru" onClick="ubahWarnaLD('BLUE')">
    </form>
    <script language = "javascript">
    <!--
     document.write("Dimodifikasi terakhir pada" +
     document.lastModified);
    //-->
    </script>
</body>
</html>
~~~
![10  Form Button](https://user-images.githubusercontent.com/81839328/116779731-3d039180-aaa2-11eb-9f5d-49e99204885b.JPG)
# 5. HTML DOM
Pilihan menggunakan checkBox dengan perhitungan otomatis
~~~
 <!--
File: daftar_menu.html
//-->
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;
            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            }
            else {
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
<label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp.5000 </label><br />
<label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp.500 </label><br />
<label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp.2500 </label><hr />
<strong>Total Bayar : Rp. <input id="total" type="text" /></strong>
</body>
</html>
~~~
![Uploading 11. DOM.JPG…]()

# Pertanyaan dan Tugas
1. Buat script untuk melakukan validasi pada isian form.
~~~
