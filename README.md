
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
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

/* Header */
header{
    background:linear-gradient(to right,#ff512f,#dd2476);
    color:white;
    text-align:center;
    padding:20px;
}

header h1{
    font-size:28px;
}

header p{
    margin-top:5px;
}

/* Container */
.container{
    max-width:1200px;
    margin:auto;
    padding:10px;
}

/* Product Grid */
.products{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
}

/* Product Card */
.product{
    width:calc(50% - 5px);
    background:white;
    border-radius:10px;
    overflow:hidden;
    box-shadow:0 2px 8px rgba(0,0,0,0.1);
}

.product img{
    width:100%;
    height:180px;       /* sab images ki same height */
    object-fit:contain; /* image cut nahi hogi */
    background:#fff;
    padding:5px;
}

.product-content{
    padding:10px;
    text-align:center;
}

.product h2{
    font-size:14px;
    margin-bottom:5px;
}

.price{
    color:green;
    font-size:20px;
    font-weight:bold;
    margin-bottom:10px;
}

/* Buttons */
.btn{
    display:block;
    width:100%;
    text-decoration:none;
    color:white;
    padding:10px;
    border-radius:5px;
    margin-top:5px;
    font-size:14px;
    transition:0.3s;
}

.btn:hover{
    opacity:0.9;
}

.buy{
    background:green;
}

.whatsapp{
    background:#25D366;
}

/* Desktop */
@media(min-width:768px){
    .product{
        width:calc(25% - 8px);
    }

    .product img{
        height:180px;
    }

    .product h2{
        font-size:18px;
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

        <!-- Product 1 -->
        <div class="product">
            <img src="chana.jpg" alt="Roasted Sing">

            <div class="product-content">
                <h2>ROASTED SING</h2>
                <p class="price">₹150</p>

                <a class="btn buy"
                href="upi://pay?pa=yourupi@upi&pn=MeraStore&am=150&cu=INR">
                💳 Pay Now
                </a>

                <a class="btn whatsapp"
                href="https://wa.me/919601393176?text=Hello%20I%20want%20to%20buy%20Roasted%20Sing">
                📲 Order on WhatsApp
                </a>
            </div>
        </div>

        <!-- Product 2 -->
        <div class="product">
            <img src="HARSHITA.jpg" alt="Banaskantha Sing">

            <div class="product-content">
                <h2>BANASKANTHA SING</h2>
                <p class="price">₹120</p>

                <a class="btn buy"
                href="upi://pay?pa=yourupi@upi&pn=MeraStore&am=120&cu=INR">
                💳 Pay Now
                </a>

                <a class="btn whatsapp"
                href="https://wa.me/919601393176?text=Hello%20I%20want%20to%20buy%20BANASKANTHA%20SING">
                📲 Order on WhatsApp
                </a>
            </div>
        </div>

        <!-- Product 3 -->
        <div class="product">
            <img src="product3.jpg" alt="Product 3">

            <div class="product-content">
                <h2>PRODUCT 3</h2>
                <p class="price">₹180</p>

                <a class="btn buy"
                href="upi://pay?pa=yourupi@upi&pn=MeraStore&am=180&cu=INR">
                💳 Pay Now
                </a>

                <a class="btn whatsapp"
                href="https://wa.me/919601393176?text=Hello%20I%20want%20to%20buy%20Product%203">
                📲 Order on WhatsApp
                </a>
            </div>
        </div>

        <!-- Product 4 -->
        <div class="product">
            <img src="product4.jpg" alt="Product 4">

            <div class="product-content">
                <h2>PRODUCT 4</h2>
                <p class="price">₹200</p>

                <a class="btn buy"
                href="upi://pay?pa=yourupi@upi&pn=MeraStore&am=200&cu=INR">
                💳 Pay Now
                </a>

                <a class="btn whatsapp"
                href="https://wa.me/919601393176?text=Hello%20I%20want%20to%20buy%20Product%204">
                📲 Order on WhatsApp
                </a>
            </div>
        </div>

    </div>

</div>

</body>
</html>
