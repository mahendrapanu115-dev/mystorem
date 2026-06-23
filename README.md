<!DOCTYPE html>
<html>

<head>

<title>Roasted Peanut Brand</title>


<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}


body{

background:#120804;
color:white;
overflow-x:hidden;

}


/* NAV */

nav{

height:80px;

width:100%;

padding:0 8%;

display:flex;

align-items:center;

justify-content:space-between;

background:#1d0d06;

}


.logo{

font-size:32px;

font-weight:bold;

color:#ffb000;

}


nav a{

color:white;

text-decoration:none;

margin-left:30px;

}



/* HERO FULL */

.hero{

min-height:100vh;

width:100%;

display:flex;

align-items:center;

justify-content:space-around;

padding:50px 8%;

}



.content{

width:45%;

}



.content h1{

font-size:75px;

line-height:1;

}


.content span{

color:#ffb000;

}



.content p{

font-size:22px;

color:#ddd;

margin:30px 0;

line-height:1.6;

}



.btn{

display:inline-block;

padding:18px 45px;

background:#ffb000;

color:black;

border-radius:50px;

font-weight:bold;

font-size:18px;

}



/* IMAGE */

.product-img{

width:45%;

text-align:center;

position:relative;

}



.product-img img{

width:500px;

max-width:100%;

animation:float 3s infinite;

}



.glow{

position:absolute;

width:450px;

height:450px;

background:#ffb000;

filter:blur(120px);

opacity:.5;

top:50px;

z-index:-1;

}





/* FEATURES */


.features{

display:flex;

justify-content:center;

gap:30px;

padding:50px;

}



.card{

background:#32170b;

width:250px;

padding:35px;

border-radius:25px;

text-align:center;

transition:.4s;

}



.card:hover{

transform:translateY(-15px);

background:#ffb000;

color:black;

}




/* ANIMATION */


@keyframes float{

0%,100%{

transform:translateY(0);

}

50%{

transform:translateY(-30px);

}

}





@media(max-width:900px){


.hero{

flex-direction:column;

text-align:center;

}



.content,
.product-img{

width:100%;

}



.content h1{

font-size:45px;

}



.features{

flex-direction:column;

align-items:center;

}


}



</style>


</head>


<body>



<nav>


<div class="logo">

🥜 Nutri Roast

</div>


<div>

<a href="#">Home</a>

<a href="#">Products</a>

<a href="#">Contact</a>

</div>


</nav>




<section class="hero">



<div class="content">


<h1>

Premium

<span>

Roasted Peanuts

</span>

</h1>


<p>

Crunchy taste, fresh roasting and premium quality peanuts.
Healthy snack delivered directly to your home.

</p>



<a class="btn">

Order Now 🛒

</a>


</div>





<div class="product-img">


<div class="glow"></div>


<img src="https://pngimg.com/uploads/peanut/peanut_PNG7.png">


</div>



</section>




<section class="features">


<div class="card">

<h2>🌱</h2>

<h3>100% Natural</h3>

<p>No Chemicals</p>

</div>



<div class="card">

<h2>🔥</h2>

<h3>Fresh Roast</h3>

<p>Daily Fresh</p>

</div>



<div class="card">

<h2>🚚</h2>

<h3>Fast Delivery</h3>

<p>Safe Packing</p>

</div>


</section>




</body>

</html>
