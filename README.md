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



# MENU ABOUT YANG BERISI PORTOFOLIO
HTML NYA
```
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
    <link rel="stylesheet" href="portofolio.css">
    <title>Portfolio Website</title>
</head>

<body>
    <header>
        <a href="#" class="logo">M RIZKY EFENDI</a>

        <nav>
            <a href="#" class="active"> Home</a>
            <a href="#">Services</a>
            <a href="#">Skills</a>
            <a href="#">Education</a>
            <a href="#">Experience</a>
            <a href="#">Contact</a>
        </nav>
    </header>
    <section class="home">
        <div class="home-img">
            <img src="foto.png" alt="">
        </div>
        <div class="home-content">
            <h1>Hi, It's <span>M RIZKY</span></h1>
            <h3 class="typing-text">I'm a <span></span></h3>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minus labore dolores esse. Odit similique
                doloribus tenetur doloremque, sunt commodi in ipsa repudiandae debitis deleniti blanditiis quibusdam
                quaerat neque asperiores ea.</p>
            <div class="social-icons">
                <a href="#"><i class="fa-brands fa-linkedin"></i></a>
                <a href="#"><i class="fa-brands fa-github"></i></a>
                <a href="#"><i class="fa-brands fa-x-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-instagram"></i></a>
            </div>
            <a href="#" class="btn">Hire me</a>
        </div>
    </section>
</body>

</html>
```
CSS NYA
```
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    font-family: 'Poppins', sans-serif;
}

html {
    font-size: 62.5%;
}

body {
    width: 100%;
    height: 100vh;
    overflow-x: hidden;
    background-color: black;
    color: white;
}

header {
    margin-top: 20px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 1rem 9%;
    background-color: transparent;
    filter: drop-shadow(10px);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.logo {
    font-size: 3rem;
    color: #b74b4b;
    font-weight: 800;
    cursor: pointer;
    transition: 0.5s ease;
}

.logo:hover {
    transform: scale(1.1);
}

nav a {
    font-size: 1.8rem;
    color: white;
    margin-left: 4rem;
    font-weight: 500;
    transition: 0.3s ease;
    border-bottom: 3px solid transparent;
}

nav a:hover,
nav a.active {
    color: #b74b4b;
    border-bottom: 3px solid #b74b4b;
}

@media(max-width:995px) {
    nav {
        position: absolute;
        display: none;
        top: 0;
        right: 0;
        width: 40%;
        border-left: 3px solid #b74b4b;
        border-bottom: 3px solid #b74b4b;
        border-bottom-left-radius: 2rem;
        padding: 1rem solid;
        background-color: #161616;
        border-top: 0.1rem solid rgba(0, 0, 0, 0.1);
    }

    nav.active {
        display: block;
    }

    nav a {
        display: block;
        font-size: 2rem;
        margin: 3rem 0;
    }

    nav a:hover,
    nav a.active {
        padding: 1rem;
        border-radius: 0.5rem;
        border-bottom: 0.5rem solid #b74b4b;
    }
}

section {
    min-height: 100vh;
    padding: 5rem 9% 5rem;
}

.home {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 8rem;
    background-color: black;
}

.home .home-content h1 {
    font-size: 6rem;
    font-weight: 700;
    line-height: 1.3;
}

span {
    color: #b74b4b;
}

.home-content h3 {
    font-size: 4rem;
    margin-bottom: 1rem;
    font-weight: 700;
}

.home-content p {
    font-size: 1.6rem;
}

.home-img {
    border-radius: 50%;
}

.home-img img {
    position: relative;
    width: 32vw;
    border-radius: 50%;
    box-shadow: 0 0 25px solid #b74b4b;
    cursor: pointer;
    transition: 0.2s linear;
}

.home-img img:hover {
    font-size: 1.8rem;
    font-weight: 500;
}

.social-icons a {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4rem;
    height: 4rem;
    background-color: transparent;
    border: 0.2rem solid #b74b4b;
    font-size: 2rem;
    border-radius: 50%;
    margin: 3rem 1.5rem 3rem 0;
    transition: 0.3s ease;
    color: #b74b4b;
}

.social-icons a:hover {
    color: black;
    transform: scale(1.3) translateY(-5px);
    background-color: #b74b4b;
    box-shadow: 0 0 25px #b74b4b;
}

.btn {
    display: inline-block;
    padding: 1rem 2.8rem;
    background-color: black;
    border-radius: 4rem;
    font-size: 1.6rem;
    color: #b74b4b;
    letter-spacing: 0.3rem;
    font-weight: 600;
    border: 2px solid #b74b4b;
    transition: 0.3s ease;
    cursor: pointer;
}

.btn:hover {
    transform: scale3d(1.03);
    background-color: #b74b4b;
    color: black;
    box-shadow: 0 0 25px #b74b4b;
}

.typing-text {
    font-size: 34px;
    font-weight: 600;
    min-width: 280px;
}

.typing-text span {
    position: relative;
}

.typing-text span::before {
    content: "software Developer";
    color: #b74b4b;
    animation: words 20s infinite;
}

.typing-text span::after {
    content: "";
    background-color: black;
    position: absolute;
    width: calc(100% + 8px);
    height: 100%;
    border-left: 3px solid black;
    right: -8;
    animation: cursor 0.6s infinite;
}

@keyframes cursor {
    to {
        border-left: 3px solid #b74b4b;
    }
}

@keyframes words {

    0%,
    20% {
        content: "Web Developer";
    }

    21%,
    40% {
        content: "Developer";
    }

    41%,
    60% {
        content: "Web Designer";
    }

    61%,
    80% {
        content: "BOSS";
    }

    81%,
    100% {
        content: "Script Writer";
    }
}

@media (max-width: 1000px) {
    .home {
        gap: 4rem;
    }
}

@media(max-width:995px) {
    .home {
        flex-direction: column;
        margin: 5rem 4rem;
    }

    .home .home-content h3 {
        font-size: 2.5rem;
    }

    .home-content h1 {
        font-size: 5rem;
    }

    .home-img img {
        width: 70vw;
        margin-top: 4rem;
    }
}
```
HASIL BROWSERNYA

