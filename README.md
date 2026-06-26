<!DOCTYPE html>
<html>
<head>

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Mera Store</title>


<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial;
}


body{
background:#f2f2f2;
}



header{

background:white;
padding:20px;
text-align:center;

}



.logo{

font-size:28px;
font-weight:bold;
color:#2874f0;

}


.search{

margin-top:20px;

display:flex;
justify-content:center;
gap:5px;

}


.search input{

width:70%;
padding:12px;

border-radius:20px;

border:1px solid #ccc;

}



.search button{

padding:12px 18px;

border:0;

border-radius:20px;

background:#2874f0;

color:white;

}




.container{

padding:10px;

}



.products{

display:grid;

grid-template-columns:repeat(2,1fr);

gap:10px;

}




.card{


background:white;

border-radius:10px;

overflow:hidden;

box-shadow:0 2px 8px #ccc;

}




.img{


height:150px;

overflow:hidden;

}



.img img{


width:100%;

height:100%;

object-fit:contain;

transition:.4s;


}



.card:hover img{

transform:scale(1.1);

}




.info{

text-align:center;

padding:10px;

}



.info h3{

font-size:14px;

}



.price{

color:green;

font-size:20px;

font-weight:bold;

margin:8px;

}



button.buy,
button.order{


width:100%;

padding:10px;

border:0;

border-radius:5px;

margin-top:5px;

color:white;


}



.buy{

background:#ff9800;

}



.order{

background:#25D366;

}




@media(min-width:800px){


.products{

grid-template-columns:repeat(4,1fr);

}


}




</style>


</head>


<body>



<header>


<div class="logo">

🛒 mystorem

</div>


<p>Best Quality Products | Fast Delivery</p>



<div class="search">


<input id="search" placeholder="Search product">


<button onclick="find()">

🔍 Search

</button>


</div>


</header>




<div class="container">


<div class="products">



<div class="card">


<div class="img">

<img src="chana.jpg">

</div>


<div class="info">


<h3>ROASTED SING</h3>


<div class="price">

₹150

</div>


<button class="buy">

💳 Pay Now

</button>


<button class="order">

📲 Order

</button>


</div>


</div>







<div class="card">


<div class="img">

<img src="HARSHITA.jpg">

</div>


<div class="info">


<h3>BANASKATHA SING</h3>


<div class="price">

₹120

</div>


<button class="buy">

💳 Pay Now

</button>


<button class="order">

📲 Order

</button>


</div>


</div>






<div class="card">


<div class="img">

<img src="product3.jpg">

</div>


<div class="info">


<h3>PRODUCT 3</h3>


<div class="price">

₹180

</div>


<button class="buy">

💳 Pay Now

</button>


<button class="order">

📲 Order

</button>


</div>


</div>






<div class="card">


<div class="img">

<img src="product4.jpg">

</div>


<div class="info">


<h3>PRODUCT 4</h3>


<div class="price">

₹200

</div>


<button class="buy">

💳 Pay Now

</button>


<button class="order">

📲 Order

</button>


</div>


</div>



</div>


</div>





<script>


function find(){


let text=document
.getElementById("search")
.value
.toLowerCase();


let cards=document
.querySelectorAll(".card");



cards.forEach(function(card){


let name=card
.querySelector("h3")
.innerText
.toLowerCase();



if(name.includes(text)){

card.style.display="block";

}

else{

card.style.display="none";

}


});


}



</script>



</body>

</html>
