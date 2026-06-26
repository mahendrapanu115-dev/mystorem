<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Mera Store</title>


<style>


*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,Arial;
}



body{

background:#f5f5f5;

}



/* HEADER */


header{

background:white;

padding:20px;

text-align:center;

box-shadow:0 2px 10px #ddd;

}



.logo{

font-size:32px;

font-weight:bold;

color:#2874f0;

}



header p{

color:#555;

margin-top:5px;

}





/* SEARCH */


.search{

margin:20px auto;

display:flex;

justify-content:center;

gap:10px;

}



.search input{


width:400px;

padding:14px 20px;

border-radius:30px;

border:1px solid #ddd;

font-size:15px;


}



.search button{


padding:14px 30px;

border:none;

border-radius:30px;

background:#2874f0;

color:white;

font-weight:bold;

cursor:pointer;


}





/* PRODUCTS */


.container{

padding:20px;

}



.products{


display:grid;

grid-template-columns:repeat(4,1fr);

gap:18px;


}





/* CARD */


.product{


background:white;

border-radius:15px;

overflow:hidden;

box-shadow:0 5px 15px rgba(0,0,0,.12);

transition:.3s;


}



.product:hover{


transform:translateY(-8px);


}




/* IMAGE */


.image{


height:220px;

display:flex;

align-items:center;

justify-content:center;

overflow:hidden;


}



.image img{


width:100%;

height:100%;

object-fit:contain;

padding:15px;

transition:.5s;


}



.product:hover img{


transform:scale(1.1);


}




/* TEXT */


.content{

padding:15px;

text-align:center;

}



.content h2{

font-size:16px;

}



.price{


font-size:22px;

font-weight:bold;

color:green;

margin:10px;


}



/* BUTTON */


.btn{


display:block;

padding:11px;

margin-top:8px;

border-radius:8px;

color:white;

text-decoration:none;

font-weight:bold;


}



.buy{

background:#ff9f00;


}



.order{

background:#25D366;


}





/* FOOTER */


footer{


margin-top:30px;

background:#222;

color:white;

text-align:center;

padding:20px;


}




@media(max-width:900px){


.products{

grid-template-columns:repeat(2,1fr);

}



.search input{

width:220px;

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




<div class="search">


<input placeholder="Search product, brand">


<button>

🔍 Search

</button>


</div>


</header>





<div class="container">


<div class="products">





<div class="product">


<div class="image">

<img src="chana.jpg">

</div>


<div class="content">


<h2>ROASTED SING</h2>

<div class="price">

₹150

</div>


<a class="btn buy">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>


</div>


</div>






<div class="product">


<div class="image">

<img src="HARSHITA.jpg">

</div>


<div class="content">


<h2>BANASKATHA SING</h2>

<div class="price">

₹120

</div>


<a class="btn buy">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>


</div>


</div>







<div class="product">


<div class="image">

<img src="product3.jpg">

</div>


<div class="content">


<h2>PRODUCT 3</h2>

<div class="price">

₹180

</div>


<a class="btn buy">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>


</div>


</div>







<div class="product">


<div class="image">

<img src="product4.jpg">

</div>


<div class="content">


<h2>PRODUCT 4</h2>

<div class="price">

₹200

</div>


<a class="btn buy">

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

© 2026 Mera Online Store | All Rights Reserved

</footer>




</body>

</html>
