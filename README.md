# lab4web
# Praktikum 4: CSS Layout
# Langkah-langkah Praktikum 
Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut. 
```
<!DOCTYPE html> 
<html lang="en"> 
<head> 
    <meta charset="UTF-8"> 
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>Box Element</title> 
</head> 
<body> 
    <header> 
        <h1>Box Element</h1> 
    </header> 
</body> 
</html> 
 
Membuat Box Element 
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut. 
<section> 
    <div class="div1">Div 1</div> 
    <div class="div2">Div 2</div> 
    <div class="div3">Div 3</div>       
</section> 
 
CSS Float Property 
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut. 
<style> 
    div { 
        float:left; 
        padding: 10px;  
    } 
    .div1 { 
        background: red; 
    } 
    .div2 { 
        background: yellow; 
    } 
    .div3 { 
        background: green; 
    } 
</style>
```
 
Kemudian buka browser untuk melihat hasilnya.
![Screenshot (240)](https://github.com/user-attachments/assets/6bcd369d-927b-44a5-90f0-356c3cc4ce64)

# Mengatur Clearfix Element 
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk 
mengaturnya. 
Tambahkan element div lainnya seteleah div3 seperti berikut. 
```
<section> 
<div class="div1">Div 1</div> 
<div class="div2">Div 2</div> 
<div class="div3">Div 3</div>   
<div class="div4">Div 4</div>     
</section> 
Kemudian atur property clear pada CSS, seperti berikut. 
.div4 { 
background-color: blue; 
clear: left; 
float: none; 
}
```
Selanjutnya buka browser dan refresh kembali.
![Screenshot (241)](https://github.com/user-attachments/assets/0362a8cb-58b5-4897-8ca8-cff2085c6a26)
# Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css.
```
<!DOCTYPE html> 
<html lang="en"> 
<head>
<meta charset="UTF-8"> 
<meta name="viewport" content="width=device-width, initial-scale=1.0"> 
<title>Layout Sederhana</title> 
<link rel="stylesheet" href="style.css"> 
</head> 
<body> 
<div id="container"> 
</div> 
</body> 
</html>
```
# Kemudian tulis kode berikut. 
```
<header> 
<h1>Layout Sederhana</h1> 
</header> 
<nav> 
<a href="home.html" class="active">Home</a> 
<a href="artikel.html">Artikel</a> 
<a href="about.html">About</a> 
<a href="kontak.html">Kontak</a> 
</nav> 
<section id="hero"></section> 
<section id="wrapper"> 
<section id="main"></section> 
<aside id="sidebar"></aside> 
</section> 
<footer> 
<p>&copy; 2021 - Universitas Pelita Bangsa</p> 
</footer>
```
Kemudian buka browser dan lihat hasilnya.
