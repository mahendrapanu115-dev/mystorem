<!DOCTYPE html>
<html>

<head>

<title>Nutri Roast | Premium Peanuts</title>


<style>


*{

margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;

}


body{

background:#160b05;

color:white;

overflow-x:hidden;

}



/* NAVBAR */


nav{

width:90%;

margin:25px auto;

padding:18px 35px;

background:#3b1b0c;

border-radius:50px;

display:flex;

justify-content:space-between;

align-items:center;

animation:top 1s;

}



.logo{

font-size:32px;

font-weight:bold;

color:#ffb703;

}



nav a{

color:white;

text-decoration:none;

margin:15px;

font-size:17px;

}




/* HERO */


.hero{

min-height:90vh;

width:100%;

display:flex;

align-items:center;

justify-content:space-around;

padding:50px 8%;

}



.text{

width:50%;

animation:left 1.2s;

}



.text h1{

font-size:70px;

line-height:1.1;

}



.text span{

color:#ffb703;

}



.text p{

font-size:22px;

color:#ddd;

margin:25px 0;

line-height:1.5;

}




button{

padding:18px 45px;

border:none;

border-radius:40px;

background:#ffb703;

font-size:18px;

font-weight:bold;

cursor:pointer;

transition:.4s;

}


button:hover{

transform:scale(1.15);

background:white;

}





/* PEANUT IMAGE */


.image{

width:45%;

position:relative;

display:flex;

justify-content:center;

}



.image img{

width:100%;

max-width:550px;

animation:float 3s infinite;

filter:drop-shadow(0 30px 40px black);

}




.circle{

position:absolute;

width:420px;

height:420px;

background:#ffb703;

border-radius:50%;

filter:blur(90px);

z-index:-1;

}





/* FLOAT PEANUT */


.peanut{

position:absolute;

font-size:45px;

animation:fall 8s infinite;

}


.p1{

left:10%;

}



.p2{

right:15%;

animation-delay:3s;

}



.p3{

left:50%;

animation-delay:5s;

}




/* FEATURES */


.features{

display:flex;

justify-content:center;

gap:30px;

padding:40px;

}



.card{

background:#3b1b0c;

padding:30px;

width:230px;

border-radius:25px;

text-align:center;

transition:.4s;

box-shadow:0 10px 30px black;

}



.card:hover{

transform:translateY(-15px);

background:#ffb703;

color:black;

}



.card h2{

font-size:40px;

}





/* ANIMATION */


@keyframes float{


0%,100%{

transform:translateY(0);

}


50%{

transform:translateY(-35px);

}


}




@keyframes fall{


0%{

top:-50px;

opacity:0;

}


50%{

opacity:1;

}


100%{

top:800px;

opacity:0;

transform:rotate(360deg);

}


}




@keyframes left{


from{

opacity:0;

transform:translateX(-100px);

}


to{

opacity:1;

transform:translateX(0);

}


}



@keyframes top{


from{

opacity:0;

transform:translateY(-80px);

}


to{

opacity:1;

transform:translateY(0);

}


}




/* MOBILE */


@media(max-width:800px){


nav{

flex-direction:column;

gap:15px;

}



.hero{

flex-direction:column;

text-align:center;

}



.text,.image{

width:100%;

}



.text h1{

font-size:42px;

}



.image img{

max-width:350px;

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

<a href="#">Shop</a>

<a href="#">Products</a>

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

Fresh crispy roasted peanuts.
Premium quality snacks with natural taste and fast delivery.

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






<div class="peanut p1">

🥜

</div>


<div class="peanut p2">

🥜

</div>


<div class="peanut p3">

🥜

</div>





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




