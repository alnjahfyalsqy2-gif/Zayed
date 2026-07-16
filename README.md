<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>تطبيقي</title>


<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}


body{

background:#2563eb;
color:white;
min-height:100vh;

}



header{

padding:25px;
text-align:center;

}



.logo{

font-size:35px;
font-weight:bold;

}



.container{

height:75vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;

}



h1{

font-size:45px;
margin-bottom:20px;

}



p{

font-size:20px;
line-height:1.8;

}



.time{

margin-top:25px;
background:rgba(255,255,255,0.15);
padding:15px 30px;
border-radius:20px;
font-size:18px;

}



.box{

margin-top:30px;
background:white;
color:#2563eb;
padding:25px;
border-radius:20px;
width:90%;
max-width:450px;

}



button{

margin:10px;
padding:12px 25px;
border:none;
border-radius:25px;
cursor:pointer;
font-size:16px;
font-weight:bold;

}



.lang{

background:#ffd700;

}



.app{

background:white;
color:#2563eb;

}



footer{

text-align:center;
padding:20px;

}



</style>


</head>


<body>



<header>

<div class="logo" id="title">

تطبيقي

</div>

</header>




<div class="container">


<h1 id="welcome">

أهلاً بك في موقعي

</h1>


<p id="description">

تطبيق حديث وسهل الاستخدام يقدم تجربة مميزة للمستخدم.

</p>



<div class="time">

<span id="date"></span>

<br>

<span id="clock"></span>

</div>




<div class="box">


<h2 id="boxTitle">

تحميل التطبيق

</h2>


<p id="boxText">

ضع رابط تطبيقك هنا لاحقاً

</p>



<button class="app" onclick="openApp()">

رابط التطبيق

</button>


<br>


<button class="lang" onclick="changeLanguage()">

English

</button>


</div>


</div>




<footer>

© 2026

</footer>





<script>


let arabic=true;



function updateTime(){

let now=new Date();


document.getElementById("date").innerHTML =
now.toLocaleDateString();


document.getElementById("clock").innerHTML =
now.toLocaleTimeString();


}



setInterval(updateTime,1000);

updateTime();






function openApp(){

// ضع رابط تطبيقك هنا لاحقاً

let appLink="";

if(appLink!=""){

window.open(appLink,"_blank");

}else{

alert("لم يتم إضافة رابط التطبيق بعد");

}

}







function changeLanguage(){


if(arabic){


document.documentElement.lang="en";

document.documentElement.dir="ltr";


document.getElementById("welcome").innerHTML=
"Welcome to my website";


document.getElementById("description").innerHTML=
"A modern and easy application experience.";


document.getElementById("boxTitle").innerHTML=
"Download App";


document.getElementById("boxText").innerHTML=
"Add your app link here later";


document.querySelector(".app").innerHTML=
"App Link";


document.querySelector(".lang").innerHTML=
"العربية";



arabic=false;



}else{


location.reload();


}



}



</script>



</body>

</html>
