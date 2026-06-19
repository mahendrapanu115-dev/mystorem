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

});
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
    width:90%;
    max-width:400px;
    padding:10px;
    border:1px solid #ccc;
    border-radius:8px;
    outline:none;
    font-size:14px;
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

<input type="text" id="searchInput" placeholder="🔍 Search products, brands...">

</div>
<header>
    <h1>🛒 Mera Online Store</h1>
    <p>Best Quality Products | Fast Delivery</p>
</header>

<div class="container">

<div class="products">

    <!-- PRODUCT 1 -->
    <div class="product">
        <img src="chana.jpg">
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
