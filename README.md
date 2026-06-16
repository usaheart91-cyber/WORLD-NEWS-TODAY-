<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>WORLD NEWS TODAY</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:#0f172a;
color:white;
}

header{
background:#111827;
padding:15px 20px;
position:sticky;
top:0;
z-index:1000;
}

.nav{
display:flex;
justify-content:space-between;
align-items:center;
}

.logo{
font-size:28px;
font-weight:bold;
}

.logo span{
color:#3b82f6;
}

.menu a{
color:white;
text-decoration:none;
margin-left:15px;
}

.hero{
height:60vh;
background:url('https://picsum.photos/1200/700') center/cover;
display:flex;
align-items:flex-end;
padding:30px;
}

.hero-box{
background:rgba(0,0,0,.7);
padding:20px;
border-radius:10px;
max-width:700px;
}

.hero h1{
font-size:40px;
margin-bottom:10px;
}

.breaking{
background:#2563eb;
padding:10px;
font-weight:bold;
text-align:center;
}

.container{
padding:25px;
}

.section-title{
margin-bottom:20px;
font-size:30px;
}

.news-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:20px;
}

.card{
background:#1e293b;
border-radius:15px;
overflow:hidden;
transition:.3s;
}

.card:hover{
transform:translateY(-5px);
}

.card img{
width:100%;
height:180px;
object-fit:cover;
}

.card-content{
padding:15px;
}

.card-content h3{
margin-bottom:10px;
}

.card-content p{
color:#cbd5e1;
margin-bottom:10px;
}

.btn{
background:#3b82f6;
color:white;
border:none;
padding:10px 15px;
border-radius:8px;
cursor:pointer;
}

.categories{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(150px,1fr));
gap:15px;
margin-top:30px;
}

.category{
background:#1e293b;
padding:20px;
text-align:center;
border-radius:10px;
font-weight:bold;
}

.search{
margin-top:15px;
}

.search input{
width:100%;
padding:12px;
border:none;
border-radius:10px;
}

footer{
margin-top:40px;
padding:30px;
background:#111827;
text-align:center;
}

@media(max-width:768px){
.hero h1{
font-size:28px;
}
.menu{
display:none;
}
}
</style>
</head>
<body>

<header>

<div class="nav">

<div class="logo">
WORLD <span>NEWS</span> TODAY
</div>

<div class="menu">
<a href="#">World</a>
<a href="#">Tech</a>
<a href="#">Business</a>
<a href="#">Sports</a>
<a href="#">Science</a>
</div>

</div>

<div class="search">
<input type="text" id="searchBox" placeholder="Search News...">
</div>

</header>

<div class="breaking">
🔥 LIVE: Global News • Technology • Business • Sports • Science
</div>

<section class="hero">

<div class="hero-box">

<h1>Global Headlines That Matter</h1>

<p>
Latest updates from around the world.
Stay informed with trusted reporting.
</p>

</div>

</section>

<div class="container">

<h2 class="section-title">
Latest News
</h2>

<div class="news-grid" id="newsGrid">

<div class="card news-item">
<img src="https://picsum.photos/500/300?1">
<div class="card-content">
<h3>World Leaders Meet</h3>
<p>Major summit discusses economy and international relations.</p>
<button class="btn">Read More</button>
</div>
</div>

<div class="card news-item">
<img src="https://picsum.photos/500/300?2">
<div class="card-content">
<h3>AI Technology Boom</h3>
<p>Artificial intelligence continues to transform industries.</p>
<button class="btn">Read More</button>
</div>
</div>

<div class="card news-item">
<img src="https://picsum.photos/500/300?3">
<div class="card-content">
<h3>Global Markets Rise</h3>
<p>Investors react positively to economic updates.</p>
<button class="btn">Read More</button>
</div>
</div>

<div class="card news-item">
<img src="https://picsum.photos/500/300?4">
<div class="card-content">
<h3>Space Discovery</h3>
<p>Scientists announce exciting findings from new missions.</p>
<button class="btn">Read More</button>
</div>
</div>

<div class="card news-item">
<img src="https://picsum.photos/500/300?5">
<div class="card-content">
<h3>Sports Championship</h3>
<p>Fans celebrate a thrilling final match.</p>
<button class="btn">Read More</button>
</div>
</div>

<div class="card news-item">
<img src="https://picsum.photos/500/300?6">
<div class="card-content">
<h3>Business Growth</h3>
<p>Companies report strong quarterly performance.</p>
<button class="btn">Read More</button>
</div>
</div>

</div>

<h2 class="section-title" style="margin-top:40px;">
Categories
</h2>

<div class="categories">

<div class="category">🌍 World</div>
<div class="category">💻 Technology</div>
<div class="category">💰 Business</div>
<div class="category">⚽ Sports</div>
<div class="category">🔬 Science</div>
<div class="category">🤖 AI</div>

</div>

</div>

<footer>

<h2>WORLD NEWS TODAY</h2>

<p>
Professional News Portal
</p>

<br>

<p>
© 2026 All Rights Reserved
</p>

</footer>

<script>

const searchBox =
document.getElementById("searchBox");

searchBox.addEventListener("keyup",()=>{

let filter =
searchBox.value.toLowerCase();

let cards =
document.querySelectorAll(".news-item");

cards.forEach(card=>{

let text =
card.innerText.toLowerCase();

card.style.display =
text.includes(filter)
? "block"
: "none";

});

});

</script>

</body>
</html>
