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
    animation:textPop 1s ease;

}


header p{

    margin-top:5px;
    color:#555;
}



/* ANIMATION */

@keyframes textPop{

0%{
transform:scale(.7);
opacity:0;
}

100%{
transform:scale(1);
opacity:1;
}

}



/* CONTAINER */


.container{

    width:100%;
    max-width:1200px;
    margin:auto;
    padding:15px;

}



/* PRODUCT GRID */


.products{

display:grid;
grid-template-columns:repeat(2,1fr);
gap:15px;

}



/* PRODUCT CARD */


.product{

background:white;
border-radius:12px;
overflow:hidden;
box-shadow:0 3px 12px rgba(0,0,0,.15);

transition:.3s;

}


.product:hover{

transform:translateY(-5px);

}




/* FLIPKART STYLE IMAGE */


.product img{

width:100%;
height:260px;

object-fit:contain;

background:white;

padding:15px;

}




/* CONTENT */


.product-content{

padding:12px;
text-align:center;

}



.product h2{

font-size:15px;
margin-bottom:8px;

}




.price{

color:#008000;
font-size:22px;
font-weight:bold;
margin:8px 0;

}




/* BUTTON */


.btn{

display:block;
width:100%;

padding:10px;

margin-top:8px;

color:white;
text-decoration:none;

border-radius:6px;

font-size:14px;

}



.buy{

background:#ff9f00;

}



.whatsapp{

background:#25D366;

}



/* TABLET */

@media(min-width:768px){


.products{

grid-template-columns:repeat(3,1fr);

}


.product img{

height:230px;

}


}




/* LAPTOP */

@media(min-width:1024px){


.products{

grid-template-columns:repeat(4,1fr);

}


.product img{

height:260px;

}



}


</style>


</head>


<body>



<header>

<h1>🛒 Mera Online Store</h1>

<p>Best Quality Products | Fast Delivery</p>

</header>




<div class="container">


<div class="products">



<div class="product">


<img src="chana.jpg">


<div class="product-content">

<h2>ROASTED SING</h2>


<div class="price">

₹150

</div>



<a class="btn buy"
href="upi://pay?pa=yourupi@upi&am=150&cu=INR">

💳 Pay Now

</a>


<a class="btn whatsapp"
href="https://wa.me/919601393176?text=I%20want%20to%20buy%20Roasted%20Sing">

📲 Order

</a>


</div>


</div>





<div class="product">


<img src="HARSHITA.jpg">


<div class="product-content">


<h2>BANASKATHA SING</h2>


<div class="price">

₹120

</div>


<a class="btn buy"
href="upi://pay?pa=yourupi@upi&am=120&cu=INR">

💳 Pay Now

</a>



<a class="btn whatsapp"
href="https://wa.me/919601393176?text=I%20want%20Banaskantha%20Sing">

📲 Order

</a>


</div>


</div>






<div class="product">


<img src="product3.jpg">


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


<img src="product4.jpg">


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


</body>

</html>
