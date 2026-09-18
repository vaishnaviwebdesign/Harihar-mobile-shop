<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Harihar Mobile Shop | Mobile Sales, Repair & Accessories</title>

<meta name="description" content="Harihar Mobile Shop - Mobile Sales, Repairing, Accessories, Recharge and Tempered Glass.">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
    scroll-behavior:smooth;
}

body{
    background:#080808;
    color:white;
}

/* HEADER */
header{
    position:sticky;
    top:0;
    z-index:1000;
    background:rgba(8,8,8,0.95);
    backdrop-filter:blur(10px);
    border-bottom:1px solid #333;
}

.navbar{
    max-width:1200px;
    margin:auto;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:15px 20px;
}

.logo{
    display:flex;
    align-items:center;
    gap:12px;
}

.logo-icon{
    width:48px;
    height:48px;
    border-radius:50%;
    background:linear-gradient(135deg,#ffd700,#ff9d00);
    display:flex;
    align-items:center;
    justify-content:center;
    color:#111;
    font-size:23px;
    font-weight:bold;
}

.logo-text h2{
    color:#ffd700;
    font-size:20px;
}

.logo-text p{
    color:#aaa;
    font-size:11px;
}

nav a{
    color:white;
    text-decoration:none;
    margin-left:22px;
    font-size:14px;
    transition:.3s;
}

nav a:hover{
    color:#ffd700;
}

/* HERO */
.hero{
    min-height:90vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:60px 20px;
    background:
    radial-gradient(circle at top,#382b00 0%,transparent 35%),
    linear-gradient(135deg,#050505,#171717,#050505);
}

.hero-content{
    max-width:900px;
}

.badge{
    display:inline-block;
    border:1px solid #ffd700;
    color:#ffd700;
    padding:8px 18px;
    border-radius:30px;
    font-size:13px;
    margin-bottom:20px;
}

.hero h1{
    font-size:clamp(40px,8vw,80px);
    line-height:1;
    margin-bottom:20px;
}

.hero h1 span{
    color:#ffd700;
}

.hero p{
    color:#ccc;
    max-width:650px;
    margin:auto;
    line-height:1.7;
    font-size:16px;
}

.buttons{
    margin-top:30px;
    display:flex;
    justify-content:center;
    gap:15px;
    flex-wrap:wrap;
}

.btn{
    padding:14px 25px;
    border-radius:30px;
    text-decoration:none;
    font-weight:bold;
    transition:.3s;
}

.btn-gold{
    background:#ffd700;
    color:#111;
}

.btn-gold:hover{
    transform:translateY(-3px);
    box-shadow:0 10px 30px rgba(255,215,0,.3);
}

.btn-outline{
    border:1px solid #ffd700;
    color:#ffd700;
}

.btn-outline:hover{
    background:#ffd700;
    color:#111;
}

/* SECTIONS */
section{
    padding:75px 20px;
}

.container{
    max-width:1150px;
    margin:auto;
}

.section-title{
    text-align:center;
    margin-bottom:45px;
}

.section-title h2{
    font-size:38px;
}

.section-title h2 span{
    color:#ffd700;
}

.section-title p{
    color:#aaa;
    margin-top:10px;
}

/* SERVICES */
.services{
    background:#0d0d0d;
}

.service-grid{
    display:grid;
    grid-template-columns:repeat(5,1fr);
    gap:18px;
}

.service-card{
    background:linear-gradient(145deg,#191919,#0c0c0c);
    border:1px solid #292929;
    border-radius:20px;
    padding:30px 15px;
    text-align:center;
    transition:.3s;
}

.service-card:hover{
    transform:translateY(-8px);
    border-color:#ffd700;
    box-shadow:0 10px 35px rgba(255,215,0,.12);
}

.service-icon{
    width:65px;
    height:65px;
    margin:0 auto 18px;
    border-radius:18px;
    background:rgba(255,215,0,.1);
    border:1px solid rgba(255,215,0,.4);
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:30px;
}

.service-card h3{
    font-size:17px;
    margin-bottom:8px;
}

.service-card p{
    color:#999;
    font-size:13px;
    line-height:1.5;
}

/* ABOUT */
.about{
    background:#080808;
}

.about-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:50px;
    align-items:center;
}

.about-box{
    background:linear-gradient(145deg,#191919,#0c0c0c);
    padding:40px;
    border-radius:25px;
    border:1px solid #292929;
}

.about-box h2{
    font-size:35px;
    margin-bottom:18px;
}

.about-box h2 span{
    color:#ffd700;
}

.about-box p{
    color:#bbb;
    line-height:1.8;
}

.features{
    margin-top:25px;
}

.features div{
    margin:12px 0;
    color:#ddd;
}

.features span{
    color:#ffd700;
    margin-right:8px;
}

/* STATS */
.stats{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
    margin-top:20px;
}

.stat{
    text-align:center;
    padding:25px;
    border:1px solid #292929;
    border-radius:18px;
}

.stat h3{
    color:#ffd700;
    font-size:30px;
}

.stat p{
    color:#999;
    font-size:13px;
}

/* PRODUCTS */
.products{
    background:#0d0d0d;
}

.product-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:20px;
}

.product-card{
    background:#151515;
    border:1px solid #292929;
    border-radius:20px;
    overflow:hidden;
    transition:.3s;
}

.product-card:hover{
    transform:translateY(-5px);
    border-color:#ffd700;
}

.product-img{
    height:180px;
    background:
    radial-gradient(circle,#393000,#141414 60%);
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:65px;
}

.product-info{
    padding:20px;
}

.product-info h3{
    margin-bottom:8px;
}

.product-info p{
    color:#999;
    font-size:13px;
    line-height:1.5;
}

/* WHY US */
.why{
    background:#080808;
}

.why-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:20px;
}

.why-card{
    padding:30px;
    background:#111;
    border-radius:20px;
    border:1px solid #292929;
}

.why-card .number{
    color:#ffd700;
    font-size:30px;
    font-weight:bold;
}

.why-card h3{
    margin:12px 0;
}

.why-card p{
    color:#999;
    line-height:1.6;
    font-size:14px;
}

/* CONTACT */
.contact{
    background:
    radial-gradient(circle at center,#332700 0%,transparent 45%),
    #0d0d0d;
}

.contact-box{
    max-width:850px;
    margin:auto;
    text-align:center;
    background:rgba(20,20,20,.9);
    border:1px solid #333;
    border-radius:25px;
    padding:45px 25px;
}

.contact-box h2{
    font-size:38px;
    margin-bottom:15px;
}

.contact-box h2 span{
    color:#ffd700;
}

.contact-box p{
    color:#aaa;
    margin-bottom:25px;
}

.contact-info{
    display:flex;
    justify-content:center;
    gap:15px;
    flex-wrap:wrap;
}

.info{
    padding:13px 20px;
    border:1px solid #333;
    border-radius:30px;
    color:#ddd;
}

/* FOOTER */
footer{
    background:#050505;
    border-top:1px solid #222;
    text-align:center;
    padding:30px 20px;
}

footer h3{
    color:#ffd700;
    margin-bottom:8px;
}

footer p{
    color:#777;
    font-size:13px;
}

/* FLOATING WHATSAPP */
.whatsapp{
    position:fixed;
    right:20px;
    bottom:20px;
    width:58px;
    height:58px;
    border-radius:50%;
    background:#25D366;
    display:flex;
    align-items:center;
    justify-content:center;
    color:white;
    text-decoration:none;
    font-size:28px;
    box-shadow:0 5px 25px rgba(0,0,0,.4);
    z-index:999;
}

/* MOBILE */
@media(max-width:900px){
    .service-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .product-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .about-grid{
        grid-template-columns:1fr;
    }

    .why-grid{
        grid-template-columns:1fr;
    }
}

@media(max-width:600px){
    nav{
        display:none;
    }

    .navbar{
        justify-content:center;
    }

    .hero{
        min-height:80vh;
    }

    .hero h1{
        font-size:45px;
    }

    section{
        padding:55px 15px;
    }

    .section-title h2{
        font-size:30px;
    }

    .service-grid{
        grid-template-columns:repeat(2,1fr);
        gap:12px;
    }

    .service-card{
        padding:22px 10px;
    }

    .product-grid{
        grid-template-columns:1fr 1fr;
        gap:12px;
    }

    .product-img{
        height:130px;
        font-size:45px;
    }

    .product-info{
        padding:15px;
    }

    .stats{
        grid-template-columns:1fr;
    }

    .about-box{
        padding:25px;
    }
}
</style>
</head>

<body>

<!-- HEADER -->
<header>
<div class="navbar">

<div class="logo">
<div class="logo-icon">H</div>
<div class="logo-text">
<h2>HARIHAR</h2>
<p>MOBILE SHOP</p>
</div>
</div>

<nav>
<a href="#home">Home</a>
<a href="#services">Services</a>
<a href="#products">Products</a>
<a href="#about">About</a>
<a href="#contact">Contact</a>
</nav>

</div>
</header>


<!-- HERO -->
<section class="hero" id="home">

<div class="hero-content">

<div class="badge">📱 YOUR TRUSTED MOBILE SHOP</div>

<h1>
HARIHAR<br>
<span>MOBILE SHOP</span>
</h1>

<p>
Mobile Sales • Repairing • Accessories • Recharge •
Tempered Glass
</p>

<p style="margin-top:12px;">
Quality Products. Reliable Service. Customer Satisfaction.
</p>

<div class="buttons">

<a href="#products" class="btn btn-gold">
Explore Products
</a>

<a href="#contact" class="btn btn-outline">
Contact Us
</a>

</div>

</div>

</section>


<!-- SERVICES -->
<section class="services" id="services">

<div class="container">

<div class="section-title">
<h2>Our <span>Services</span></h2>
<p>Everything you need for your mobile, all in one place.</p>
</div>

<div class="service-grid">

<div class="service-card">
<div class="service-icon">📱</div>
<h3>Mobile Sales</h3>
<p>Latest smartphones and mobile devices.</p>
</div>

<div class="service-card">
<div class="service-icon">🔧</div>
<h3>Mobile Repair</h3>
<p>Reliable mobile repairing and service.</p>
</div>

<div class="service-card">
<div class="service-icon">🎧</div>
<h3>Accessories</h3>
<p>Chargers, cables, earphones, covers and more.</p>
</div>

<div class="service-card">
<div class="service-icon">⚡</div>
<h3>Recharge</h3>
<p>Quick and convenient mobile recharge.</p>
</div>

<div class="service-card">
<div class="service-icon">🛡️</div>
<h3>Tempered Glass</h3>
<p>Screen protection for your smartphone.</p>
</div>

</div>
</div>

</section>


<!-- PRODUCTS -->
<section class="products" id="products">

<div class="container">

<div class="section-title">
<h2>Popular <span>Products</span></h2>
<p>Explore some of the products available at our shop.</p>
</div>

<div class="product-grid">

<div class="product-card">
<div class="product-img">📱</div>
<div class="product-info">
<h3>Smartphones</h3>
<p>New smartphones from popular brands.</p>
</div>
</div>

<div class="product-card">
<div class="product-img">🎧</div>
<div class="product-info">
<h3>Earphones</h3>
<p>Wired and wireless audio accessories.</p>
</div>
</div>

<div class="product-card">
<div class="product-img">🔌</div>
<div class="product-info">
<h3>Chargers</h3>
<p>Chargers and charging accessories.</p>
</div>
</div>

<div class="product-card">
<div class="product-img">📱</div>
<div class="product-info">
<h3>Mobile Covers</h3>
<p>Stylish and protective mobile covers.</p>
</div>
</div>

</div>

</div>

</section>


<!-- ABOUT -->
<section class="about" id="about">

<div class="container">

<div class="about-grid">

<div class="about-box">

<h2>Why <span>Harihar?</span></h2>

<p>
Harihar Mobile Shop is your local destination for
mobile phones, repairing services, accessories,
recharge and screen protection.
</p>

<div class="features">
<div><span>✓</span> Quality Products</div>
<div><span>✓</span> Reliable Mobile Repairing</div>
<div><span>✓</span> Useful Accessories</div>
<div><span>✓</span> Friendly Service</div>
<div><span>✓</span> Customer Satisfaction</div>
</div>

</div>


<div>

<div class="stats">

<div class="stat">
<h3>5+</h3>
<p>Services</p>
</div>

<div class="stat">
<h3>100%</h3>
<p>Customer Care</p>
</div>

<div class="stat">
<h3>24/7</h3>
<p>Online Enquiry</p>
</div>

</div>

</div>

</div>

</div>

</section>


<!-- WHY US -->
<section class="why">

<div class="container">

<div class="section-title">
<h2>Why Choose <span>Us?</span></h2>
<p>Simple service. Genuine products. Customer-focused experience.</p>
</div>

<div class="why-grid">

<div class="why-card">
<div class="number">01</div>
<h3>Trusted Service</h3>
<p>
We focus on providing dependable mobile services
and helpful customer support.
</p>
</div>

<div class="why-card">
<div class="number">02</div>
<h3>Quality Products</h3>
<p>
Choose from useful mobile accessories and products
for your everyday needs.
</p>
</div>

<div class="why-card">
<div class="number">03</div>
<h3>Easy Enquiry</h3>
<p>
Contact us easily for product availability,
repairing and service enquiries.
</p>
</div>

</div>

</div>

</section>


<!-- CONTACT -->
<section class="contact" id="contact">

<div class="container">

<div class="contact-box">

<h2>Visit <span>Harihar Mobile Shop</span></h2>

<p>
For mobile sales, repairing, accessories,
recharge and tempered glass.
</p>

<div class="contact-info">

<div class="info">📞 Your Mobile Number</div>

<div class="info">📍 Your Shop Address</div>

</div>

<div class="buttons">

<a href="tel:YOURNUMBER" class="btn btn-gold">
📞 Call Now
</a>

<a href="https://wa.me/YOURNUMBER" class="btn btn-outline">
💬 WhatsApp
</a>

</div>

</div>

</div>

</section>


<!-- FOOTER -->
<footer>

<h3>HARIHAR MOBILE SHOP</h3>

<p>
Mobile Sales • Repairing • Accessories • Recharge • Tempered Glass
</p>

<p style="margin-top:12px;">
© 2026 Harihar Mobile Shop. All Rights Reserved.
</p>

</footer>


<!-- WHATSAPP -->
<a href="https://wa.me/YOURNUMBER" class="whatsapp">
💬
</a>

</body>
</html>
