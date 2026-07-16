<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>موقعي الأول</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:linear-gradient(135deg,#0f172a,#2563eb);
color:white;
}

header{
display:flex;
justify-content:space-between;
align-items:center;
padding:20px 40px;
}

.logo{
font-size:28px;
font-weight:bold;
}

nav a{
color:white;
text-decoration:none;
margin:0 12px;
transition:.3s;
}

nav a:hover{
color:#ffd700;
}

.hero{
height:85vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
}

.hero h1{
font-size:45px;
margin-bottom:15px;
}

.hero p{
font-size:20px;
max-width:650px;
line-height:1.8;
}

.btn{
margin-top:30px;
padding:15px 35px;
background:#ffd700;
color:black;
text-decoration:none;
font-weight:bold;
border-radius:50px;
transition:.3s;
}

.btn:hover{
transform:scale(1.08);
}

.cards{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:20px;
padding:60px 20px;
}

.card{
background:white;
color:black;
width:260px;
padding:25px;
border-radius:15px;
text-align:center;
transition:.4s;
}

.card:hover{
transform:translateY(-10px);
}

footer{
padding:30px;
text-align:center;
opacity:.8;
}
</style>
</head>

<body>

<header>
<div class="logo">🚀 النجاح</div>

<nav>
<a href="#">الرئيسية</a>
<a href="#">الخدمات</a>
<a href="#">الأعمال</a>
<a href="#">تواصل</a>
</nav>
</header>

<section class="hero">
<h1>اصنع مستقبلك مع البرمجة</h1>

<p>
تعلم تطوير المواقع والتطبيقات وابدأ ببناء مشاريع احترافية وتحقيق دخل من الإنترنت.
</p>

<a class="btn" href="#">ابدأ الآن</a>
</section>

<section class="cards">

<div class="card">
<h2>سرعة</h2>
<p>تصميم سريع وحديث.</p>
</div>

<div class="card">
<h2>احترافية</h2>
<p>واجهة جميلة ومتجاوبة.</p>
</div>

<div class="card">
<h2>سهولة</h2>
<p>يعمل على الهاتف والكمبيوتر.</p>
</div>

</section>

<footer>
© 2026 جميع الحقوق محفوظة
</footer>

</body>
</html>
