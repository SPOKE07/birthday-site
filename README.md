<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Happy Birthday My Love</title>

<style>
body{
margin:0;
font-family:'Segoe UI',sans-serif;
background:linear-gradient(#ffe6f2,#fff);
overflow-x:hidden;
text-align:center;
}

canvas{
position:fixed;
top:0;
left:0;
z-index:-1;
}

section{
padding:50px 20px;
min-height:100vh;
}

h1,h2{
color:#ff4d88;
}

.card{
background:white;
border-radius:20px;
padding:20px;
margin:20px auto;
max-width:400px;
box-shadow:0 0 15px rgba(0,0,0,.1);
}

button{
background:#ff4d88;
border:none;
padding:12px 20px;
border-radius:20px;
color:white;
font-size:16px;
}

.heart{
position:fixed;
color:pink;
animation:float 6s linear infinite;
}

@keyframes float{
0%{bottom:-20px;opacity:1}
100%{bottom:100%;opacity:0}
}

.balloon{
position:absolute;
font-size:40px;
animation:up 8s infinite;
}

@keyframes up{
0%{bottom:-50px}
100%{bottom:100%}
}

.gift{
font-size:80px;
animation:bounce 1s infinite alternate;
}

@keyframes bounce{
from{transform:translateY(0)}
to{transform:translateY(-15px)}
}

.timeline{
text-align:left;
max-width:400px;
margin:auto;
}

.timeline div{
margin:15px 0;
background:#fff0f6;
padding:10px;
border-radius:10px;
}

.sparkle{
position:fixed;
width:5px;
height:5px;
background:white;
border-radius:50%;
animation:spark 3s linear infinite;
}

@keyframes spark{
0%{opacity:1}
100%{opacity:0;transform:translateY(-200px)}
}
.cake-wrap{
display:flex;
justify-content:center;
margin-top:20px;
}

.cake{
position:relative;
width:220px;
}

.layer{
height:60px;
border-radius:10px;
background:linear-gradient(#fff,#f5c6d6);
margin-bottom:5px;
box-shadow:0 4px 6px rgba(0,0,0,.2);
}

.icing{
position:absolute;
top:0;
width:100%;
height:25px;
background:#ff9ac2;
border-radius:10px;
}

.drip{
position:absolute;
background:#ff9ac2;
width:20px;
height:30px;
border-radius:0 0 10px 10px;
}

.name{
position:absolute;
top:75px;
width:100%;
text-align:center;
font-size:24px;
color:#ff4d88;
font-weight:bold;
font-family:cursive;
}

.candle{
position:absolute;
top:-35px;
width:8px;
height:30px;
background:white;
left:50%;
transform:translateX(-50%);
}

.flame{
position:absolute;
top:-12px;
left:-4px;
width:16px;
height:16px;
background:orange;
border-radius:50%;
animation:flicker .5s infinite alternate;
}

@keyframes flicker{
from{transform:scale(1)}
to{transform:scale(.8)}
}

</style>
</head>

<body>

<canvas id="fireworks"></canvas>



<!-- Welcome -->
<section>
<h1>🎉🎂 Happy Birthday My Love 🎂🎉</h1>

<div class="card">
<p>To my jaan, my sweetheart, my everything — today is all about YOU 💕</p>
<p>You make my world brighter every single day.</p>
</div>

<div class="balloon" style="left:10%">🎈</div>
<div class="balloon" style="left:80%">🎈</div>

</section>

<section>
<h2>🎂 Pal Pal Dil Ke Paas 💗</h2>
<div class="card">
<p>Pal pal dil ke paas tum rehti ho…  
Jeevan meethi pyaas yeh kehti ho…  
Har shaam aankhon par tera aanchal lehraye…  
Har raat yaadon ki baaraat le aaye…</p>
</div>
</section>



<section>
<h2>🎂 Our Story 📖</h2>
<div class="card">
<p>💖 Our Bus Stop Love Story 💖

Class 9 ki queen thi main, swag full on,
Class 8 ka junior aaya — scene = cute version 😎
First day bola “Didi”, I was like bro chill,
Little did we know — dil hone wala tha kill 💘

Same bus, long route, daily wahi ride,
Mostly alone, talking side by side.
Main third seat queen, he sat just behind,
Taaki gossip ho full aur connection divine 😄

My hands were his favorite view,
Staring like — wow God really made you 😌Arm wrestling hua, obviously I lost,
But uske attitude pe hi ho gaya dil toast 💪😂

Gaane gaate, laughs unlimited pass,
But “Pal Pal Dil Ke Paas” was our forever class 🎶
Indirect crush confession, smooth sa style,
I teased him hard — beta wait for a while 😛

I said no, we’re too young babe,
Future ke chapters abhi blank page.
Then papa ki posting — Udaipur called,
Two years no contact… heart slightly stalled 💔

But destiny said — picture abhi baaki hai mere dost,
7 March 2024 — love officially post 💖
Now long distance, miles apart,
But WiFi strong and even stronger heart 🫶

From junior to jaan, what a glow up scene,
From “didi” to “baby” — ultimate upgrade machine 😭❤️
He’s my bestie, my comfort zone,
My home away from home, my ringtone tone 📱

So Happy Birthday Vikash, my jaan, my guy,
You’re my laugh, my peace, my favorite hi & bye 🎂
Pal Pal Dil Ke Paas, forever you stay,
Bus wali love story — now lifetime okay 💖</p>
</div>
</section>

<section>
<h2>🎂 Surprise 🎁</h2>

<button onclick="reveal()">Click for surprise</button>

<div id="surprise" style="display:none">

<div class="cake-wrap">
<div class="cake">

<div class="icing"></div>

<div class="drip" style="left:30px"></div>
<div class="drip" style="left:100px"></div>
<div class="drip" style="left:160px"></div>

<div class="layer"></div>
<div class="layer"></div>
<div class="layer"></div>

<div class="name">Vikash</div>

<div class="candle">
<div class="flame"></div>
</div>

</div>
</div>


<div class="card">
<p>My love,  
Happy Birthday jaaaannnnaaaa 😘😘♥️
meerraaa babyyy meraa baachhhaaa you know you are the most special most important person for me in this world baachhhaa 
gadheduuuu i cant even think of living without you , i haven't even thought what i am without you 
me , my present , my future , my life its all about you baachhhaaa  💕  
</p>
</div>

</div>
</section>

<script>

// Surprise
function reveal(){
document.getElementById("surprise").style.display="block";
}

// Hearts
setInterval(()=>{
let h=document.createElement("div");
h.className="heart";
h.innerHTML="❤️";
h.style.left=Math.random()*100+"%";
h.style.fontSize=Math.random()*20+10+"px";
document.body.appendChild(h);
setTimeout(()=>h.remove(),6000);
},500);

// Sparkles
setInterval(()=>{
let s=document.createElement("div");
s.className="sparkle";
s.style.left=Math.random()*100+"%";
s.style.bottom="0";
document.body.appendChild(s);
setTimeout(()=>s.remove(),3000);
},300);

// Fireworks
const canvas=document.getElementById("fireworks");
const ctx=canvas.getContext("2d");

function resize(){
canvas.width=window.innerWidth;
canvas.height=window.innerHeight;
}
resize();
window.onresize=resize;

let fireworks=[];

setInterval(()=>{
fireworks.push({
x:Math.random()*canvas.width,
y:canvas.height,
vx:(Math.random()-0.5)*3,
vy:-Math.random()*8-5,
life:60
});
},500);

function animate(){
ctx.clearRect(0,0,canvas.width,canvas.height);

fireworks.forEach((f,i)=>{
ctx.fillStyle="rgba(255,100,150,.8)";
ctx.beginPath();
ctx.arc(f.x,f.y,3,0,Math.PI*2);
ctx.fill();

f.x+=f.vx;
f.y+=f.vy;
f.life--;

if(f.life<=0)fireworks.splice(i,1);
});

requestAnimationFrame(animate);
}
animate();

</script>

</body>
</html>
# birthday-site
