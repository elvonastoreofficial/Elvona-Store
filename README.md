<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Elvona Store — Coming Soon</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box}

body{
  min-height:100vh;
  background:
    radial-gradient(circle at top left, #fdecef, transparent 40%),
    radial-gradient(circle at bottom right, #f7e7d0, transparent 45%),
    #fff;
  display:flex;
  align-items:center;
  justify-content:center;
  font-family:'Inter',sans-serif;
  padding:20px;
  color:#333;
}

@keyframes pop {
  0%{transform:scale(0.9);opacity:0}
  100%{transform:scale(1);opacity:1}
}

.card{
  width:100%;
  max-width:460px;
  background:rgba(255,255,255,0.8);
  backdrop-filter:blur(20px);
  border-radius:28px;
  padding:36px 26px;
  box-shadow:0 40px 90px rgba(0,0,0,0.15);
  text-align:center;
  animation:pop 0.8s ease;
}

.brand{
  font-family:'Playfair Display',serif;
  font-size:38px;
  font-weight:700;
  background:linear-gradient(135deg,#c9a46c,#f1d6a3);
  -webkit-background-clip:text;
  -webkit-text-fill-color:transparent;
}

.sub{
  margin-top:6px;
  font-size:13px;
  color:#777;
}

.badge{
  margin:26px auto 16px;
  display:inline-block;
  padding:7px 18px;
  border-radius:50px;
  font-size:12px;
  background:linear-gradient(135deg,#c9a46c,#f1d6a3);
  color:#fff;
  letter-spacing:1px;
}

.title{
  font-family:'Playfair Display',serif;
  font-size:24px;
  margin-bottom:12px;
}

.text{
  font-size:14px;
  color:#666;
  line-height:1.7;
}

.products{
  display:flex;
  gap:12px;
  margin:26px 0;
}

.product{
  flex:1;
  background:#fff;
  border-radius:18px;
  padding:12px;
  box-shadow:0 12px 25px rgba(0,0,0,0.08);
}

.product img{
  width:100%;
  border-radius:14px;
}

.product span{
  display:block;
  margin-top:8px;
  font-size:12px;
  color:#555;
}

/* TIMER */
.timer{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:10px;
  margin:30px 0;
}

.box{
  background:#fff;
  border-radius:16px;
  padding:14px 6px;
  box-shadow:0 10px 25px rgba(0,0,0,0.08);
}

.box h2{
  font-size:22px;
  font-weight:700;
  color:#c9a46c;
}

.box span{
  font-size:11px;
  color:#888;
}

#live{
  display:none;
  margin:30px 0;
  font-family:'Playfair Display',serif;
  font-size:26px;
  color:#c9a46c;
}

.btn{
  display:block;
  padding:16px;
  border-radius:50px;
  background:linear-gradient(135deg,#c9a46c,#f1d6a3);
  color:#000;
  font-weight:600;
  text-decoration:none;
}

.email{
  margin-top:14px;
  font-size:12px;
  color:#888;
}

footer{
  margin-top:26px;
  font-size:11px;
  color:#aaa;
}
</style>
</head>

<body>

<div class="card">

  <div class="brand">Elvona Store</div>
  <div class="sub">Beauty • Cosmetics • Personal Care</div>

  <div class="badge">COMING SOON</div>

  <div class="title">A New Beauty Experience ✨</div>

  <div class="text">
    Discover skincare, beauty, and personal care  
    crafted for modern elegance.
  </div>

  <div class="products">
    <div class="product">
      <img src="https://images.unsplash.com/photo-1611930022073-b7a4ba5fcccd?w=400">
      <span>Luxury Skincare</span>
    </div>
    <div class="product">
      <img src="https://images.unsplash.com/photo-1620916566398-39f1143ab7be?w=400">
      <span>Personal Care</span>
    </div>
  </div>

  <div id="timer" class="timer">
    <div class="box"><h2 id="d">150</h2><span>Days</span></div>
    <div class="box"><h2 id="h">00</h2><span>Hours</span></div>
    <div class="box"><h2 id="m">00</h2><span>Minutes</span></div>
    <div class="box"><h2 id="s">00</h2><span>Seconds</span></div>
  </div>

  <div id="live">🚀 We’re Live!</div>

  <a class="btn" href="https://wa.me/message/X4Z4QP4LIRQFN1" target="_blank">
    Contact Us on WhatsApp
  </a>

  <div class="email">📧 elvonabusiness@gmail.com</div>

  <footer>© 2026 Elvona Store</footer>

</div>

<script>
const TOTAL_DAYS = 150;
const KEY = "elvona_150_days";

let end = localStorage.getItem(KEY);
if(!end){
  end = Date.now() + TOTAL_DAYS*24*60*60*1000;
  localStorage.setItem(KEY,end);
}
end = Number(end);

setInterval(()=>{
  const now = Date.now();
  const diff = end - now;

  if(diff <= 0){
    document.getElementById("timer").style.display="none";
    document.getElementById("live").style.display="block";
    return;
  }

  d.innerText = Math.floor(diff / 86400000);
  h.innerText = Math.floor(diff / 3600000) % 24;
  m.innerText = Math.floor(diff / 60000) % 60;
  s.innerText = Math.floor(diff / 1000) % 60;
},1000);
</script>

</body>
</html>
