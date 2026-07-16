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
display:flex;
justify-content:center;
}



.app{

width:100%;
max-width:500px;
min-height:100vh;
overflow:hidden;

}



header{

text-align:center;
padding:25px;

}



.logo{

font-size:32px;
font-weight:bold;

}



.container{

padding:20px;
text-align:center;

}



h1{

font-size:38px;
margin-top:70px;
margin-bottom:20px;

}



.description{

font-size:18px;
line-height:1.8;

}



.time{

margin:30px auto;
background:rgba(255,255,255,0.15);
padding:15px;
border-radius:20px;
width:90%;

}



.card{

background:white;
color:#2563eb;
padding:25px;
border-radius:25px;
margin-top:25px;

}



button{

border:none;
padding:13px 25px;
border-radius:30px;
margin-top:20px;
font-size:16px;
font-weight:bold;
cursor:pointer;

}



.download{

background:#2563eb;
color:white;

}



.language{

background:#ffd700;

}



footer{

text-align:center;
padding:20px;
font-size:14px;

}



</style>

</head>


<body>


<div class="app">



<header>

<div class="logo">
تطبيقي
</div>

</header>



<div class="container">



<h1 id="welcome">
أهلاً بك في موقعي
</h1>


<p class="description" id="desc">
تطبيق حديث وسهل الاستخدام يقدم تجربة مميزة للمستخدم.
</p>



<div class="time">

<div id="date"></div>

<div id="clock"></div>

</div>




<div class="card">


<h2 id="title">
تحميل التطبيق
</h2>


<p id="text">
يمكنك إضافة رابط التطبيق هنا لاحقاً.
</p>



<button class="download" onclick="downloadApp()" id="download">
رابط التطبيق
</button>


<br>


<button class="language" onclick="changeLang()" id="lang">
English
</button>



</div>



</div>



<footer>
© 2026
</footer>



</div>



<script>


let english=false;



function updateTime(){

let now=new Date();

document.getElementById("date").innerHTML=
now.toLocaleDateString();

document.getElementById("clock").innerHTML=
now.toLocaleTimeString();

}


setInterval(updateTime,1000);

updateTime();




function downloadApp(){

let link="";

if(link){

window.open(link);

}else{

alert("لم يتم إضافة رابط التطبيق بعد");

}

}




function changeLang(){


if(!english){


document.documentElement.lang="en";
document.documentElement.dir="ltr";


document.getElementById("welcome").innerHTML=
"Welcome to my website";


document.getElementById("desc").innerHTML=
"A modern and easy application experience.";


document.getElementById("title").innerHTML=
"Download App";


document.getElementById("text").innerHTML=
"You can add your app link here later.";


document.getElementById("download").innerHTML=
"App Link";


document.getElementById("lang").innerHTML=
"العربية";


english=true;


}else{


location.reload();


}


}


</script>


</body>

</html>
