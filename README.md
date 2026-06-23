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
    font-family: Arial, sans-serif;
}

body{
    background:#f5f5f5;
}

/* SEARCH */

.search-wrapper{

    background:white;
    padding:12px;
    text-align:center;
}

        
/* HEADER */
header{
    background:#ffffff;
    color:#222;
    text-align:center;
    padding:18px;
    border-bottom:1px solid #eee;
}

header h1,
header p{
    text-align:center;
}
/* Title animation */
header h1{
    animation: textPop 1s ease;
}

/* subtitle animation */
header p{
    animation: fadeUp 1.2s ease;

}

.search-box input{

    width:95%;
    max-width:450px;

    padding:12px 15px;

    border:none;
    outline:none;

    border-radius:30px;

    background:#f1f3f6;

    font-size:14px;

    box-shadow:0 2px 6px rgba(0,0,0,.1);
}
/* CLEAN TITLE ANIMATION */
@keyframes textPop{
    0%{
        transform:translateY(-10px);
        opacity:0;
    }
    100%{
        transform:translateY(0);
        opacity:1;
    }
}

/* CLEAN TEXT ANIMATION */
@keyframes fadeUp{
    0%{
        opacity:0;
        transform:translateY(15px);
    }
    100%{
        opacity:1;
        transform:translateY(0);
    }
}
}

/* Title effect */
@keyframes textPop{
    0%{
        transform:scale(0.6);
        opacity:0;
        letter-spacing:5px;
    }
    100%{
        transform:scale(1);
        opacity:1;
        letter-spacing:0px;
    }
}

/* Subtitle effect */
@keyframes fadeUp{
    0%{
        opacity:0;
        transform:translateY(20px);
    }
    100%{
        opacity:1;
        transform:translateY(0);
    }
}


/* CONTAINER */
.container{
    width:100%;
    max-width:1200px;
    margin:auto;
    padding:10px;
}

/* PRODUCTS GRID */
.product-detail{

background:white;
border-radius:25px;
padding:30px;

display:grid;
grid-template-columns:1fr 1fr;

gap:40px;

}


.product-image img{

width:100%;
height:500px;

object-fit:cover;

border-radius:20px;

}


.thumbs{

display:flex;
gap:10px;
margin-top:15px;

}


.thumbs img{

width:70px;
height:70px;

object-fit:cover;

border-radius:10px;

cursor:pointer;

}



.detail h1{

font-size:38px;

}


.detail-price{

font-size:35px;
font-weight:bold;

margin:20px 0;

}


.action{

display:flex;
gap:15px;

}


.action a{

width:50%;
padding:15px;
text-align:center;

border-radius:10px;

text-decoration:none;

}


.pay{

background:black;
color:white;

}


.order{

border:1px solid #ccc;
color:black;

}


.tag{

display:inline-block;

background:#eee;

padding:10px 18px;

border-radius:25px;

margin:5px;

}



@media(max-width:800px){

.product-detail{

grid-template-columns:1fr;

}

}

/* TABLET */
@media (min-width:768px){
    .products{
        grid-template-columns:repeat(3, 1fr);
    }

    .product img{
        height:160px;
    }
}

/* LAPTOP */
@media (min-width:1024px){
    .products{
        grid-template-columns:repeat(4, 1fr);
    }
}
</style>
</head>

<body>

<!-- SEARCH -->

<div class="search-wrapper">

<input type="text" id="searchInput" placeholder="🔍 Search products, brands...">

</div>
<header>
    <h1>🛒 Mera Online Store</h1>
    <p>Best Quality Products | Fast Delivery</p>
</header>

<div class="container">

<div class="products">

    <!-- PRODUCT 1 -->
   <div class="product-detail">


<div class="product-image">


<img id="mainImg" src="divya.new.jpg">


<div class="thumbs">

<img onclick="changeImg(this.src)" src="divya.new.jpg">

<img onclick="changeImg(this.src)" src="HARSHITA.jpg">

<img onclick="changeImg(this.src)" src="product3.jpg">


</div>


</div>




<div class="detail">


<h1>
ROASTED SING
</h1>


<div class="detail-price">

₹150

</div>


<p>
+ ₹20 Shipping
</p>


<br>


<div class="action">

<a class="pay" href="#">
💳 Buy Now
</a>


<a class="order" href="#">
✉ Contact Seller
</a>

</div>



<br>


<div>

<span class="tag">🥜 Premium</span>

<span class="tag">✨ Fresh</span>

<span class="tag">📦 New</span>

</div>



<p style="margin-top:25px;color:#666">

Best quality roasted sing.
Fresh product with fast delivery.

</p>



<hr style="margin:25px 0">


<b>
Mera Online Store
</b>

<br>

⭐ ⭐ ⭐ ⭐ ⭐ 4.9




    <!-- PRODUCT 2 -->
       
<div class="product-image">


<img id="mainImg" src="HARSHITA.jpg">


<div class="thumbs">

<img onclick="changeImg(this.src)" src="HARSHITA.jpg">

<img onclick="changeImg(this.src)" src="HARSHITA.jpg">

<img onclick="changeImg(this.src)" src="product3.jpg">


</div>


</div>




<div class="detail">


<h1>
BANASKANTHA SING
</h1>


<div class="detail-price">

₹150

</div>


<p>
+ ₹20 Shipping
</p>


<br>


<div class="action">

<a class="pay" href="#">
💳 Buy Now
</a>


<a class="order" href="#">
✉ Contact Seller
</a>

</div>



<br>


<div>

<span class="tag">🥜 Premium</span>

<span class="tag">✨ Fresh</span>

<span class="tag">📦 New</span>

</div>



<p style="margin-top:25px;color:#666">

Best quality roasted sing.
Fresh product with fast delivery.

</p>



<hr style="margin:25px 0">


<b>
Mera Online Store
</b>

<br>

⭐ ⭐ ⭐ ⭐ ⭐ 4.9

</div>
<script>

function changeImg(src){

document.getElementById("mainImg").src=src;

}

</script>

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
