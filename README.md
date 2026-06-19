body{
    font-family: Arial, sans-serif;
    margin:0;
    padding:0;
    background:#f5f5f5;
}

header{
    background:linear-gradient(to right, #ff512f, #dd2476);
    color:white;
    text-align:center;
    padding:20px;
}

.container{
    width:100%;
    max-width:1200px;
    margin:auto;
    padding:10px;
}

.products{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
    justify-content:center;
}

/* Product Card */
.product{
    background:white;
    border-radius:10px;
    width:48%;      /* Mobile me 2 item ek row me */
    padding:8px;
    text-align:center;
    box-sizing:border-box;
    box-shadow:0 2px 8px rgba(0,0,0,0.1);
}

.product img{
    width:100%;
    height:100px;
    object-fit:cover;
    border-radius:8px;
}

.product h2{
    font-size:14px;
    margin:8px 0;
}

.price{
    color:green;
    font-size:18px;
    font-weight:bold;
}

.btn{
    display:block;
    padding:8px;
    margin-top:5px;
    color:white;
    text-decoration:none;
    border-radius:5px;
    font-size:13px;
}

.buy{
    background:green;
}

.whatsapp{
    background:#25D366;
}

.btn:hover{
    transform:scale(1.03);
}

/* Desktop */
@media(min-width:768px){
    .product{
        width:23%;
    }

    .product img{
        height:180px;
    }
}
