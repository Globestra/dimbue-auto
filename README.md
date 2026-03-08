<!DOCTYPE html>
<html lang="fr">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Globestra Trade</title>

<style>

body{
font-family:Arial;
margin:0;
background:#f4f4f4;
}

header{
background:#0a0a0a;
color:white;
padding:20px;
display:flex;
justify-content:space-between;
align-items:center;
}

.logo{
font-size:28px;
color:#ff3b3b;
font-weight:bold;
}

nav a{
color:white;
margin-left:15px;
text-decoration:none;
}

.hero{
background:url("https://images.unsplash.com/photo-1552519507-da3b142c6e3d");
height:420px;
background-size:cover;
display:flex;
align-items:center;
justify-content:center;
color:white;
font-size:40px;
font-weight:bold;
text-align:center;
}

.container{
padding:40px;
}

.products{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
}

.product{
background:white;
border-radius:10px;
overflow:hidden;
box-shadow:0 5px 15px rgba(0,0,0,0.1);
}

.product img{
width:100%;
height:200px;
object-fit:cover;
}

.product-info{
padding:15px;
}

.price{
color:red;
font-size:22px;
font-weight:bold;
}

button{
background:#ff3b3b;
color:white;
border:none;
padding:10px;
width:100%;
margin-top:10px;
border-radius:6px;
cursor:pointer;
}

.admin{
background:white;
padding:30px;
margin-top:50px;
border-radius:10px;
}

input{
padding:10px;
margin:5px;
width:100%;
}

footer{
background:black;
color:white;
text-align:center;
padding:30px;
margin-top:50px;
}

.tiktok{
position:fixed;
bottom:20px;
left:20px;
background:black;
color:white;
padding:10px 20px;
border-radius:40px;
}

</style>

</head>

<body>

<header>

<div class="logo">GLOBESTRA TRADE</div>

<nav>

<a href=" ">Accueil</a >
<a href="#">Voitures</a >
<a href="#">Produits</a >
<a href="#">Contact</a >

</nav>

</header>

<div class="hero">

Importation Chine • Voitures • Marchandises

</div>

<div class="container">

<h2>Produits disponibles</h2>

<div class="products" id="productList">

</div>

<div class="admin">

<h2>Ajouter un produit</h2>

<input id="name" placeholder="Nom du produit">
<input id="price" placeholder="Prix">
<input id="image" placeholder="Lien image">

<button onclick="addProduct()">Ajouter</button>

</div>

</div>

<footer>

<p>Globestra Trade Import Export</p >

<p>WhatsApp : +86XXXXXXXX</p >

</footer>

<div class="tiktok">

Suivez-nous sur TikTok

</div>

<script>

let products=[]

function addProduct(){

let name=document.getElementById("name").value
let price=document.getElementById("price").value
let image=document.getElementById("image").value

let product={
name,
price,
image
}

products.push(product)

displayProducts()

}

function displayProducts(){

let container=document.getElementById("productList")

container.innerHTML=""

products.forEach(p=>{

container.innerHTML+=`

<div class="product">

< img src="${p.image}">

<div class="product-info">

<h3>${p.name}</h3>

<div class="price">$${p.price}</div>

<button onclick="buy()">Acheter</button>

</div>

</div>

`

})

}

function buy(){

window.location="https://wa.me/86123456789"

}

</script>

</body>

</html>
