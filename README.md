<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Roasted Sing Store</title>


<style>


*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial;
}


body{

background:#f5f5f5;

}



/* SEARCH */

.search-wrapper{

background:white;
padding:15px;
display:flex;
justify-content:center;

}


.search-container{

width:600px;
height:55px;
background:white;
display:flex;
border-radius:30px;
box-shadow:0 5px 20px #ccc;
overflow:hidden;

}


.search-container input{

flex:1;
border:none;
outline:none;
padding-left:20px;
font-size:16px;

}


.search-btn{

width:120px;
border:none;
background:#0d8cff;
color:white;
font-weight:bold;
cursor:pointer;

}




/* HEADER */


header{

background:white;
text-align:center;
padding:25px;
border-bottom:1px solid #ddd;

}


header h1{

color:#ff9900;
animation:title 1s;

}


@keyframes title{

from{

opacity:0;
transform:translateY(-20px);

}

to{

opacity:1;

}

}






/* PRODUCTS */


.container{

max-width:1200px;
margin:auto;
padding:20px;

}



.products{

display:grid;
grid-template-columns:repeat(4,1fr);
gap:15px;

}




.product{

background:white;
border-radius:15px;
overflow:hidden;
box-shadow:0 5px 15px #ddd;
transition:.3s;

}


.product:hover{

transform:translateY(-8px);

}






/* IMAGE SLIDER */


.slider{

height:220px;
position:relative;
overflow:hidden;
background:white;

}


.slider img{

width:100%;
height:220px;
object-fit:contain;
display:none;
cursor:pointer;

}


.slider img.active{

display:block;

}


.slider button{

position:absolute;
top:50%;
transform:translateY(-50%);
background:black;
color:white;
border:none;
width:35px;
height:35px;
border-radius:50%;

}



.prev{

left:5px;

}



.next{

right:5px;

}






/* DETAILS */


.content{

padding:12px;
text-align:center;

}


.content h2{

font-size:16px;

}


.price{

color:green;
font-size:22px;
font-weight:bold;
margin:8px;

}



.btn{

display:block;
padding:10px;
margin-top:8px;
border-radius:8px;
text-decoration:none;
color:white;

}



.pay{

background:#ff9900;

}


.order{

background:#25D366;

}







/* MOBILE */


@media(max-width:767px){


.products{

grid-template-columns:repeat(2,1fr);

}



.slider,
.slider img{

height:150px;

}



.content h2{

font-size:13px;

}


.btn{

font-size:12px;

}


}




</style>

</head>



<body>





<div class="search-wrapper">


<div class="search-container">


<input id="searchInput" placeholder="Search Product">


<button class="search-btn" onclick="searchProduct()">

🔍 Search

</button>


</div>


</div>







<header>

<h1>

🥜 Roasted Sing Store

</h1>

<p>

Fresh Quality | Fast Delivery

</p>


</header>






<div class="container">


<div class="products">





<!-- PRODUCT 1 -->


<div class="product">


<div class="slider">


<img class="active" src="divya.new.jpg">

<img src="sing2.jpg">

<img src="sing3.jpg">

<img src="sing4.jpg">

<img src="sing5.jpg">


<button class="prev" onclick="changeSlide(-1,this)">
❮
</button>


<button class="next" onclick="changeSlide(1,this)">
❯
</button>


</div>




<div class="content">


<h2>

ROASTED SING

</h2>


<div class="price">

₹150

</div>



<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>


</div>


</div>









<!-- PRODUCT 2 -->


<div class="product">


<div class="slider">


<img class="active" src="HARSHITA.jpg">

<img src="sing6.jpg">

<img src="sing7.jpg">

<img src="sing8.jpg">

<img src="sing9.jpg">


<button class="prev" onclick="changeSlide(-1,this)">
❮
</button>


<button class="next" onclick="changeSlide(1,this)">
❯
</button>


</div>





<div class="content">


<h2>

BANASKATHA SING

</h2>


<div class="price">

₹120

</div>


<a class="btn pay">

💳 Pay Now

</a>


<a class="btn order">

📲 Order

</a>


</div>


</div>







</div>

</div>







<script>



// SEARCH FUNCTION


function searchProduct(){


let value=document
.getElementById("searchInput")
.value
.toLowerCase();



let products=document.querySelectorAll(".product");



products.forEach(product=>{


let text=product.innerText.toLowerCase();



if(text.includes(value)){


product.style.display="block";


}

else{


product.style.display="none";


}



});


}






// MANUAL SLIDE


function changeSlide(direction,btn){


let slider=btn.parentElement;


let images=slider.querySelectorAll("img");


let index=0;



images.forEach((img,i)=>{


if(img.classList.contains("active")){

index=i;

}


});



images[index].classList.remove("active");


index=index+direction;



if(index>=images.length){

index=0;

}



if(index<0){

index=images.length-1;

}



images[index].classList.add("active");



}







// AUTO SLIDE


setInterval(()=>{


document.querySelectorAll(".slider")
.forEach(slider=>{


let images=slider.querySelectorAll("img");


let index=0;



images.forEach((img,i)=>{


if(img.classList.contains("active")){

index=i;

}


});



images[index].classList.remove("active");


index++;


if(index>=images.length){

index=0;

}


images[index].classList.add("active");



});



},3000);



</script>




</body>

</html>
