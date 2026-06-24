<!DOCTYPE html>
<html>
<head>

<title>Roasted Sing Premium</title>

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



/* HEADER */

header{

display:flex;
justify-content:space-between;
align-items:center;
padding:25px 8%;
background:#000;

}


.logo{

font-size:30px;
font-weight:bold;
color:#f5a623;

}



nav a{

color:white;
text-decoration:none;
margin-left:25px;

}




/* HERO */


.hero{

min-height:90vh;
display:flex;
align-items:center;
justify-content:space-around;
padding:40px;

}


.hero h1{

font-size:60px;

}


.hero span{

color:#f5a623;

}


.hero p{

font-size:20px;
color:#ccc;
margin:20px 0;

}



.btn{

display:inline-block;
background:#f5a623;
color:black;
padding:15px 40px;
border-radius:30px;
font-weight:bold;

}



.hero img{

width:420px;
animation:float 3s infinite;

}



@keyframes float{

50%{

transform:translateY(-25px);

}

}



/* PRODUCTS */


.products{

padding:60px 8%;
text-align:center;

}


.products h2{

font-size:45px;
margin-bottom:40px;

}



.card{

background:#111;
width:330px;
margin:auto;
padding:25px;
border-radius:25px;
border:1px solid #333;
transition:.4s;

}



.card:hover{

transform:translateY(-15px);
box-shadow:0 0 30px #f5a623;

}



.card img{

width:100%;
height:230px;
object-fit:contain;

}



.card h3{

font-size:28px;
margin:15px 0;

}



.price{

font-size:32px;
color:#f5a623;
font-weight:bold;

}



.card p{

color:#aaa;
margin:10px;

}



button{

background:#f5a623;
border:none;
padding:14px 35px;
border-radius:30px;
font-weight:bold;
cursor:pointer;

}




/* ANIMATION */

.hero-text{

animation:show 1s;

}


@keyframes show{

from{

opacity:0;
transform:translateX(-50px);

}

to{

opacity:1;
transform:translateX(0);

}

}




@media(max-width:700px){

.hero{

flex-direction:column;

}


.hero h1{

font-size:40px;

}


.hero img{

width:280px;

}

}


</style>

</head>


<body>



<header>


<div class="logo">

🥜 ROASTED SING

</div>


<nav>

<a href="#">Home</a>
<a href="#">Products</a>
<a href="#">Order</a>

</nav>


</header>




<section class="hero">


<div class="hero-text">


<h1>

Premium <span>Roasted Sing</span>

</h1>


<p>

Fresh roasted peanuts with rich crispy taste

</p>


<a class="btn">

Buy Now

</a>


</div>




<img <img src="https://cdn.pixabay.com/photo-2017/06/02/18/24/peanuts-2367598_1280.png">



</section>





<section class="products">


<h2>

Our Best Product

</h2>



<div class="card">


 <img src="https://images.unsplash.com/photo-1599599810694-57a9e5c8b4f2">


<h3>

Roasted Sing

</h3>


<p>

Premium Quality • 250 Gram

</p>


<div class="price">

₹150

</div>



<button>

Order Now

</button>


</div>



</section>



</body>
</html>
