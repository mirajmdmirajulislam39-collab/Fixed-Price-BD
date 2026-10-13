
<!doctype html>
<html lang="bn">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Fixed Price BD | Online Store</title>
<style>
*{box-sizing:border-box}
body{margin:0;background:#f5faf7;color:#17352f;font-family:system-ui,sans-serif}
header,footer{background:linear-gradient(110deg,#004a43,#00815f);color:white;padding:16px 4%;display:flex;justify-content:space-between;align-items:center;gap:14px;flex-wrap:wrap}
.logo{font-size:25px;font-weight:900}.logo span{color:#ffd52b}
.search{flex:1;min-width:180px}.search input{width:100%;padding:12px;border:0;border-radius:10px}
nav{display:flex;gap:20px;padding:14px 4%;background:white;overflow:auto;white-space:nowrap}
nav a{color:#17352f;font-weight:bold;text-decoration:none}
.wrap{max-width:1300px;margin:auto;padding:18px}
.hero{padding:28px;border-radius:16px;background:linear-gradient(100deg,#ffe5ef,#e2ffdf,#fff0c6);display:flex;justify-content:space-between;align-items:center;gap:15px}
.hero h1{font-size:clamp(30px,5vw,55px);margin:0;color:#005247}
.tag{background:#ffdc28;padding:8px 14px;border-radius:9px;font-weight:900}
.heroart{font-size:65px}
.products{display:grid;grid-template-columns:repeat(5,minmax(0,1fr));gap:12px}
.product,.feature,.cart{background:white;border:1px solid #dce9e4;border-radius:13px;padding:10px;min-width:0}
.pic{height:130px;border-radius:9px;background:linear-gradient(135deg,#fce4e7,#e8f5ee);display:grid;place-items:center;font-size:55px;position:relative;overflow:hidden}
.pic img{width:100%;height:100%;object-fit:contain}
.badge{position:absolute;top:8px;left:8px;background:#e9233a;color:white;border-radius:30px;padding:4px 7px;font-size:12px;font-weight:bold}
.product h3{font-size:14px;min-height:36px}
.old{text-decoration:line-through;color:#718980}
.now{color:#e9233a;font-size:20px;font-weight:900}
.save{display:inline-block;background:#d7f7df;padding:5px 8px;border-radius:20px;font-size:12px}
.rating{font-size:12px;color:#aa7200;margin:9px 0}
.btn{background:#00845f;color:white;border:0;border-radius:8px;padding:10px;font-weight:bold;cursor:pointer;width:100%;margin-top:7px}
.features{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin:22px 0}
.feature{padding:18px}.cart{margin:20px 0;padding:16px}
.cartrow{display:flex;justify-content:space-between;gap:8px;border-bottom:1px solid #e3eeea;padding:8px 0}
.total{font-size:20px;color:#e9233a;font-weight:900}
.muted{color:#607872;font-size:13px}
@media(max-width:950px){.products{grid-template-columns:repeat(3,1fr)}}
@media(max-width:600px){.products{grid-template-columns:repeat(2,minmax(0,1fr))}.pic{height:110px}.features{grid-template-columns:1fr}.wrap{padding:10px}.hero{padding:18px}.heroart{font-size:40px}}
</style>
</head>
<body>
<header>
<div class="logo">🛍 Fixed Price <span>BD</span><div class="muted" style="color:white">Retail & Wholesale</div></div>
<div class="search"><input id="search" placeholder="পণ্য খুঁজুন..." oninput="draw()"></div>
<div>🛒 কার্ট <b id="count">0</b></div>
<div>WhatsApp & imo<br><b style="color:#ffdc28">01865146318</b></div>
<a style="color:white" href="admin.html">অ্যাডমিন</a>
</header>
<nav>
<a href="#">⌂ হোম</a><a href="#products">সব পণ্য</a><a href="#products">ব্রা ও পেন্টি</a><a href="#products">নাইটি</a><a href="#products">বেল্ট</a><a href="#products">স্কিন কেয়ার</a><a href="#products">বিউটি প্রোডাক্ট</a><a href="#products">ইলেকট্রনিক</a><a href="#products">অফার</a>
</nav>
<main class="wrap">
<section class="hero">
<div><div class="muted">FIXED PRICE BD</div><h1>Retail & Wholesale</h1><p><span class="tag">সেরা পণ্য, সেরা দাম!</span></p><p>✅ মানসম্মত পণ্য　🚚 সারা বাংলাদেশে ডেলিভারি　🕒 ২৪ ঘণ্টা অর্ডার</p><a class="btn" style="display:inline-block;width:auto;text-decoration:none" href="#products">পণ্য দেখুন →</a></div>
<div class="heroart">🎀 🧴 🩱</div>
</section>
<h2 id="products">🔥 জনপ্রিয় পণ্য</h2>
<div class="products" id="grid"></div>
<div class="features">
<div class="feature">💯 <b>ডিসকাউন্ট অটো হিসাব</b><p class="muted">আগের দাম ও অফার দাম থেকে ছাড় হিসাব হবে।</p></div>
<div class="feature">🛍️ <b>সুন্দর পণ্যের কার্ড</b><p class="muted">ছবি, দাম, ছাড় ও কার্টের তথ্য।</p></div>
<div class="feature">🚚 <b>হোম ডেলিভারি</b><p class="muted">ঢাকা ১–২ দিন | অন্যান্য ১–৩ দিন</p></div>
</div>
<section class="cart">
<h2>🛒 আপনার কার্ট (<span id="count2">0</span>)</h2>
<div id="cartitems">কার্ট খালি</div>
<div class="cartrow"><span>মোট দাম</span><b id="subtotal">৳0</b></div>
<div class="cartrow"><span>ডিসকাউন্ট</span><b id="discount">৳0</b></div>
<div class="cartrow total"><span>সর্বমোট</span><b id="total">৳0</b></div>
<button class="btn" onclick="checkout()">WhatsApp-এ অর্ডার করুন</button>
</section>
<p class="muted">খুচরা ও পাইকারি বিক্রি করা হয়।</p>
</main>
<footer>
<div>📣 খুচরা ও পাইকারি বিক্রি করা হয়<br>Retail & Wholesale</div>
<div>WhatsApp & imo: 01865146318</div>
<div>🏠 সারা বাংলাদেশে হোম ডেলিভারি সুবিধা</div>
</footer>
<script>
const DEFAULT=[
{id:1,n:"৬ পিস সেমিস ব্রা (Genji)",d:"সুন্দর ফিটিং, আরামদায়ক",e:"🎀",o:1200,p:350,r:"4.8",s:50,img:""},
{id:2,n:"Jute Full Net Bra",d:"হালকা ও আরামদায়ক",e:"👙",o:370,p:150,r:"4.6",s:30,img:""},
{id:3,n:"Depilatory Hot Wax Beans",d:"ওয়াক্সিংয়ের জন্য",e:"🧴",o:396,p:250,r:"4.7",s:40,img:""},
{id:4,n:"TONO HIME Jelly (100ml)",d:"স্কিন কেয়ার জেল",e:"🫙",o:250,p:120,r:"4.9",s:60,img:""},
{id:5,n:"Women's Waist Trainer Belt",d:"কোমর সাপোর্ট বেল্ট",e:"🩱",o:800,p:400,r:"4.5",s:25,img:""}
];
function getProducts(){
try{let x=JSON.parse(localStorage.getItem("fpbd_products"));return Array.isArray(x)&&x.length?x:DEFAULT}
catch(e){return DEFAULT}
}
let P=getProducts(),C={};
const money=n=>"৳"+Math.round(n).toLocaleString("en-US");
const pct=p=>p.o>0?Math.max(0,Math.round((p.o-p.p)/p.o*100)):0;
function draw(){
P=getProducts();
let q=document.getElementById("search").value.toLowerCase();
document.getElementById("grid").innerHTML=P.filter(p=>(p.n+" "+p.d).toLowerCase().includes(q)).map(p=>`
<article class="product">
<div class="pic"><span class="badge">${pct(p)}% ছাড়</span>${p.img?`<img src="${p.img}" alt="">`:p.e||"📦"}</div>
<h3>${p.n}</h3><div class="muted">${p.d||""}</div>
<p><span class="old">${money(p.o)}</span> <span class="now">${money(p.p)}</span></p>
<span class="save">সাশ্রয় ${money(Math.max(0,p.o-p.p))}</span>
<div class="rating">⭐⭐⭐⭐⭐ (${p.r||"5.0"})<br>স্টক: ${p.s||0}</div>
<button class="btn" onclick="add(${p.id})">🛒 কার্টে নিন</button>
</article>`).join("")||"<p>কোনো পণ্য পাওয়া যায়নি।</p>";
}
function add(id){C[id]=(C[id]||0)+1;cartdraw()}
function change(id,n){C[id]=(C[id]||0)+n;if(C[id]<=0)delete C[id];cartdraw()}
function cartdraw(){
let ids=Object.keys(C),cnt=ids.reduce((s,id)=>s+C[id],0),sub=0,off=0;
document.getElementById("count").textContent=cnt;
document.getElementById("count2").textContent=cnt;
document.getElementById("cartitems").innerHTML=ids.length?ids.map(id=>{
let p=P.find(x=>x.id==id);if(!p)return "";
sub+=p.o*C[id];off+=(p.o-p.p)*C[id];
return `<div class="cartrow"><span>${p.e||"📦"} ${p.n}<br><small>${money(p.p)} × ${C[id]}</small><br><span><button onclick="change(${id},-1)">−</button> ${C[id]} <button onclick="change(${id},1)">+</button></span></span><b>${money(p.p*C[id])}</b></div>`;
}).join(""):"কার্ট খালি";
document.getElementById("subtotal").textContent=money(sub);
document.getElementById("discount").textContent="−"+money(off);
document.getElementById("total").textContent=money(sub-off);
}
function checkout(){
let ids=Object.keys(C);
if(!ids.length){alert("আগে কার্টে পণ্য যোগ করুন।");return}
let rows=ids.map(id=>{let p=P.find(x=>x.id==id);return p.n+" × "+C[id]+" = "+money(p.p*C[id])}).join("\n");
let total=ids.reduce((s,id)=>s+P.find(p=>p.id==id).p*C[id],0);
let msg="আসসালামু আলাইকুম, Fixed Price BD থেকে অর্ডার করতে চাই:\n"+rows+"\nমোট: "+money(total)+"\nনাম ও ঠিকানা জানাব।";
location.href="https://wa.me/8801865146318?text="+encodeURIComponent(msg);
}
draw();cartdraw();
</script>
</body>
</html>

