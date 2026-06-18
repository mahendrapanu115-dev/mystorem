!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mera Online Store</title>

<style>
body{
    font-family: Arial, sans-serif;
    margin:0;
    padding:0;
    background:#f5f5f5;
}

/* PINK HEADER */
header{
    background:linear-gradient(to right, #ff512f, #dd2476);
    color:white;
    text-align:center;
    padding:25px;
}

/* PRODUCTS ROW */
.container{
    max-width:1000px;
    margin:auto;
    padding:20px;
}

.products{
    .products{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:10px;
    }
}

/* PRODUCT BOX */
.product{
    background:white;
    border-radius:10px;
    padding:15px;
    width:45%;
    text-align:center;
    box-shadow:0 0 10px rgba(0,0,0,0.1);
    box-sizing:border-box;
}
}

.product img{
    width:100%;
    height:180px;
    object-fit:cover;
    border-radius:10px;
}

.price{
    color:green;
    font-size:22px;
    font-weight:bold;
}

/* BUTTON STYLE */
.btn{
    display:inline-block;
    padding:10px 15px;
    margin:5px;
    color:white;
    text-decoration:none;
    border-radius:5px;
    transition:0.3s;   /* IMPORTANT */
}

/* BUTTON ZOOM EFFECT */
.btn:hover{
    transform:scale(1.1);
}

.buy{
    background:green;
}

.whatsapp{
    background:#25D366;
}
    
@media (max-width:768px){
    .product{
        width:45%;
        padding:10px;
    }

    .product img{
        height:120px;
    }
}
</head>

<body>

<header>
    <h1>🛒 Mera Online Store</h1>
    <p>Best Quality Products | Fast Delivery</p>
</header>

<div class="container">

<div class="products">

    <!-- PRODUCT 1 -->
    <div class="product">
        <img src="chana.jpg">
        <h2>ROASTED SING</h2>
        <p class="price">₹150</p>

        <a class="btn buy" href="upi://pay?pa=yourupi@upi&am=150">
        Pay Now
        </a>

        <a class="btn whatsapp" href="https://wa.me/919601393176 <text=Hello%20I%20want%20to%20buy%20Roasted%20Sing">
        Order
        </a>
    </div>

    <!-- PRODUCT 2 -->
    <div class="product">
        <img src="HARSHITA.jpg">
        <h2>BANASAKATHA SING</h2>
        <p class="price">₹120</p>

        <a class="btn buy" href="upi://pay?pa=yourupi@upi&am=120">
        Pay Now
        </a>

        <a class="btn whatsapp" href="https://wa.me/919601393176 <text=Hello%20I%20want%20to%20buy%20BANASKANTHA SING%20Sing">
        Order
        </a>
    </div>

</div>

</div>

</body>
</html>
