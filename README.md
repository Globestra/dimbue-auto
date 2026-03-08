<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dimbue Auto Market</title>

<style>

body{
font-family:Arial;
margin:0;
background:#f2f2f2;
}

header{
background:#000;
color:white;
padding:20px;
display:flex;
justify-content:space-between;
align-items:center;
}

.logo{
font-size:24px;
font-weight:bold;
color:#ff3c3c;
}

nav a{
color:white;
margin:10px;
text-decoration:none;
}

.hero{
background:url('https://images.unsplash.com/photo-1503376780353-7e6692767b70');
background-size:cover;
height:400px;
display:flex;
align-items:center;
justify-content:center;
color:white;
font-size:40px;
font-weight:bold;
}

.container{
padding:40px;
}

.car-list{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
}

.car{
background:white;
padding:15px;
border-radius:10px;
box-shadow:0 5px 10px rgba(0,0,0,0.1);
}

.car img{
width:100%;
border-radius:10px;
}

.price{
color:red;
font-size:20px;
font-weight:bold;
}

button{
background:red;
color:white;
padding:10px;
border:none;
border-radius:5px;
cursor:pointer;
width:100%;
}

footer{
background:black;
color:white;
text-align:center;
padding:20px;
margin-top:40px;
}

</style>

</head>

<body>

<header>

<div class="logo">DIMBUE AUTO</div>

<nav>
<a href=" ">Accueil</a >
<a href="#">Voitures</a >
<a href="#">Contact</a >
</nav>

</header>

<div class="hero">
Voitures fiables au meilleur prix
</div>

<div class="container">

<h2>Nos voitures disponibles</h2>

<div class="car-list">

<div class="car">
< img src="https://images.unsplash.com/photo-1555215695-3004980ad54c">
<h3>Toyota RAV4 2016</h3>
<p>Engine 2.0L</p >
<p class="price">9800 USD</p >
<button onclick="contact()">Contact WhatsApp</button>
</div>

<div class="car">
< img src="https://images.unsplash.com/photo-1542362567-b07e54358753">
<h3>Haval SUV</h3>
<p>Automatic</p >
<p class="price">8500 USD</p >
<button onclick="contact()">Contact WhatsApp</button>
</div>

<div class="car">
< img src="https://images.unsplash.com/photo-1503736334956-4c8f8e92946d">
<h3>Honda CRV</h3>
<p>Very clean</p >
<p class="price">9200 USD</p >
<button onclick="contact()">Contact WhatsApp</button>
</div>

</div>

</div>

<footer>

<p>© 2026 Dimbue Auto Market</p >
<p>Contact WhatsApp : +86XXXXXXXX</p >

</footer>

<script>

function contact(){
window.location.href="https://wa.me/86123456789";
}

</script>

</body>
</html>
