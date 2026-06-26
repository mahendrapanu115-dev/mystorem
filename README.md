<!DOCTYPE html>
<html lang="en">
<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Mera Online Store</title>


<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}


body{

background:#f1f3f6;

}


/* HEADER */

header{

background:white;
text-align:center;
padding:20px;
border-bottom:1px solid #ddd;

}


header h1{

font-size:28px;

animation:textPop 1s;

}



@keyframes textPop{

from{

opacity:0;
transform:scale(.5);

}

to{

opacity:1;
transform:scale(1);

}

}



/* SEARCH */


.search-box{

margin-top:15px;

}


.search-box input{

width:90%;
max-width:400px;

padding:12px;

border-radius:8px;

border:1px solid #ccc;

font-size:15px;

outline:none;

}



/* CONTAINER */


.container{

max-width:1200px;

margin:auto;

padding:15px;

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

border-radius:12px;

overflow:hidden;

box-shadow:0 3px 12px rgba(0,0,0,.15);

transition:.3s;

}



.product:hover{

transform:translateY(-6px);

}



/* IMAGE ANIMATION */


.img-box{

overflow:hidden;

}


.product img{

width:100%;

height:260px;

object-fit:contain;

padding:15px;

transition:.5s;

}



.product:hover img{

transform:scale(1.12);

}





/* CONTENT */


.product-content{

padding:12px;

text-align:center;

}



.product h2{

font-size:15px;

}



.price{

font-size:22px;

font-weight:bold;

color:green;

margin:8px;

}




/* BUTTON */


.btn{

display:block;

padding:10px;

margin-top:8px;

color:white;

text-decoration:none;

border-radius:6px;

}


.buy{

background:#ff9f00;

}


.whatsapp{

background:#25D366;

}




@media(min-width:768px){

.products{

grid-template-columns:repeat(3,1fr);

}

}



@media(min-width:1024px){

.products{

grid-template-columns:repeat(4,1fr);

}

}



</style>

</head>



<body>



<header>


<h1>🛒 Mera Online Store</h1>

<p>Best Quality Products | Fast Delivery</p>


<div class="search-box">

<input type="text" 
id="search"
placeholder="🔍 Search Product..."
onkeyup="searchProduct()">


</div>


</header>





<div class="container">


<div class="products" id="products">



<div class="product">


<div class="img-box">

<img src="chana.jpg">

</div>


<div class="product-content">

<h2>ROASTED SING</h2>

<div class="price">₹150</div>


<a class="btn buy"
href="upi://pay?pa=yourupi@upi&am=150&cu=INR">

💳 Pay Now

</a>


<a class="btn whatsapp"
href="https://wa.me/919601393176">

📲 Order

</a>


</div>


</div>






<div class="product">


<div class="img-box">

<img src="HARSHITA.jpg">

</div>


<div class="product-content">


<h2>BANASKATHA SING</h2>


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


<div class="img-box">

<img src="product3.jpg">

</div>


<div class="product-content">


<h2>PRODUCT 3</h2>


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


<div class="img-box">

<img src="product4.jpg">

</div>


<div class="product-content">


<h2>PRODUCT 4</h2>


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





<script>


function searchProduct(){


let input=document
.getElementById("search")
.value
.toLowerCase();



let products=document
.querySelectorAll(".product");



products.forEach(function(product){


let name=product
.querySelector("h2")
.innerText
.toLowerCase();



if(name.includes(input)){


product.style.display="block";


}

else{


product.style.display="none";


}



});


}



</script>



</body>

</html>
