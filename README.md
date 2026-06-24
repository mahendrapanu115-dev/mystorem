<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Roasted Sing Store</title>


<style>


*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}


body{

background:#050505;
color:white;

}



/* OFFER */

.offer{

background:#ffb000;
color:#000;
text-align:center;
padding:10px;
font-weight:bold;

}



/* SEARCH */

.search-box{

background:#fff;
padding:15px;
display:flex;
justify-content:center;

}


.search{

width:95%;
max-width:600px;
height:50px;
display:flex;
background:white;
border-radius:30px;
box-shadow:0 5px 20px #333;
overflow:hidden;

}


.search input{

flex:1;
border:none;
outline:none;
padding:15px;
font-size:16px;

}



.search button{

width:100px;
border:none;
background:#ffb000;
font-weight:bold;
cursor:pointer;

}




/* HEADER */


header{

text-align:center;
padding:30px 10px;

}


header h1{

font-size:35px;
color:#ffb000;
animation:show 1s;

}


header p{

color:#ccc;
margin-top:10px;

}



@keyframes show{

from{

opacity:0;
transform:translateY(-30px);

}

to{

opacity:1;

}

}




/* PRODUCTS */


.container{

width:100%;
max-width:1200px;
margin:auto;
padding:20px;

}


.products{

display:grid;
grid-template-columns:repeat(4,1fr);
gap:20px;

}





.card{

background:#111;
border-radius:20px;
overflow:hidden;
position:relative;
padding-bottom:15px;
transition:.4s;
border:1px solid #333;

}


.card:hover{

transform:translateY(-10px);
box-shadow:0 0 25px #ffb000;

}



.card img{

width:100%;
height:220px;
object-fit:contain;
background:white;
transition:.4s;

}


.card:hover img{

transform:scale(1.08);

}




.tag{

position:absolute;
top:10px;
left:10px;
background:red;
padding:5px 12px;
border-radius:20px;
font-size:12px;

}



.info{

text-align:center;
padding:15px;

}



.info h2{

font-size:18px;

}



.star{

color:#ffb000;
margin:8px;

}



.price{

color:#00ff66;
font-size:25px;
font-weight:bold;

}



.btn{

display:block;
margin:10px;
padding:12px;
border-radius:25px;
text-decoration:none;
text-align:center;
font-weight:bold;

}



.pay{

background:#ffb000;
color:black;

}



.order{

background:#25D366;
color:white;

}




/* WHATSAPP */


.float{

position:fixed;
right:20px;
bottom:20px;

background:#25D366;
color:white;

font-size:30px;

padding:15px;
border-radius:50%;

}




/* MOBILE */


@media(max-width:767px){


.products{

grid-template-columns:repeat(2,1fr);
gap:10px;

}



.card img{

height:150px;

}



.info{

padding:8px;

}


.info h2{

font-size:13px;

}



.price{

font-size:18px;

}



.btn{

font-size:12px;
padding:8px;

}



header h1{

font-size:25px;

}


.search button{

width:80px;

}



}




</style>


</head>



<body>



<div class="offer">

🔥 Roasted Sing Special Offer ₹150 Only 🔥

</div>




<div class="search-box">

<div class="search">


<input id="search" placeholder="Search Product">


<button>

🔍 Search

</button>


</div>

</div>





<header>

<h1>

🥜 Roasted Sing Store

</h1>


<p>

Fresh Quality | Fast Delivery

</p>


</header>






<div class="container">


<div class="products" id="products">




<div class="card">


<div class="tag">

BEST

</div>


<img src="divya.new.jpg">


<div class="info">

<h2>

ROASTED SING

</h2>


<div class="star">

⭐⭐⭐⭐⭐

</div>


<div class="price">

₹150

</div>


<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order WhatsApp

</a>


</div>


</div>





<div class="card">


<img src="HARSHITA.jpg">


<div class="info">

<h2>

BANASKATHA SING

</h2>


<div class="star">

⭐⭐⭐⭐

</div>


<div class="price">

₹120

</div>


<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order WhatsApp

</a>


</div>


</div>






<div class="card">


<img src="product3.jpg">


<div class="info">

<h2>

PREMIUM SING

</h2>


<div class="star">

⭐⭐⭐⭐⭐

</div>


<div class="price">

₹180

</div>


<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order WhatsApp

</a>


</div>


</div>






<div class="card">


<img src="product4.jpg">


<div class="info">

<h2>

SPECIAL SING

</h2>


<div class="star">

⭐⭐⭐⭐

</div>


<div class="price">

₹200

</div>


<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order WhatsApp

</a>


</div>


</div>





</div>

</div>





<a class="float">

📲

</a>






<script>


let search=document.getElementById("search");


let cards=document.querySelectorAll(".card");



search.addEventListener("keyup",()=>{


let value=search.value.toLowerCase();


cards.forEach(card=>{


let text=card.innerText.toLowerCase();


if(text.includes(value)){

card.style.display="block";

}

else{

card.style.display="none";

}


});


});



</script>



</body>

</html>
