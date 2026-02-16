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
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Elvona Store | Coming Soon</title>

<!-- Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&family=Open+Sans:wght@400;500&display=swap" rel="stylesheet">

<style>
  :root {
    --bg: #fefefe;
    --primary: #5fa8a3;
    --text-main: #222222;
    --text-muted: #6b7280;
  }

  * { margin:0; padding:0; box-sizing:border-box; }
  body {
    font-family: 'Open Sans', sans-serif;
    background-color: var(--bg);
    color: var(--text-main);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    text-align: center;
    padding: 20px;
  }

  header h1 {
    font-family: 'Poppins', sans-serif;
    font-size: 3rem;
    font-weight: 600;
    margin-bottom: 10px;
  }

  header p {
    font-size: 1.2rem;
    color: var(--text-muted);
    margin-bottom: 40px;
  }

  /* Email Waitlist */
  .email-container {
    display: flex;
    max-width: 400px;
    width: 100%;
    margin: auto;
    margin-bottom: 30px;
  }

  .email-container input {
    flex: 1;
    padding: 12px 16px;
    border: 1px solid #ddd;
    border-radius: 8px 0 0 8px;
    outline: none;
    font-size: 0.95rem;
  }

  .email-container button {
    padding: 12px 20px;
    background-color: var(--primary);
    color: #fff;
    border: none;
    border-radius: 0 8px 8px 0;
    cursor: pointer;
    font-size: 0.95rem;
    font-weight: 500;
  }

  .email-container button:hover {
    opacity: 0.9;
  }

  /* Contact */
  .contact {
    font-size: 0.95rem;
    margin-top: 25px;
  }

  .contact a {
    color: var(--primary);
    text-decoration: none;
    margin: 0 10px;
  }

  footer {
    font-size: 0.85rem;
    color: var(--text-muted);
    margin-top: 50px;
  }

  /* Aura Effect (simple subtle animation) */
  .hero {
    position: relative;
    margin-bottom: 50px;
  }

  .hero::before {
    content: "";
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: radial-gradient(circle, rgba(95,168,163,0.15) 0%, transparent 70%);
    z-index: -1;
    animation: pulse 6s infinite;
  }

  @keyframes pulse {
    0% { transform: scale(1); opacity: 0.7; }
    50% { transform: scale(1.1); opacity: 1; }
    100% { transform: scale(1); opacity: 0.7; }
  }

  @media(max-width:480px){
    header h1 { font-size: 2.2rem; }
    header p { font-size: 1rem; }
  }

</style>
</head>
<body>

<div class="hero">
  <header>
    <h1>Elvona Store</h1>
    <p>Beauty, Cosmetic & Personal Care | Coming Soon</p>
  </header>
</div>

<div class="email-container">
  <input type="email" placeholder="Enter your email to join our waitlist">
  <button>Notify Me</button>
</div>

<div class="contact">
  <a href="https://wa.me/message/X4Z4QP4LIRQFN1" target="_blank">WhatsApp</a> |
  <a href="mailto:elvonabusiness@gmail.com">Email</a>
</div>

<footer>
  © 2026 Elvona Store • All Rights Reserved
</footer>

<!-- Start of LiveChat (www.livechat.com) code -->
<script>
    window.__lc = window.__lc || {};
    window.__lc.license = 19508807;
    window.__lc.integration_name = "manual_channels";
    window.__lc.product_name = "livechat";
    ;(function(n,t,c){function i(n){return e._h?e._h.apply(null,n):e._q.push(n)}var e={_q:[],_h:null,_v:"2.0",on:function(){i(["on",c.call(arguments)])},once:function(){i(["once",c.call(arguments)])},off:function(){i(["off",c.call(arguments)])},get:function(){if(!e._h)throw new Error("[LiveChatWidget] You can't use getters before load.");return i(["get",c.call(arguments)])},call:function(){i(["call",c.call(arguments)])},init:function(){var n=t.createElement("script");n.async=!0,n.type="text/javascript",n.src="https://cdn.livechatinc.com/tracking.js",t.head.appendChild(n)}};!n.__lc.asyncInit&&e.init(),n.LiveChatWidget=n.LiveChatWidget||e}(window,document,[].slice))
</script>
<noscript><a href="https://www.livechat.com/chat-with/19508807/" rel="nofollow">Chat with us</a>, powered by <a href="https://www.livechat.com/?welcome" rel="noopener nofollow" target="_blank">LiveChat</a></noscript>
<!-- End of LiveChat code -->
</body>
</html>
