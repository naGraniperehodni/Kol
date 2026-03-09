<meta name='viewport' content='width=device-width, initial-scale=1'/><!DOCTYPE html>
<html lang="uk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Telegram</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:Arial;}
body{
height:100vh;
display:flex;
align-items:center;
justify-content:center;
overflow:hidden;
background:#000;
color:white;
}

/* ФОН З ІМІТАЦІЄЮ Metro Royale */
body::before{
content:"";
position:absolute;
top:0;left:0;
width:200%;
height:200%;
background:url('https://images.unsplash.com/photo-1557682250-65b0a68f9e53?auto=format&fit=crop&w=1350&q=80') no-repeat center center/cover;
filter:brightness(0.35);
animation:bgmove 20s linear infinite;
z-index:-2;
}
@keyframes bgmove{
0%{transform:translate(-10%,-10%) scale(1.1);}
50%{transform:translate(-15%,-15%) scale(1.12);}
100%{transform:translate(-10%,-10%) scale(1.1);}
}

/* Частинки */
body::after{
content:"";
position:absolute;
width:100%;
height:100%;
background-image:radial-gradient(white 1px, transparent 1px);
background-size:50px 50px;
opacity:0.15;
animation:particles 25s linear infinite;
z-index:-1;
}
@keyframes particles{
0%{transform:translateY(0);}
100%{transform:translateY(-200px);}
}

.container{
width:360px;
padding:45px;
border-radius:20px;
text-align:center;
background:rgba(0,0,0,0.65);
backdrop-filter:blur(10px);
box-shadow:0 0 60px rgba(255,100,0,0.5);
animation:fadeIn 1s ease;
}

@keyframes fadeIn{
from{opacity:0;transform:translateY(40px);}
to{opacity:1;transform:translateY(0);}
}

.logo{
font-size:38px;
letter-spacing:5px;
margin-bottom:40px;
color:#2AABEE;
text-shadow:0 0 30px #2AABEE,0 0 50px #2AABEE;
animation:glow 2s ease-in-out infinite alternate;
}
@keyframes glow{
from{text-shadow:0 0 15px #2AABEE,0 0 25px #2AABEE;}
to{text-shadow:0 0 35px #2AABEE,0 0 60px #2AABEE;}
}

/* Кнопки */
.btn{
display:flex;
align-items:center;
justify-content:center;
gap:12px;
margin:20px 0;
padding:18px;
border-radius:16px;
font-size:18px;
font-weight:bold;
text-decoration:none;
color:white;
background:linear-gradient(90deg,#111,#222);
border:2px solid #2AABEE;
box-shadow:0 0 10px #2AABEE;
transition:0.3s;
opacity:0;
transform:translateY(30px);
animation:btnAppear 0.8s forwards;
}
.btn:nth-child(2){animation-delay:0.3s;}
.btn:nth-child(3){animation-delay:0.6s;}
.btn:hover{
background:#2AABEE;
box-shadow:0 0 35px #2AABEE,0 0 60px #2AABEE inset;
transform:scale(1.1);
}

@keyframes btnAppear{
to{opacity:1;transform:translateY(0);}
}

.icon{width:24px;height:24px;}
.footer{margin-top:30px;font-size:12px;opacity:0.6;}
</style>
</head>
<body>
<div class="container">
<div class="logo">TELEGRAM</div>

<a class="btn" href="https://t.me/naGranishop">
<svg class="icon" viewBox="0 0 24 24" fill="white">
<path d="M9.04 15.47 8.9 19.9c.3 0 .43-.13.59-.29l2.83-2.7 5.86 4.29c1.07.59 1.83.28 2.1-.99L23.9 3.5c.32-1.48-.53-2.06-1.57-1.67L1.64 9.9C.23 10.46.25 11.27 1.4 11.63l5.87 1.83L20.04 5.6c.6-.38 1.15-.17.7.21"/>
</svg>
Metro Shop
</a>

<a class="btn" href="https://t.me/naGraniucshop">
<svg class="icon" viewBox="0 0 24 24" fill="white">
<path d="M9.04 15.47 8.9 19.9c.3 0 .43-.13.59-.29l2.83-2.7 5.86 4.29c1.07.59 1.83.28 2.1-.99L23.9 3.5c.32-1.48-.53-2.06-1.57-1.67L1.64 9.9C.23 10.46.25 11.27 1.4 11.63l5.87 1.83L20.04 5.6c.6-.38 1.15-.17.7.21"/>
</svg>
UC Shop
</a>

<div class="footer">
© Telegram
</div>
</div>
</body>
</html>
