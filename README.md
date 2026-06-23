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


</section>




</body>

</html>


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




