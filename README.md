<!DOCTYPE html>
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

header h1{
    animation: textPop 1s ease;
}

header p{
    animation: fadeUp 1.2s ease;
}

/* PREMIUM SEARCH BOX */
.search-wrapper{
    background:#fff;
    padding:12px;
    text-align:center;
    border-bottom:1px solid #eee;
}

.search-wrapper input{
    width:95%;
    max-width:450px;
    padding:12px 15px;
    border:none;
    outline:none;
    border-radius:30px;
    background:#f1f3f6;
    font-size:14px;
    box-shadow:0 2px 6px rgba(0,0,0,0.08);
    transition:0.3s;
}

.search-wrapper input:focus{
    background:#fff;
    box-shadow:0 4px 12px rgba(0,0,0,0.12);
    transform:scale(1.02);
}

/* ANIMATION */
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
    grid-template-columns:repeat(2, 1fr);
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

/* IMAGE */
.product img{
    width:100%;
    height:180px;
    object-fit:cover;
}

/* CONTENT */
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

<header>
    <h1>🛒 Mera Online Store</h1>
    <p>Best Quality Products | Fast Delivery</p>
</header>

<!-- SEARCH BOX -->
<div class="search-wrapper">
    <input type="text" id="searchInput" placeholder="🔍 Search products, brands...">
</div>

<div class="container">

<div class="products">

    <div class="product">
        <img src="chana.jpg">
        <div class="product-content">
            <h2>ROASTED SING</h2>
            <div class="price">₹150</div>
            <a class="btn buy">💳 Pay Now</a>
            <a class="btn whatsapp">📲 Order</a>
        </div>
    </div>

    <div class="product">
        <img src="HARSHITA.jpg">
        <div class="product-content">
            <h2>BANASKANTHA SING</h2>
            <div class="price">₹120</div>
            <a class="btn buy">💳 Pay Now</a>
            <a class="btn whatsapp">📲 Order</a>
        </div>
    </div>

    <div class="product">
        <img src="product3.jpg">
        <div class="product-content">
            <h2>PRODUCT 3</h2>
            <div class="price">₹180</div>
            <a class="btn buy">💳 Pay Now</a>
            <a class="btn whatsapp">📲 Order</a>
        </div>
    </div>

    <div class="product">
        <img src="product4.jpg">
        <div class="product-content">
            <h2>PRODUCT 4</h2>
            <div class="price">₹200</div>
            <a class="btn buy">💳 Pay Now</a>
            <a class="btn whatsapp">📲 Order</a>
        </div>
    </div>

</div>

</div>

<script>
const searchInput = document.getElementById("searchInput");
const products = document.querySelectorAll(".product");

searchInput.addEventListener("input", function(){

    let value = this.value.toLowerCase();

    products.forEach(function(item){
        let title = item.querySelector("h2").innerText.toLowerCase();

        if(title.includes(value)){
            item.style.display = "block";
        } else {
            item.style.display = "none";
        }
    });

});
</script>

</body>
</html>
