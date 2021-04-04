## Praktikum Latihan 2:

### 1. Membuat dokumen HTML

```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CSS Dasar</title>
</head>
<body>
<header>
<h1>CSS Internal dan <i>Inline CSS</i></h1>
</header>
<nav>
<a href="lab2_css_dasar.html">CSS Dasar</a>
<a href="lab2_css_eksternal.html">CSS Eksternal</a>
<a href="lab1_tag_dasar.html">HTML Dasar</a>
</nav>
<!-- CSS ID Selector -->
<div id="intro">
<h1>Hello World</h1>
<p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</p>
<!-- CSS Class Selector -->
<a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
</div>
</body>
</html>
```

![Screenshot (15)](https://user-images.githubusercontent.com/81921974/113520565-27dc3580-95be-11eb-8f91-270786b86598.png)

### 2. Mendeklarasikan CSS Internal

```
<head>
<title>CSS Dasar</title>
<style>
body {
font-family:'Open Sans', sans-serif;
}
header {
min-height: 80px;
border-bottom:1px solid #77CCEF;
}
h1 {
font-size: 24px;
color: #0F189F;
text-align: center;
padding: 20px 10px;
}
h1 i {
color:#6d6a6b;
}
</style>
</head>
```

![Screenshot (17)](https://user-images.githubusercontent.com/81921974/113520748-8fdf4b80-95bf-11eb-933b-82690febd472.png)

### 3. Menambahkan Inline CSS

*`Kemudian menambahkan deklarasi inline CSS pada tag <p> seperti berikut.`*

**```<p style="text-align: center; color: #ccd8e4;">```**

![Screenshot (19)](https://user-images.githubusercontent.com/81921974/113520985-ca95b380-95c0-11eb-9a1a-92be298dd729.png)

### 4. Membuat CSS Eksternal

*`Membuat file baru dengan nama style_eksternal.css kemudian membuat deklarasi CSS.`*

```
nav {
background: #20A759;
color:#fff;
padding: 10px;
}
nav a {
color: #fff;
text-decoration: none;
padding:10px 20px;
}
nav .active,
nav a:hover {
background: #0B6B3A;
}
```
*`Kemudian menambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head>`*
```
<head>
<!-- menyisipkan css eksternal -->
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```
![Screenshot (21)](https://user-images.githubusercontent.com/81921974/113521228-4e03d480-95c2-11eb-88d4-e46611c6ff71.png)

### 5. Menambahkan CSS Selector

*`Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css.`*

```
/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}
```
## Hasil Akhir

![Screenshot (23)](https://user-images.githubusercontent.com/81921974/113521313-dbdfbf80-95c2-11eb-91a4-a6ebd37449bb.png)


