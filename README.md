<!DOCTYPE html>
<html>
<head>

<title>Roasted Peanut Premium</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Poppins,Arial;
}


body{

background:#1b0d05;

color:white;

overflow-x:hidden;

}


/* NAVBAR */


nav{

width:90%;

margin:25px auto;

background:#3a1b0d;

border-radius:50px;

padding:18px 35px;

display:flex;

justify-content:space-between;

align-items:center;

animation:show 1s;

}



.logo{

font-size:30px;

font-weight:bold;

color:#ffb703;

}



nav a{

color:white;

text-decoration:none;

margin:15px;

}



/* HERO */


.hero{

display:flex;

align-items:center;

justify-content:center;

min-height:600px;

padding:40px;

gap:50px;

}



.text{

width:45%;

animation:left 1.2s;

}



.text h1{

font-size:65px;

line-height:1.1;

}


.text span{

color:#ffb703;

}



.text p{

font-size:20px;

color:#ddd;

margin:25px 0;

}



button{

background:#ffb703;

border:none;

padding:18px 40px;

border-radius:40px;

font-size:18px;

font-weight:bold;

cursor:pointer;

transition:.4s;

}


button:hover{

transform:scale(1.15);

background:white;

}





/* PRODUCT IMAGE */


.image{

width:40%;

position:relative;

}


.image img{

width:100%;

animation:updown 3s infinite;

filter:drop-shadow(0 20px 30px black);

}




/* floating */


.circle{

position:absolute;

width:350px;

height:350px;

background:#ffb703;

border-radius:50%;

z-index:-1;

right:0;

top:50px;

filter:blur(80px);

}





/* cards */


.cards{

display:flex;

justify-content:center;

gap:30px;

margin:40px;


}



.card{

background:#3a1b0d;

padding:30px;

border-radius:25px;

width:220px;

text-align:center;

transition:.4s;

}



.card:hover{

transform:translateY(-15px);

background:#ffb703;

color:black;

}



/* peanuts animation */


.peanut{

position:absolute;

font-size:40px;

animation:move 8s infinite;

}


.one{

left:10%;

}


.two{

right:20%;

animation-delay:3s;

}



@keyframes move{

0%{

top:-50px;

opacity:0;

}


50%{

opacity:1;

}


100%{

top:700px;

opacity:0;

transform:rotate(360deg);

}

}





@keyframes updown{


0%,100%{

transform:translateY(0);

}


50%{

transform:translateY(-30px);

}

}




@keyframes left{

from{

transform:translateX(-100px);

opacity:0;

}

to{

transform:translateX(0);

opacity:1;

}

}




@keyframes show{

from{

opacity:0;

transform:translateY(-50px);

}

to{

opacity:1;

}

}




@media(max-width:800px){


.hero{

flex-direction:column;

}


.text,.image{

width:90%;

}


.text h1{

font-size:40px;

}


.cards{

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

<a href="#">Shop</a>

<a href="#">About</a>

<a href="#">Contact</a>

</div>


</nav>





<section class="hero">



<div class="text">


<h1>

Real Taste Of

<span>

Roasted Peanuts

</span>

</h1>


<p>

Crunchy, fresh and healthy roasted peanuts.
Premium quality snacks delivered at your doorstep.

</p>



<button>

Order Now 🛒

</button>



</div>





<div class="image">


<div class="circle"></div>


<img src="https://pngimg.com/uploads/peanut/peanut_PNG7.png">


</div>



</section>





<div class="peanut one">

🥜

</div>


<div class="peanut two">

🥜

</div>




<section class="cards">


<div class="card">

<h2>🌱</h2>

<h3>Natural</h3>

<p>No chemicals</p>

</div>



<div class="card">

<h2>🔥</h2>

<h3>Fresh Roast</h3>

<p>Daily prepared</p>

</div>



<div class="card">

<h2>🚚</h2>

<h3>Fast Delivery</h3>

<p>Safe packing</p>

</div>


</section>




</body>
<!-- SEARCH -->
<div class="search-wrapper">
  <div class="search-container">

    <input id="mySearch" type="text" placeholder="product, brand">

    <button class="search-btn" onclick="searchNow()">
      🔍 Search
    </button>

  </div>
</div>


<script>
function searchNow(){

  let text = document.getElementById("mySearch").value;

  alert("Aapne search kiya: " + text);

}
</script>

<header>
    <h1>🛒 Mera Online Store</h1>
    <p>Best Quality Products | Fast Delivery</p>
</header>

<div class="container">

<div class="products">

    <!-- PRODUCT 1 -->
    <div class="product">
        <img src="divya.new.jpg">
        <div class="product-content">
            <h2>ROASTED SING</h2>
            <div class="price">₹150</div>

            <a class="btn buy" href="upi://pay?pa=yourupi@upi&am=150&cu=INR">💳 Pay Now</a>

            <a class="btn whatsapp" href="https://wa.me/919601393176?text=I%20want%20to%20buy%20Roasted%20Sing">
            📲 Order
            </a>
        </div>
    </div>

    <!-- PRODUCT 2 -->
    <div class="product">
        <img src="HARSHITA.jpg">
        <div class="product-content">
            <h2>BANASKATHA SING</h2>
            <div class="price">₹120</div>

            <a class="btn buy" href="upi://pay?pa=yourupi@upi&am=120&cu=INR">💳 Pay Now</a>

            <a class="btn whatsapp" href="https://wa.me/919601393176?text=I%20want%20to%20buy%20Banaskantha%20Sing">
            📲 Order
            </a>
        </div>
    </div>

    <!-- PRODUCT 3 -->
    <div class="product">
        <img src="product3.jpg">
        <div class="product-content">
            <h2>PRODUCT 3</h2>
            <div class="price">₹180</div>

            <a class="btn buy" href="upi://pay?pa=yourupi@upi&am=180&cu=INR">💳 Pay Now</a>

            <a class="btn whatsapp" href="https://wa.me/919601393176?text=I%20want%20Product%203">
            📲 Order
            </a>
        </div>
    </div>

    <!-- PRODUCT 4 -->
    <div class="product">
        <img src="product4.jpg">
        <div class="product-content">
            <h2>PRODUCT 4</h2>
            <div class="price">₹200</div>

            <a class="btn buy" href="upi://pay?pa=yourupi@upi&am=200&cu=INR">💳 Pay Now</a>

            <a class="btn whatsapp" href="https://wa.me/919601393176?text=I%20want%20Product%204">
            📲 Order
            </a>
        </div>
    </div>

</div>

</div>

</body>

</script>
</html>
</html>




