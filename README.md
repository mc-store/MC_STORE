<!DOCTYPE html>  <html lang="en">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<meta name="theme-color" content="#080b12">  
<title>MC STORE | Minecraft Cape Shop</title>  <style>  
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800;900&display=swap');  
  
:root {  
  --bg: #080b12;  
  --panel: #101722;  
  --border: #253745;  
  --text: #f4faff;  
  --muted: #9aabb8;  
  --cyan: #00e5ff;  
  --orange: #e07828;  
}  
  
* {  
  box-sizing: border-box;  
  margin: 0;  
  padding: 0;  
}  
  
html {  
  scroll-behavior: smooth;  
  scroll-padding-top: 90px;  
}  
  
body {  
  color: var(--text);  
  font-family: Inter, Arial, sans-serif;  
  overflow-x: hidden;  
  background:  
    radial-gradient(ellipse at 0% 8%, #00e5ff20, transparent 35%),  
    radial-gradient(ellipse at 100% 24%, #b9501329, transparent 37%),  
    #080b12;  
  background-attachment: fixed;  
}  
  
a {  
  color: inherit;  
  text-decoration: none;  
}  
  
.sale-marquee {  
  overflow: hidden;  
  white-space: nowrap;  
  background: linear-gradient(100deg, #873b12, #007d91, #a44813);  
  color: white;  
  padding: 12px 0;  
  border-bottom: 1px solid #00e5ff35;  
}  
  
.sale-track {  
  display: flex;  
  width: max-content;  
  animation: scroll 30s linear infinite;  
}  
  
.sale-track span {  
  padding: 0 25px;  
  font-size: 11px;  
  font-weight: 900;  
  letter-spacing: 2px;  
}  
  
@keyframes scroll {  
  to { transform: translateX(-50%); }  
}  
  
nav {  
  min-height: 76px;  
  display: flex;  
  align-items: center;  
  justify-content: space-between;  
  gap: 20px;  
  padding: 10px 8%;  
  border-bottom: 1px solid #00e5ff20;  
  background: #080b12ed;  
  position: sticky;  
  top: 0;  
  z-index: 10;  
}  
  
.brand-logo {  
  display: block;  
  width: 165px;  
  height: 58px;  
  object-fit: contain;  
}  
  
.links {  
  display: flex;  
  align-items: center;  
  gap: 25px;  
}  
  
.links a:not(.btn) {  
  color: var(--muted);  
  font-size: 13px;  
  font-weight: 600;  
}  
  
.btn {  
  display: inline-flex;  
  align-items: center;  
  justify-content: center;  
  gap: 8px;  
  padding: 13px 20px;  
  border-radius: 9px;  
  background: linear-gradient(110deg, #a94b16, #007f96);  
  color: white;  
  font-size: 13px;  
  font-weight: 800;  
  border: 1px solid #00e5ff35;  
  cursor: pointer;  
  transition: .25s;  
}  
  
.btn:hover {  
  transform: translateY(-3px);  
  filter: brightness(1.15);  
  box-shadow: 0 8px 28px #00cfe52b;  
}  
  
.btn-secondary {  
  background: #101722;  
  border: 1px solid #344650;  
}  
  
.hero {  
  text-align: center;  
  padding: 112px 20px 85px;  
}  
  
.eyebrow {  
  display: inline-block;  
  border: 1px solid #00e5ff50;  
  color: var(--cyan);  
  padding: 9px 15px;  
  border-radius: 30px;  
  font-size: 10px;  
  font-weight: 800;  
  letter-spacing: 2px;  
}  
  
h1 {  
  font-size: clamp(40px, 7vw, 78px);  
  line-height: 1.08;  
  letter-spacing: -4px;  
  margin: 27px auto 22px;  
}  
  
.gradient {  
  background: linear-gradient(100deg, var(--cyan), #65f0ff 45%, var(--orange));  
  -webkit-background-clip: text;  
  background-clip: text;  
  color: transparent;  
}  
  
.hero p {  
  max-width: 570px;  
  margin: 0 auto 30px;  
  color: var(--muted);  
  font-size: 15px;  
  line-height: 1.9;  
}  
  
.hero-actions {  
  display: flex;  
  justify-content: center;  
  flex-wrap: wrap;  
  gap: 12px;  
}  
  
.stats {  
  display: flex;  
  justify-content: center;  
  gap: 55px;  
  margin-top: 48px;  
  flex-wrap: wrap;  
}  
  
.stat strong {  
  display: block;  
  font-size: 19px;  
}  
  
.stat span {  
  display: block;  
  color: var(--muted);  
  font-size: 11px;  
  margin-top: 6px;  
}  
  
section {  
  padding: 72px 8%;  
}  
  
.section-head {  
  display: flex;  
  justify-content: space-between;  
  align-items: end;  
  gap: 20px;  
  margin-bottom: 32px;  
  flex-wrap: wrap;  
}  
  
.kicker {  
  color: var(--cyan);  
  text-transform: uppercase;  
  font-size: 10px;  
  font-weight: 900;  
  letter-spacing: 2px;  
  margin-bottom: 11px;  
}  
  
h2 {  
  font-size: clamp(28px, 4vw, 39px);  
  letter-spacing: -1.5px;  
}  
  
.sub {  
  color: var(--muted);  
  font-size: 13px;  
  margin-top: 10px;  
  line-height: 1.8;  
}  
  
.products {  
  display: grid;  
  grid-template-columns: repeat(3, minmax(0, 1fr));  
  gap: 23px;  
}  
  
.card {  
  border: 1px solid #263b49;  
  background: linear-gradient(150deg, #131f2cf5, #0c131df5);  
  border-radius: 16px;  
  overflow: hidden;  
  transition: .3s;  
}  
  
.card:hover {  
  transform: translateY(-7px);  
  border-color: var(--cyan);  
  box-shadow: 0 15px 40px #0006;  
}  
  
.art {  
  height: 245px;  
  display: flex;  
  align-items: center;  
  justify-content: center;  
  position: relative;  
  overflow: hidden;  
  background:  
    radial-gradient(ellipse at 18% 50%, #b9501323, transparent 60%),  
    radial-gradient(ellipse at 82% 50%, #00e5ff20, transparent 60%),  
    #0a111b;  
}  
  
.tag {  
  position: absolute;  
  top: 15px;  
  left: 15px;  
  z-index: 2;  
  background: #17232d;  
  border: 1px solid #344650;  
  color: #dceaf0;  
  padding: 7px 10px;  
  border-radius: 6px;  
  font-size: 9px;  
  font-weight: 800;  
}  
  
.tag.stock {  
  color: #8af7b0;  
  border-color: #35d77966;  
  background: #123522;  
}  
  
.tag.sold {  
  color: #ffaaaa;  
  border-color: #ff777755;  
  background: #3a1c25;  
}  
  
.cape-img {  
  display: block;  
  width: 165px;  
  height: 190px;  
  object-fit: contain;  
  filter: drop-shadow(0 12px 22px #0009);  
  transition: .35s;  
}  
  
.card:hover .cape-img {  
  transform: scale(1.08);  
}  
  
.details {  
  padding: 22px;  
}  
  
.details h3 {  
  font-size: 17px;  
  font-weight: 800;  
}  
  
.details p {  
  color: var(--muted);  
  font-size: 12px;  
  margin-top: 9px;  
  line-height: 1.8;  
  min-height: 43px;  
}  
  
.price-row {  
  display: flex;  
  justify-content: space-between;  
  align-items: center;  
  gap: 12px;  
  margin-top: 22px;  
  flex-wrap: wrap;  
}  
  
.price {  
  font-size: 14px;  
  font-weight: 800;  
}  
  
.price small {  
  display: block;  
  color: var(--muted);  
  font-size: 10px;  
  font-weight: 500;  
  margin-top: 4px;  
}  
  
.order {  
  font-size: 11px;  
  padding: 11px 14px;  
}  
  
.discord {  
  margin: 20px 8% 75px;  
  padding: 58px 25px;  
  text-align: center;  
  border: 1px solid #00e5ff45;  
  border-radius: 20px;  
  background:  
    radial-gradient(ellipse at 0% 100%, #b9501328, transparent 55%),  
    radial-gradient(ellipse at 100% 0%, #00e5ff1d, transparent 55%),  
    #101722ed;  
}  
  
.discord p {  
  color: var(--muted);  
  max-width: 500px;  
  margin: 16px auto 26px;  
  font-size: 13px;  
  line-height: 1.9;  
}  
  
footer {  
  border-top: 1px solid #00e5ff25;  
  padding: 27px 8%;  
  display: flex;  
  justify-content: space-between;  
  align-items: center;  
  gap: 15px;  
  flex-wrap: wrap;  
  color: var(--muted);  
  font-size: 11px;  
}  
  
@media (max-width: 850px) {  
  nav { padding: 10px 5%; }  
  section { padding: 55px 5%; }  
  .products { grid-template-columns: repeat(2, minmax(0, 1fr)); }  
  .discord { margin: 15px 5% 50px; }  
}  
  
@media (max-width: 540px) {  
  nav { min-height: 66px; gap: 10px; padding: 8px 4%; }  
  .brand-logo { width: 105px; height: 42px; }  
  .links { gap: 12px; }  
  .links a:not(.btn) { font-size: 11px; }  
  .links .btn { padding: 10px 12px; font-size: 11px; }  
  .hero { padding: 76px 18px 58px; }  
  h1 { letter-spacing: -2px; }  
  .stats { gap: 25px; }  
  .products { grid-template-columns: 1fr; }  
  .art { height: 260px; }  
  .discord { padding: 42px 20px; }  
  footer { flex-direction: column; align-items: flex-start; }  
}  
  
@media (prefers-reduced-motion: reduce) {  
  html { scroll-behavior: auto; }  
  *, *::before, *::after {  
    animation-duration: .01ms !important;  
    animation-iteration-count: 1 !important;  
    transition-duration: .01ms !important;  
  }  
}  
</style>  </head>  <body>  <div class="sale-marquee">  
  <div class="sale-track">  
    <span>IN STOCK: BUILDER ✦ AURORA ✦ CORRUPTED CAPES</span>  
    <span>OTHER CAPES: NOT IN STOCK</span>  
    <span>QUESTIONS? JOIN OUR DISCORD</span>  
    <span>IN STOCK: BUILDER ✦ AURORA ✦ CORRUPTED CAPES</span>  
    <span>OTHER CAPES: NOT IN STOCK</span>  
    <span>QUESTIONS? JOIN OUR DISCORD</span>  
  </div>  
</div>  <nav>  
  <a class="brand" href="#home">  
    <img class="brand-logo" src="media/1792194385872.png" alt="MC STORE Logo">  
  </a>  
  <div class="links">  
    <a href="#home">Home</a>  
    <a href="#shop">Capes</a>  
    <a class="btn" href="#shop">Shop Now ↗</a>  
  </div>  
</nav>  <header class="hero" id="home">  
  <span class="eyebrow">THE MC STORE COLLECTION</span>  
  <h1>Discover Minecraft<br><span class="gradient">Capes.</span></h1>  
  <p>  
    Builder, Aurora, and Corrupted Capes are currently in stock.  
    All other capes are not in stock. Contact our team on Discord  
    to order or ask about restocks.  
  </p>    <div class="hero-actions">  
    <a class="btn" href="#shop">Explore Collection ↗</a>  
    <a class="btn btn-secondary"  
       href="https://discord.com/invite/F38vcYVHA"  
       target="_blank" rel="noopener noreferrer">Join Discord ↗</a>  
  </div>    <div class="stats">  
    <div class="stat"><strong>MC STORE</strong><span>Your cape destination</span></div>  
    <div class="stat"><strong>Exclusive</strong><span>Minecraft capes</span></div>  
    <div class="stat"><strong>Community</strong><span>Discord support</span></div>  
  </div>  
</header>  <section id="shop">  
  <div class="section-head">  
    <div>  
      <div class="kicker">OUR COLLECTION</div>  
      <h2>Featured <span class="gradient">Capes</span></h2>  
      <p class="sub">  
        Currently in stock: Builder Cape, Aurora Cape, and Corrupted Cape.  
        All other capes are not in stock.  
      </p>  
    </div>  
    <a class="btn" href="https://discord.com/invite/F38vcYVHA"  
       target="_blank" rel="noopener noreferrer">Ask About Stock ↗</a>  
  </div>    <div class="products">  <!-- 1. CORRUPTED CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag stock">IN STOCK</span>  
    <img class="cape-img" src="media/cloakFront%20(2).webp"  
         alt="Corrupted Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Corrupted Cape</h3>  
    <p>A distinctive cape for your Minecraft collection.</p>  
    <div class="price-row">  
      <div class="price">Contact us<small>For current price</small></div>  
      <a class="btn order" href="https://discord.com/invite/F38vcYVHA"  
         target="_blank" rel="noopener noreferrer">BUY NOW ↗</a>  
    </div>  
  </div>  
</article>  

<!-- 2. AURORA CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag stock">IN STOCK</span>  
    <img class="cape-img" src="media/aurora-front.png"  
         alt="Aurora Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Aurora Cape</h3>  
    <p>A vibrant cape for players who want to stand out.</p>  
    <div class="price-row">  
      <div class="price">Contact us<small>For current price</small></div>  
      <a class="btn order" href="https://discord.com/invite/F38vcYVHA"  
         target="_blank" rel="noopener noreferrer">BUY NOW ↗</a>  
    </div>  
  </div>  
</article>  

<!-- 3. BUILDER CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag stock">IN STOCK</span>  
    <img class="cape-img" src="media/320%20(1).png"  
         alt="Builder Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Builder Cape</h3>  
    <p>A classic addition for Minecraft cape collectors.</p>  
    <div class="price-row">  
      <div class="price">Contact us<small>For current price</small></div>  
      <a class="btn order" href="https://discord.com/invite/F38vcYVHA"  
         target="_blank" rel="noopener noreferrer">BUY NOW ↗</a>  
    </div>  
  </div>  
</article>  

<!-- 4. EXPERIENCE CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag sold">NOT IN STOCK</span>  
    <img class="cape-img" src="media/320%20(2).png"  
         alt="Experience Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Experience Cape</h3>  
    <p>A special cape to add to your Minecraft collection.</p>  
    <div class="price-row">  
      <div class="price">Not in stock<small>Currently unavailable</small></div>  
    </div>  
  </div>  
</article>  

<!-- 5. CRAFTER CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag sold">NOT IN STOCK</span>  
    <img class="cape-img" src="media/320%20(3).png"  
         alt="Crafter Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Crafter Cape</h3>  
    <p>A distinctive cape for Minecraft fans and collectors.</p>  
    <div class="price-row">  
      <div class="price">Not in stock<small>Currently unavailable</small></div>  
    </div>  
  </div>  
</article>  

<!-- 6. MENACE CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag sold">NOT IN STOCK</span>  
    <img class="cape-img" src="media/320%20(5).png"  
         alt="Menace Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Menace Cape</h3>  
    <p>A striking cape for your Minecraft collection.</p>  
    <div class="price-row">  
      <div class="price">Not in stock<small>Currently unavailable</small></div>  
    </div>  
  </div>  
</article>  

<!-- 7. COPPER CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag sold">NOT IN STOCK</span>  
    <img class="cape-img" src="media/320%20(6).png"  
         alt="Copper Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Copper Cape</h3>  
    <p>A copper-themed cape for Minecraft players.</p>  
    <div class="price-row">  
      <div class="price">Not in stock<small>Currently unavailable</small></div>  
    </div>  
  </div>  
</article>  

<!-- 8. MOONLIGHT CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag sold">NOT IN STOCK</span>  
    <img class="cape-img" src="media/cloakFront%20(4).webp"  
         alt="Moonlight Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Moonlight Cape</h3>  
    <p>A moonlight-inspired cape for your Minecraft collection.</p>  
    <div class="price-row">  
      <div class="price">Not in stock<small>Currently unavailable</small></div>  
    </div>  
  </div>  
</article>  

<!-- 9. PURPLE HEART CAPE -->  
<article class="card">  
  <div class="art">  
    <span class="tag sold">NOT IN STOCK</span>  
    <img class="cape-img" src="media/320%20(7).png"  
         alt="Purple Heart Cape" loading="lazy">  
  </div>  
  <div class="details">  
    <h3>Purple Heart Cape</h3>  
    <p>A purple-themed cape to add to your Minecraft collection.</p>  
    <div class="price-row">  
      <div class="price">Not in stock<small>Currently unavailable</small></div>  
    </div>  
  </div>  
</article>

  </div>  
</section>  <div class="discord" id="discord">  
  <div class="kicker">NEED HELP?</div>  
  <h2>Join the <span class="gradient">MC STORE</span> Discord</h2>  
  <p>  
    Have a question about an available cape or a future restock?  
    Join our Discord community to contact us.  
  </p>  
  <a class="btn" href="https://discord.com/invite/F38vcYVHA"  
     target="_blank" rel="noopener noreferrer">Join Discord ↗</a>  
</div>  <footer>  
  <span>© <span id="year">2026</span> MC STORE. All rights reserved.</span>  
  <span>Independent community shop. Not affiliated with Mojang or Microsoft.</span>  
</footer>  <script>  
document.getElementById('year').textContent = new Date().getFullYear();  
</script>  </body>  
  </html>
