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

padding:15px;

text-align:center;

box-shadow:0 2px 8px #ccc;

}



.logo{

font-size:28px;

font-weight:bold;

color:#2874f0;

}



header p{

margin-top:5px;

color:#555;

}





/* SEARCH */


.search-box{

margin-top:15px;

display:flex;

justify-content:center;

gap:8px;

}



.search-box input{


width:65%;

max-width:400px;

padding:12px 15px;

border-radius:25px;

border:1px solid #ccc;

outline:none;

font-size:14px;


}




.search-box button{


padding:12px 22px;

border:none;

border-radius:25px;

background:#2874f0;

color:white;

font-weight:bold;

cursor:pointer;


}





/* MAIN */


.container{

padding:12px;

max-width:1200px;

margin:auto;


}





/* PRODUCTS */


.products{

display:grid;

grid-template-columns:repeat(2,1fr);

gap:12px;


}





/* CARD */


.product{


background:white;

border-radius:12px;

overflow:hidden;

box-shadow:0 3px 10px rgba(0,0,0,.15);

transition:.3s;


}



.product:hover{

transform:translateY(-5px);

}






/* IMAGE */


.image-box{


height:160px;

overflow:hidden;

display:flex;

align-items:center;

justify-content:center;


}




.image-box img{


width:100%;

height:100%;

object-fit:contain;

padding:10px;

transition:.5s;


}



.product:hover img{

transform:scale(1.1);

}







/* CONTENT */


.content{

padding:10px;

text-align:center;

}



.content h2{

font-size:14px;

height:35px;

}



.price{


font-size:20px;

font-weight:bold;

color:green;

margin:8px;


}




/* BUTTON */


.btn{


display:block;

text-decoration:none;

color:white;

padding:9px;

margin-top:7px;

border-radius:6px;

font-size:14px;


}


.pay{

background:#ff9f00;

}



.order{

background:#25D366;

}





/* FOOTER */


footer{

background:#222;

color:white;

text-align:center;

padding:15px;

margin-top:20px;

}







/* TABLET */


@media(min-width:700px){


.products{

grid-template-columns:repeat(3,1fr);

}



.image-box{

height:200px;

}



}







/* LAPTOP */


@media(min-width:1000px){


.products{

grid-template-columns:repeat(4,1fr);

}


.image-box{

height:230px;

}


}






</style>



</head>



<body>




<header>



<div class="logo">

🛒 mystorem

</div>


<p>

Best Quality Products | Fast Delivery

</p>




<div class="search-box">


<input type="text" 
id="search"
placeholder="Search product">



<button onclick="searchProduct()">

🔍 Search

</button>


</div>



</header>







<div class="container">


<div class="products" id="products">





<div class="product">


<div class="image-box">

<img src="chana.jpg">

</div>



<div class="content">


<h2>ROASTED SING</h2>


<div class="price">

₹150

</div>


<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>



</div>


</div>







<div class="product">


<div class="image-box">

<img src="HARSHITA.jpg">

</div>


<div class="content">


<h2>BANASKATHA SING</h2>


<div class="price">

₹120

</div>



<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>



</div>


</div>








<div class="product">


<div class="image-box">

<img src="product3.jpg">

</div>


<div class="content">


<h2>PRODUCT 3</h2>


<div class="price">

₹180

</div>



<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>



</div>


</div>








<div class="product">


<div class="image-box">

<img src="product4.jpg">

</div>


<div class="content">


<h2>PRODUCT 4</h2>


<div class="price">

₹200

</div>



<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>



</div>


</div>





</div>


</div>








<footer>

© 2026 Mera Online Store

</footer>







<script>


function searchProduct(){


let input=document
.getElementById("search")
.value
.toLowerCase();



let products=document
.querySelectorAll(".product");



products.forEach(function(item){


let name=item
.querySelector("h2")
.innerText
.toLowerCase();



if(name.includes(input)){


item.style.display="block";


}

else{


item.style.display="none";


}



});


}




</script>




</body>

</html>
