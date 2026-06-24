<!DOCTYPE html>
<html>
<head>

<title>Roasted Sing Store</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}


body{

background:#f5f5f5;

}



/* OFFER */

.offer{

background:#111;
color:#ffb000;
text-align:center;
padding:10px;
font-weight:bold;

}



/* SEARCH */

.search-wrapper{

background:white;
padding:15px;
display:flex;
justify-content:center;

}


.search-container{

width:600px;
height:55px;
display:flex;
background:white;
border-radius:35px;
box-shadow:0 5px 20px #ddd;
padding:5px;

}


.search-container input{

flex:1;
border:none;
outline:none;
padding-left:20px;
font-size:16px;

}


.search-btn{

background:#0d8cff;
color:white;
border:none;
border-radius:30px;
padding:0 30px;
cursor:pointer;

}




/* HEADER */

header{

background:white;
text-align:center;
padding:20px;

}


header h1{

color:#222;
animation:pop 1s;

}


header p{

color:#777;

}




@keyframes pop{

from{

opacity:0;
transform:scale(.5);

}

to{

opacity:1;

}

}





/* CONTAINER */

.container{

max-width:1200px;
margin:auto;
padding:20px;

}



/* PRODUCTS */

.products{

display:grid;
grid-template-columns:repeat(2,1fr);
gap:15px;

}



/* CARD */

.product{

background:white;
border-radius:15px;
overflow:hidden;
position:relative;
box-shadow:0 5px 15px #ddd;
transition:.4s;

}


.product:hover{

transform:translateY(-10px);
box-shadow:0 15px 30px #bbb;

}



.badge{

position:absolute;
top:10px;
left:10px;
background:#ff0000;
color:white;
padding:5px 12px;
border-radius:20px;
font-size:12px;

}




.product img{

width:100%;
height:200px;
object-fit:cover;
transition:.4s;

}



.product:hover img{

transform:scale(1.08);

}



.product-content{

padding:12px;
text-align:center;

}



.product h2{

font-size:16px;

}



.rating{

color:#ffb000;
margin:5px;

}



.price{

color:green;
font-size:22px;
font-weight:bold;

}




.btn{

display:block;
padding:10px;
margin-top:8px;
border-radius:8px;
text-decoration:none;
color:white;

}



.buy{

background:#0a8f08;

}


.whatsapp{

background:#25D366;

}





/* DESKTOP */


@media(min-width:768px){

.products{

grid-template-columns:repeat(4,1fr);

}

}




/* FLOAT WHATSAPP */


.float{

position:fixed;
right:20px;
bottom:20px;
background:#25D366;
color:white;
font-size:30px;
padding:15px;
border-radius:50%;
text-decoration:none;

}


</style>


</head>


<body>


<div class="offer">

🔥 Today Offer: Roasted Sing ₹150 Only | Free Delivery

</div>




<div class="search-wrapper">

<div class="search-container">


<input id="search" placeholder="Search Product...">


<button class="search-btn">

🔍

</button>


</div>

</div>





<header>

<h1>

🥜 Mera Online Store

</h1>


<p>

Best Quality Products | Fast Delivery

</p>


</header>






<div class="container">


<div class="products" id="products">





<div class="product">


<div class="badge">

Best Seller

</div>


<img src="divya.new.jpg">


<div class="product-content">


<h2>

ROASTED SING

</h2>


<div class="rating">

⭐⭐⭐⭐⭐

</div>


<div class="price">

₹150

</div>



<a class="btn buy">

💳 Pay Now

</a>


<a class="btn whatsapp">

📲 Order

</a>


</div>

</div>






<div class="product">


<img src="HARSHITA.jpg">


<div class="product-content">


<h2>

BANASKATHA SING

</h2>


<div class="rating">

⭐⭐⭐⭐

</div>


<div class="price">

₹120

</div>


<a class="btn buy">

💳 Pay Now

</a>


<a class="btn whatsapp">

📲 Order

</a>


</div>

</div>







<div class="product">


<img src="product3.jpg">


<div class="product-content">


<h2>

ROASTED PEANUT

</h2>


<div class="rating">

⭐⭐⭐⭐⭐

</div>


<div class="price">

₹180

</div>


<a class="btn buy">

💳 Pay Now

</a>


<a class="btn whatsapp">

📲 Order

</a>


</div>


</div>






<div class="product">


<img src="product4.jpg">


<div class="product-content">


<h2>

PREMIUM SING

</h2>


<div class="rating">

⭐⭐⭐⭐

</div>


<div class="price">

₹200

</div>


<a class="btn buy">

💳 Pay Now

</a>


<a class="btn whatsapp">

📲 Order

</a>


</div>


</div>





</div>

</div>





<a class="float" href="https://wa.me/919601393176">

📲

</a>





<script>


let search=document.getElementById("search");

let products=document.querySelectorAll(".product");


search.addEventListener("keyup",function(){


let value=this.value.toLowerCase();


products.forEach(function(product){


let name=product.innerText.toLowerCase();


if(name.includes(value)){

product.style.display="block";

}

else{

product.style.display="none";

}


});


});



</script>



</body>
</html>
