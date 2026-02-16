<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Elvona Store | Coming Soon</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&family=Open+Sans:wght@400;500&display=swap" rel="stylesheet">

<style>
:root {
  --bg: #fefefe;
  --primary: #5fa8a3;
  --text-main: #222;
  --text-muted: #6b7280;
}

* { margin:0; padding:0; box-sizing:border-box; }

body {
  font-family: 'Open Sans', sans-serif;
  background-color: var(--bg);
  color: var(--text-main);
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  min-height:100vh;
  text-align:center;
  padding:20px;
}

.hero {
  position:relative;
  margin-bottom:50px;
}

.hero::before {
  content:"";
  position:absolute;
  top:-50%;
  left:-50%;
  width:200%;
  height:200%;
  background:radial-gradient(circle, rgba(95,168,163,0.15) 0%, transparent 70%);
  z-index:-1;
  animation:pulse 6s infinite;
}

@keyframes pulse {
  0% { transform:scale(1); opacity:0.7; }
  50% { transform:scale(1.1); opacity:1; }
  100% { transform:scale(1); opacity:0.7; }
}

h1 {
  font-family:'Poppins', sans-serif;
  font-size:3rem;
  font-weight:600;
  margin-bottom:10px;
}

p.subtitle {
  font-size:1.1rem;
  color:var(--text-muted);
  margin-bottom:40px;
}

.email-container {
  display:flex;
  max-width:400px;
  width:100%;
  margin-bottom:30px;
}

.email-container input {
  flex:1;
  padding:12px 16px;
  border:1px solid #ddd;
  border-radius:8px 0 0 8px;
  outline:none;
  font-size:0.95rem;
}

.email-container button {
  padding:12px 20px;
  background-color:var(--primary);
  color:#fff;
  border:none;
  border-radius:0 8px 8px 0;
  cursor:pointer;
  font-size:0.95rem;
  font-weight:500;
}

.email-container button:hover {
  opacity:0.9;
}

.contact {
  font-size:0.95rem;
  margin-top:20px;
}

.contact a {
  color:var(--primary);
  text-decoration:none;
  margin:0 10px;
}

footer {
  margin-top:50px;
  font-size:0.85rem;
  color:var(--text-muted);
}

@media(max-width:480px){
  h1 { font-size:2.2rem; }
  p.subtitle { font-size:1rem; }
}
</style>
</head>

<body>

<div class="hero">
  <h1>Elvona Store</h1>
  <p class="subtitle">Beauty, Cosmetic & Personal Care | Coming Soon</p>
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
;(function(n,t,c){
function i(n){return e._h?e._h.apply(null,n):e._q.push(n)}
var e={_q:[],_h:null,_v:"2.0",
on:function(){i(["on",c.call(arguments)])},
once:function(){i(["once",c.call(arguments)])},
off:function(){i(["off",c.call(arguments)])},
get:function(){
if(!e._h)throw new Error("[LiveChatWidget] You can't use getters before load.");
return i(["get",c.call(arguments)])
},
call:function(){i(["call",c.call(arguments)])},
init:function(){
var n=t.createElement("script");
n.async=!0;
n.type="text/javascript";
n.src="https://cdn.livechatinc.com/tracking.js";
t.head.appendChild(n)
}};
!n.__lc.asyncInit&&e.init();
n.LiveChatWidget=n.LiveChatWidget||e
}(window,document,[].slice))
</script>
<noscript>
<a href="https://www.livechat.com/chat-with/19508807/" rel="nofollow">
Chat with us
</a>
</noscript>
<!-- End of LiveChat code -->

</body>
</html>
