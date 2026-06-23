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

.search-wrapper{
  width:100%;
  display:flex;
  justify-content:center;
}

.search-container{
  width:600px;
  height:55px;
  background:white;
  border-radius:35px;
  display:flex;
  align-items:center;
  padding:6px;
  box-shadow:0 8px 20px rgba(0,0,0,0.15);
}

.search-container input{
  flex:1;
  border:none;
  outline:none;
  padding-left:20px;
  font-size:16px;
}


/* pura button popup effect */
.search-btn{
  height:48px;
  padding:0 35px;
  border:none;
  border-radius:30px;
  background:#0d8cff;
  color:white;
  font-size:16px;
  font-weight:bold;
  cursor:pointer;

  transition:0.25s ease;
  box-shadow:0 6px 15px rgba(0,140,255,0.4);
}


/* mouse le jane par */
.search-btn:hover{
  transform:scale(1.08);
}


/* click karne par pura button bahar pop */
.search-btn:active{
  transform:scale(1.25);
  box-shadow:0 0 35px rgba(0,140,255,0.8);
}
}


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
.products{
    display:grid;
    grid-template-columns:repeat(2, 1fr); /* MOBILE = 2 per row */
    gap:10px;
}

/* PRODUCT CARD */
.product{
    background:#fff;
    border-radius:10px;
    overflow:hidden;
    box-shadow:0 2px 8px rgba(0,0,0,0.1);
    display:flex;
    flex-direction:column;
}

/* IMAGE FIX */
.product img{
    width:100%;
    height:180px;      /* पहले 140px था, अब बड़ा कर दिया */
    object-fit:cover;  /* सभी images same crop + same look */
    background:#fff;
}

/* TEXT AREA */
.product-content{
    padding:8px;
    text-align:center;
}

.product h2{
    font-size:13px;
    margin:5px 0;
}

.price{
    color:green;
    font-size:18px;
    font-weight:bold;
    margin-bottom:5px;
}

/* BUTTONS */
.btn{
    display:block;
    width:100%;
    padding:8px;
    margin-top:5px;
    text-decoration:none;
    color:white;
    border-radius:5px;
    font-size:13px;
}

.buy{
    background:green;
}

.whatsapp{
    background:#25D366;
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

    <!DOCTYPE html>
<html>
<head>
<title>Product Detail Page</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial,sans-serif;
}

body{
    background:#f5f5f5;
}


.container{
    max-width:1200px;
    margin:auto;
    padding:30px;
}


.card{
    background:white;
    border-radius:20px;
    padding:25px;
}


/* top */

.top{
    display:flex;
    justify-content:flex-end;
    gap:15px;
}

.icon{
    border:none;
    background:#eee;
    width:40px;
    height:40px;
    border-radius:50%;
    cursor:pointer;
}


/* main */

.main{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:40px;
    margin-top:20px;
}



/* images */

.big-img{
    width:100%;
    height:500px;
    border-radius:15px;
    overflow:hidden;
}

.big-img img{
    width:100%;
    height:100%;
    object-fit:cover;
}


.small-images{
    display:flex;
    gap:10px;
    margin-top:15px;
}


.small-images img{

    width:70px;
    height:70px;
    object-fit:cover;
    border-radius:10px;
    cursor:pointer;
}




/* details */

h1{
    font-size:35px;
}


.price{

font-size:35px;
font-weight:bold;
margin:20px 0;

}


.shipping{

color:gray;
font-size:14px;

}


.buttons{

display:flex;
gap:15px;
margin:25px 0;

}


button{

padding:15px 25px;
border-radius:10px;
border:none;
cursor:pointer;
font-size:16px;

}


.buy{

background:black;
color:white;
flex:1;

}


.contact{

background:white;
border:1px solid #ccc;
flex:1;

}


/* tags */


.tags{

display:flex;
gap:10px;
flex-wrap:wrap;
margin:20px 0;

}


.tag{

background:#eee;
padding:8px 15px;
border-radius:20px;

}



.desc{

color:#666;
line-height:1.6;

}


/* seller */

.seller{

margin-top:30px;
border-top:1px solid #ddd;
padding-top:20px;
display:flex;
align-items:center;
gap:15px;

}


.seller img{

width:60px;
height:60px;
border-radius:50%;

}


.rating{

color:#d99b00;

}


/* related */


.related{

margin-top:40px;

}


.products{

display:grid;
grid-template-columns:repeat(4,1fr);
gap:15px;

}


.products img{

width:100%;
height:200px;
object-fit:cover;
border-radius:15px;

}



/* mobile */

@media(max-width:800px){


.main{

grid-template-columns:1fr;

}


.products{

grid-template-columns:repeat(2,1fr);

}


.big-img{

height:350px;

}

}


</style>

</head>


<body>


<div class="container">

<div class="card">


<div class="top">

<button class="icon">♡</button>
<button class="icon">↗</button>

</div>



<div class="main">


<div>


<div class="big-img">

<img id="mainImage"
src="https://images.unsplash.com/photo-1591047139829-d91aecb6caea">

</div>


<div class="small-images">

<img onclick="changeImg(this.src)"
src="divya.jpg">


<img onclick="changeImg(this.src)"
src="divya.jpg">


<img onclick="changeImg(this.src)"
src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab">


</div>


</div>




<div>


<h1>
Lightweight Brown Bomber Jacket
</h1>


<div class="price">

€70

</div>


<span class="shipping">

+ €5.60 Shipping

</span>



<div class="buttons">

<button class="buy">
🛒 Buy Now
</button>


<button class="contact">
✉ Contact Seller
</button>

</div>




<div class="tags">

<div class="tag">🏷 Brown</div>

<div class="tag">📏 L Size</div>

<div class="tag">👩 Women</div>

<div class="tag">✨ New</div>


</div>




<p class="desc">

A stylish light bomber jacket, perfect for transitional seasons.
Made from breathable water resistant material with zip front,
side pockets and modern design.

</p>





<div class="seller">


<img src="https://i.pravatar.cc/150">


<div>


<br>

<span class="rating">
★★★★★ 4.9
</span>

</div>


</div>



</div>


</div>





<div class="related">



</div>


</div>



<script>


function changeImg(src){

document.getElementById("mainImage").src=src;

}


</script>


</body>

</html>

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
