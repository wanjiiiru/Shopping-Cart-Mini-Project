# Shopping-Cart-Mini-Project
<html>
<head>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap" rel="stylesheet">
<script src="https://kit.fontawesome.com/1439b4882a.js" crossorigin="anonymous"></script>
<style>
 *{  
margin: 0;  
padding: 0;  
box-sizing: border-box;  
 }  
header{
background-color:#5C5CFF;
height:60px;
}
h1{
font-family: 'Dancing Script', cursive;
color:white;
padding-top:10px;
padding-left:20px;
 }
.search{
padding-top:15px;
}
.column1{
float:left;
padding:10px;
height:100px;
}
.left
{
width:40%;
}
.right
{
width:60%;
padding-left:15px;
}
.row1:after{
content:"";
display:table;
clear:both;
}
.search{
padding-top:0px;
height:50px;
}
a:visited{
color:black;
}
a:hover{
color:red;
}
input[type=text] {
  padding: 10px;
  font-size: 17px;
  border: 1px solid grey;
  float: left;
  width: 80%;
  background: #f1f1f1;
}
button {
  float: left;
  width: 10%;
  padding: 10px;
  background: #2196F3;
height:42px;
  color: white;
  font-size: 17px;
  border: 1px solid grey;
  border-left: none; /* Prevent double borders */
  cursor: pointer;
}
button:hover {
  background: #0b7dda;
}
.navbar{
background-color:#5C5CFF;
margin-top:15px;
height:60px;
text-align:center;
}
a:link
{
text-decoration:none;
font-size:25px;
color:black;
}
a:visited{
color:#483531;
}
a:hover{
text-decoration:underline;
color:red;
}
#sect2
{
margin-top:-30px;
margin-bottom:-130px;
padding:0;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
}
.slider{
width:800px;
height:500px;
border-radius:10px;
overflow:hidden;
}
.slides{
width:500%;
height;500px;
display:flex;
}
.slides input{
display:none;
}
.slide{
width:20%;
transition:2s;
}
.slide img{
width:800px;
height:400px;
}
.navigation-manual
{
position:absolute;
width:800px;
margin-top:-40px;
display:flex;
justify-content:center;
}
.manual-btn{
border:2px solid #5C5CFF;
padding:5px;
border-radius:10px;
cursor:pointer;
transition:1s;
}
.manual-btn:not(:last-child){
margin-right:40px;
}
.manual-btn:hover{
background:#5C5CFF;
}
#radio1:checked ~.first{
margin-left:0;
}
#radio2:checked ~.first{
margin-left:-20%;
}
#radio3:checked ~.first{
margin-left:-40%;
}
#radio4:checked ~.first{
margin-left:-60%;
}
#radio5:checked ~.first{
margin-left:-80%;
}
.navigation-auto{
position:absolute;
width:800px;
display:flex;
justify-content:center;
margin-top:460px;
}
.navigation-auto div{
transition:3s;
}
.column{
float: left;
  width:40%;
  padding: 5px;
}
.container{
font-size:30px;
font-weight:bold;
}
.copy{
background-color:#5C5CFF;
padding-top:20px;
margin-top:1180px;
text-align:center;
height:230px;
font-weight:bold;
font-size:20px;
color:white;
}
.foot{
font-weight:lighter;
} 
body{
background-color:B1A189;
}
.title{
text-align:center;
color:black;
font-weight:bold;
font-size:30px;
background-color:white;
height:50px;
margin-bottom:25px;
padding-top:10px;
font-family: 'Dancing Script', cursive;
}
</style>
</head>
<body>
<header>
<div class="row1">
<div class="column1 left">
<h1>STAHI FURNITURE</h1>
</div>
<div class="column1 right">
<div class="search">  
<a href=""><input type="text" placeholder="search..." id="input">
<button type="submit"><i class="fa-sharp fa-solid fa-magnifying-glass"></i></button></a>  
</div>
</div>
</div>
</header>
<nav class="navbar">
<a href="login.html">Login<i class="fa-solid fa-arrow-right-to-bracket"></i></a> &nbsp &nbsp &nbsp &nbsp
<a href="reg.html"><i class="fa-solid fa-user-plus"></i>Sign up</a>&nbsp &nbsp &nbsp &nbsp
<a href="gallery.html"><i class="fa-solid fa-camera"></i>Gallery</a>&nbsp &nbsp &nbsp &nbsp
<a href="contactus.html">Contact Us<i class="fa-sharp fa-solid fa-phone"></i></a> &nbsp &nbsp &nbsp
<a href="cart.html"><i class="fa-solid fa-cart-shopping"></i></a>
</nav>
<section id="sect2">
<div class="slider">
<div class="slides">
<input type="radio" name="radio-btn" id="radio1">
<input type="radio" name="radio-btn" id="radio2">
<input type="radio" name="radio-btn" id="radio3">
<input type="radio" name="radio-btn" id="radio4">
<input type="radio" name="radio-btn" id="radio5">
<div class="slide first">
<img src="pexel8.jpg"  >
</div>
<div class="slide">
<img src="bed22.jpg" >
</div>
<div class="slide">
<img src="office66.jpg">
</div>
<div class="slide">
<img src="dining3.jpg">
</div>
<div class="slide">
<img src="outdoor11.jpg">
</div>
<div class="navigation-auto">
<div class="auto-btn1"></div>
<div class="auto-btn2"></div>
<div class="auto-btn3"></div>
<div class="auto-btn4"></div>
<div class="auto-btn5"></div>
</div>
</div>
<div class="navigation-manual">
<label for="radio1" class="manual-btn"></label>
<label for="radio2" class="manual-btn"></label>
<label for="radio3" class="manual-btn"></label>
<label for="radio4" class="manual-btn"></label>
<label for="radio5" class="manual-btn"></label>
</div>
</div>
<script>
var counter=1;
setInterval(function() {
document.getElementById('radio' + counter).checked=true;
counter ++;
if(counter>4){
counter=1;
}
},3000);
</script>
</section>
<div class="title">SHOP ONLINE</div>
<div class="container">
<div class="row">
<div class="column">
<a href="living.html"><img src="pexel25.jpg" width="350" height="350"></a>
<a href="living.html"><div class="livingr">Living Room</div></a>
</div>
<div class="column">
<a href="default.asp"><img src="bed.jpg" width="350" height="350"></a>
<a href="bedroom.html"><div class="bedr">Bedroom</div></a>
</div>
</div>
<div class="row">
<div class="column">
<a href="default.asp"><img src="office.jpg" width="350" height="350"></a>
<a href="office.html"><div class="off">Office</div></a>
</div>
<div class="column">
<a href="default.asp"><img src="dining3.jpg" width="350" height="350"></a>
<a href="dining.html"><div class="dine">Dining</div></a>
</div>
</div>
<div class="row">
<div class="column">
<a href="default.asp"><img src="outdoor10.jpg" width="350" height="350"></a>
<a href="outdoor.html"><div class="out">Outdoor</div></a>
</div>
</div>
</div>
<footer class="copy">
<p>Connect with us</p>
<center><table> <tr><td><i class="fa-brands fa-twitter"></i></td>
<td><i class="fa-brands fa-instagram"></i></td>
<td><i class="fa-brands fa-facebook"></i></td>
<td><i class="fa-brands fa-youtube"></i></td></tr>
</table>
<table><tr><td>GARGEN CITY SHOWROOM<td></td></tr>
<center><p>Website by Wanjiru</p></center>
</footer>
</body>
</html>
