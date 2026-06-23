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

<div class="product">
        <img src="divya.jpg"

</div>


<div class="small-images">

<div class="product">
        <img src="HARSHITA.jpg"

<div class="product">
        <img src="divya.jpg"


<div class="product">
        <img src="HARSHITA.jpg"

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

<b>Maria Johansson</b>

<br>

<span class="rating">
★★★★★ 4.9
</span>

</div>


</div>



</div>


</div>





<div class="related">


<h2>
You might also like
</h2>


<div class="products">


<img src="https://images.unsplash.com/photo-1525507119028-ed4c629a60a3">


<img src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab">


<img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30">


<img src="https://images.unsplash.com/photo-1519741497674-611481863552">


</div>


</div>



</div>


</div>



<script>


function changeImg(src){

document.getElementById("mainImage").src=src;

}


</script>


</body>

</html>