![Screenshot (253)](https://github.com/user-attachments/assets/ce0abf14-c3bc-47b2-80a7-5fe50fa4be94)

# MENU CONTACT
HTML NYA
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Form</title>
    <link rel="stylesheet" href="kontak.css"> <!-- Link to the CSS file -->
</head>

<body>
    <div class="contact-container">
        <form action="" class="contact-left">
            <div class="contact-left-title">
                <h2>Get in Touch</h2>
                <hr>
                <input type="text" name="name" placeholder="Your Name" class="contact-inputs" required>
                <input type="email" name="email" placeholder="Your Email" class="contact-inputs" required>
                <textarea name="message" placeholder="Your Message" class="contact-inputs" required></textarea>
                <button type="submit">Submit</button>
            </div>
        </form>
    </div>
</body>

</html>
```
CSSNYA
```
/* Reset default styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f4f4f9;
}

.contact-container {
    width: 100%;
    max-width: 500px;
    margin: auto;
    padding: 20px;
}

.contact-left {
    background-color: #fff;
    border-radius: 10px;
    padding: 25px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
}

.contact-left-title h2 {
    font-size: 26px;
    color: #333;
    margin-bottom: 15px;
    text-transform: uppercase;
}

.contact-left-title hr {
    width: 60px;
    height: 3px;
    background-color: #3498db;
    border: none;
    margin-bottom: 20px;
}

.contact-inputs {
    width: 100%;
    padding: 14px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
    border-radius: 6px;
    font-size: 17px;
    color: #333;
}

.contact-inputs:focus {
    border-color: #3498db;
    outline: none;
}

button[type="submit"] {
    width: 100%;
    padding: 14px;
    background-color: #3498db;
    border: none;
    border-radius: 6px;
    color: #fff;
    font-size: 18px;
    cursor: pointer;
    text-transform: uppercase;
    transition: background-color 0.3s;
}

button[type="submit"]:hover {
    background-color: #2980b9;
}

/* Responsive Design */
@media (max-width: 768px) {
    .contact-container {
        padding: 15px;
    }

    .contact-left {
        padding: 20px;
    }

    .contact-left-title h2 {
        font-size: 22px;
    }

    .contact-inputs {
        font-size: 16px;
    }

    button[type="submit"] {
        font-size: 16px;
        padding: 12px;
    }
}
```

HASIL BROWSERNYA

![Screenshot (254)](https://github.com/user-attachments/assets/656b089b-46b9-4a2f-9e14-a15830c47764)
