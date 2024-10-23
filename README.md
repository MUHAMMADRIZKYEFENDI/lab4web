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
![Screenshot (242)](https://github.com/user-attachments/assets/9b186984-2ca2-4d9e-9abd-abe14bf494b5)
# Membuat Navigasi 
Kemudian selanjutnya mengatur navigasi. 
```/* navigasi */ 
nav { 
display: block; 
background-color: #1f5faa; 
} 
nav a { 
padding: 15px 30px; 
display: inline-block; 
color: #ffffff; 
font-size: 14px; 
text-decoration: none; 
font-weight: bold; 
} 
nav a.active, 
nav a:hover { 
background-color: #2b83ea; 
}
```
Kemudian lihat hasilnya. 
![Screenshot (244)](https://github.com/user-attachments/assets/d6587fe7-bdc6-417c-9845-5964e19bde17)
# Membuat Hero Panel. 
Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut. 
```
<section id="hero"> 
    <h1>Hello World!</h1> 
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p> 
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a> 
</section> 
 ```
# cssnya
```
/* Hero Panel */ 
#hero { 
    background-color: #e4e4e5; 
    padding: 50px 20px; 
    margin-bottom: 20px; 
} 
 
#hero h1 { 
    margin-bottom: 20px; 
    font-size: 35px; 
} 
 
#hero p { 
    margin-bottom: 20px; 
    font-size: 18px; 
    line-height: 25px; 
}
```
gambarnya
![Screenshot (245)](https://github.com/user-attachments/assets/39c56d3d-646c-4602-9f15-261050f242cf)
# Mengatur Layout Main dan Sidebar 
Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
```
/* main content */ 
#wrapper { 
    margin: 0; 
}
#main { 
    float: left; 
    width: 640px; 
    padding: 20px; 
} 
 
/* sidebar area */ 
#sidebar { 
    float: left; 
    width: 260px; 
    padding: 20px; 
}
```
# Membuat Sidebar Widget 
Kemudian selanjutnya menambahkan element lain dalam sidebar. 
```
<aside id="sidebar"> 
    <div class="widget-box"> 
        <h3 class="title">Widget Header</h3> 
        <ul> 
            <li><a href="#">Widget Link</a></li> 
            <li><a href="#">Widget Link</a></li> 
            <li><a href="#">Widget Link</a></li> 
            <li><a href="#">Widget Link</a></li> 
            <li><a href="#">Widget Link</a></li> 
        </ul> 
    </div> 
    <div class="widget-box"> 
        <h3 class="title">Widget Text</h3> 
        <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt 
arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer 
pharetra est nunc, nec pretium nunc pretium ac.</p> 
    </div> 
</aside> 
 ```
# Kemudian tambahkan CSS. 
```
/* widget */ 
.widget-box { 
    border:1px solid #eee; 
    margin-bottom:20px; 
} 
 
.widget-box  .title { 
    padding:10px 16px; 
    background-color:#428bca; 
    color:#fff; 
} 
 
.widget-box ul { 
    list-style-type:none; 
} 
 
.widget-box li { 
    border-bottom:1px solid #eee;
} 
.widget-box li a { 
padding:10px 16px; 
color:#333; 
display:block; 
text-decoration:none; 
} 
.widget-box li:hover a { 
background-color:#eee; 
} 
.widget-box p { 
padding:15px; 
line-height:25px; 
} 
```
gambar
![Screenshot (247)](https://github.com/user-attachments/assets/8eb8cbb3-a8bc-479c-a24c-6f2f265985d5)
# Mengatur Footer 
Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer. 
/* footer */ 
footer { 
clear:both; 
background-color:#1d1d1d; 
padding:20px; 
color:#eee; 
}
gambar
![Screenshot (247)](https://github.com/user-attachments/assets/8eb8cbb3-a8bc-479c-a24c-6f2f265985d5)
# Menambahkan Elemen lainnya pada Main Content 
 ```
<section id="main"> 
    <div class="row"> 
        <div class="box"> 
            <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" 
class="image-circle"> 
            <h3>Heading</h3> 
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p> 
            <a href="#" class="btn btn-default">View detail</a> 
        </div> 
        <div class="box"> 
            <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" 
class="image-circle"> 
            <h3>Heading</h3> 
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p> 
            <a href="#" class="btn btn-default">View detail</a> 
        </div> 
        <div class="box"> 
            <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" 
class="image-circle"> 
            <h3>Heading</h3> 
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
euismod.</p> 
            <a href="#" class="btn btn-default">View detail</a> 
        </div> 
    </div> 
</section> 
 ```
# Kemudian tambahkan CSS. 
```/* box */ 
.box { 
    display:block; 
    float:left; 
    width:33.333333%; 
    box-sizing:border-box; 
    -moz-box-sizing:border-box; 
    -webkit-box-sizing:border-box;
 padding:0 10px; 
    text-align:center; 
} 
 
.box h3 { 
    margin: 15px 0; 
} 
 
.box p { 
    line-height: 20px; 
    font-size: 14px; 
    margin-bottom: 15px; 
} 
 
box img { 
    border: 0; 
    vertical-align: middle; 
} 
 
.image-circle { 
    border-radius: 50%; 
} 
 
.row { 
    margin: 0 -10px; 
    box-sizing: border-box; 
    -moz-box-sizing: border-box; 
    -webkit-box-sizing: border-box; 
} 
 
.row:after, .row:before, 
.entry:after, .entry:before { 
    content:''; 
    display:table; 
} 
 
.row:after, 
.entry:after { 
    clear:both; 
} 
```
Lihat hasilnya dibrowser.
![Screenshot (248)](https://github.com/user-attachments/assets/d8aa6d91-fad5-45ca-83d0-fe7c0fd65ff0)
# Menambahkan Content Artikel 
Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content. 
```<hr class="divider" /> 
<article class="entry"> 
    <h2>First featurette heading.</h2> 
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""> 
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p> 
</article> 
<hr class="divider" /> 
<article class="entry"> 
    <h2>First featurette heading.</h2> 
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" 
class="right-img"> 
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
pretium ac.</p> 
</article> 
 ```
# Kemudian tambahkan CSS. 
```.divider { 
    border:0; 
    border-top:1px solid #eeeeee; 
    margin:40px 0; 
} 
 
/* entry */ 
.entry { 
    margin: 15px 0; 
} 
 
.entry h2 { 
    margin-bottom: 20px; 
} 
.entry p { 
line-height: 25px; 
} 
.entry img { 
float: left; 
border-radius: 5px; 
margin-right: 15px; 
} 
.entry .right-img { 
float: right; 
}
```
hasil browsernya
![Screenshot (249)](https://github.com/user-attachments/assets/d68cd2b3-001c-4154-a8d3-b6301b80070a)
