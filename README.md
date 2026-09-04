
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>HAN ET HOUSE — Etin Gerçek Hali</title>
<meta name="description" content="HAN ET HOUSE — Premium et ve ızgara deneyimi. Tokat.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<style>

:root{
  --bg:#f8f4ec;
  --bg2:#f1e9dc;
  --card:#fffdf8;
  --gold:#a77b32;
  --gold2:#c49a54;
  --dark:#211d18;
  --text:#332d25;
  --muted:#756d61;
  --line:rgba(100,75,40,.18);
  --shadow:0 25px 70px rgba(61,45,25,.10);
}

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

html{
  scroll-behavior:smooth;
}

body{
  background:var(--bg);
  color:var(--text);
  font-family:"Manrope",sans-serif;
  overflow-x:hidden;
}

a{
  color:inherit;
  text-decoration:none;
}

button,
input,
select,
textarea{
  font:inherit;
}

.container{
  width:min(1180px,92%);
  margin:auto;
}

section{
  padding:110px 0;
  position:relative;
}

.section-label{
  color:var(--gold);
  font-size:11px;
  letter-spacing:4px;
  text-transform:uppercase;
  font-weight:800;
  margin-bottom:18px;
}

.section-title{
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(45px,6vw,78px);
  line-height:.95;
  color:var(--dark);
  font-weight:600;
}

.section-title span{
  color:var(--gold);
  font-style:italic;
}

.section-text{
  color:var(--muted);
  line-height:1.9;
  font-size:14px;
  max-width:600px;
}


/* =========================================
   GİRİŞ ANİMASYONU
========================================= */

.loader{
  position:fixed;
  inset:0;
  z-index:99999;
  background:#181512;
  display:flex;
  align-items:center;
  justify-content:center;
  overflow:hidden;
  animation:loaderExit 1s ease 3.2s forwards;
}

.loader-content{
  text-align:center;
  animation:loaderContent 1.5s ease forwards;
}

.loader-brand{
  color:#f8f4ec;
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(55px,10vw,120px);
  letter-spacing:8px;
  line-height:.8;
}

.loader-sub{
  color:#c49a54;
  font-size:9px;
  letter-spacing:6px;
  margin-top:20px;
  opacity:0;
  animation:subAppear 1s ease 1s forwards;
}

.loader-line{
  width:0;
  height:1px;
  background:#c49a54;
  margin:25px auto 0;
  animation:lineGrow 1.2s ease .7s forwards;
}

@keyframes lineGrow{
  to{
    width:180px;
  }
}

@keyframes subAppear{
  to{
    opacity:1;
  }
}

@keyframes loaderContent{
  from{
    opacity:0;
    transform:scale(.92);
  }
  to{
    opacity:1;
    transform:scale(1);
  }
}

@keyframes loaderExit{
  to{
    opacity:0;
    visibility:hidden;
    pointer-events:none;
  }
}


/* NAVBAR */

.navbar{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  height:82px;
  z-index:1000;
  display:flex;
  align-items:center;
  transition:.35s;
}

.navbar.scrolled{
  background:rgba(248,244,236,.88);
  backdrop-filter:blur(20px);
  box-shadow:0 10px 30px rgba(40,30,20,.06);
}

.nav-inner{
  width:min(1180px,92%);
  margin:auto;
  display:flex;
  align-items:center;
  justify-content:space-between;
}

.logo{
  font-family:"Cormorant Garamond",serif;
  font-size:30px;
  font-weight:700;
  letter-spacing:2px;
  color:var(--dark);
}

.logo small{
  display:block;
  font-family:"Manrope",sans-serif;
  font-size:7px;
  letter-spacing:4px;
  color:var(--gold);
  margin-top:-5px;
}

.nav-links{
  display:flex;
  align-items:center;
  gap:30px;
}

.nav-links a{
  font-size:12px;
  font-weight:700;
  color:#4c443a;
  position:relative;
}

.nav-links a::after{
  content:"";
  position:absolute;
  bottom:-8px;
  left:0;
  width:0;
  height:1px;
  background:var(--gold);
  transition:.3s;
}

.nav-links a:hover::after{
  width:100%;
}

.nav-btn{
  background:var(--dark);
  color:white !important;
  padding:13px 20px;
  border-radius:4px;
}

.nav-btn::after{
  display:none;
}

.menu-toggle{
  display:none;
  border:0;
  background:none;
  font-size:28px;
  color:var(--dark);
  cursor:pointer;
}


/* HERO */

.hero{
  min-height:100vh;
  display:flex;
  align-items:center;
  overflow:hidden;
  background:
    radial-gradient(circle at 15% 20%,rgba(196,154,84,.18),transparent 25%),
    radial-gradient(circle at 90% 75%,rgba(167,123,50,.10),transparent 30%),
    var(--bg);
}

.hero-bg{
  position:absolute;
  inset:0;
  pointer-events:none;
}

.orb{
  position:absolute;
  border:1px solid rgba(167,123,50,.18);
  border-radius:50%;
  animation:float 10s ease-in-out infinite;
}

.orb.one{
  width:520px;
  height:520px;
  right:-180px;
  top:-120px;
}

.orb.two{
  width:300px;
  height:300px;
  left:-150px;
  bottom:-100px;
  animation-delay:-3s;
}

.orb.three{
  width:100px;
  height:100px;
  right:25%;
  bottom:15%;
  animation-delay:-5s;
}

@keyframes float{
  0%,100%{
    transform:translateY(0) rotate(0deg)
  }

  50%{
    transform:translateY(-25px) rotate(8deg)
  }
}

.hero-content{
  position:relative;
  z-index:2;
  max-width:850px;
  padding-top:70px;
}

.hero-kicker{
  display:flex;
  align-items:center;
  gap:12px;
  color:var(--gold);
  font-size:11px;
  letter-spacing:4px;
  font-weight:800;
  margin-bottom:25px;
}

.hero-kicker::before{
  content:"";
  width:45px;
  height:1px;
  background:var(--gold);
}

.hero h1{
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(70px,12vw,155px);
  line-height:.78;
  font-weight:600;
  letter-spacing:-5px;
  color:var(--dark);
}

.hero h1 em{
  display:block;
  color:var(--gold);
  font-weight:400;
}

.hero-desc{
  margin-top:35px;
  max-width:560px;
  color:var(--muted);
  line-height:1.9;
  font-size:15px;
}

.hero-actions{
  display:flex;
  gap:14px;
  margin-top:35px;
  flex-wrap:wrap;
}

.btn{
  border:0;
  cursor:pointer;
  padding:16px 25px;
  border-radius:3px;
  font-size:11px;
  letter-spacing:1.5px;
  font-weight:800;
  text-transform:uppercase;
  transition:.3s;
}

.btn-dark{
  background:var(--dark);
  color:white;
}

.btn-dark:hover{
  transform:translateY(-3px);
  box-shadow:0 15px 30px rgba(33,29,24,.18);
}

.btn-light{
  border:1px solid var(--line);
  background:transparent;
  color:var(--dark);
}

.btn-light:hover{
  background:white;
}

.hero-bottom{
  position:absolute;
  bottom:35px;
  left:50%;
  transform:translateX(-50%);
  font-size:9px;
  letter-spacing:3px;
  color:#958a7c;
}


/* STORY */

.story{
  background:var(--card);
}

.story-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:90px;
  align-items:center;
}

.story-art{
  min-height:560px;
  position:relative;
  overflow:hidden;
  background:
    linear-gradient(135deg,#d7c3a3,#f3eadc 48%,#9d7742);
  box-shadow:var(--shadow);
}

.story-art::before{
  content:"";
  position:absolute;
  width:360px;
  height:360px;
  border-radius:50%;
  border:1px solid rgba(255,255,255,.65);
  top:50%;
  left:50%;
  transform:translate(-50%,-50%);
}

.story-art::after{
  content:"HAN";
  position:absolute;
  font-family:"Cormorant Garamond",serif;
  font-size:180px;
  color:rgba(255,255,255,.30);
  left:50%;
  top:50%;
  transform:translate(-50%,-50%);
}

.story-card{
  position:absolute;
  bottom:25px;
  right:25px;
  background:rgba(255,253,248,.9);
  backdrop-filter:blur(10px);
  padding:22px 25px;
  width:210px;
}

.story-card strong{
  display:block;
  font-family:"Cormorant Garamond",serif;
  font-size:35px;
  color:var(--dark);
}

.story-card span{
  font-size:10px;
  color:var(--muted);
}


/* FEATURES */

.features{
  background:var(--bg2);
}

.feature-grid{
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:15px;
  margin-top:60px;
}

.feature{
  padding:35px 25px;
  background:rgba(255,253,248,.7);
  border:1px solid var(--line);
  transition:.35s;
}

.feature:hover{
  transform:translateY(-8px);
  box-shadow:var(--shadow);
}

.feature-number{
  font-size:10px;
  color:var(--gold);
  letter-spacing:2px;
}

.feature h3{
  font-family:"Cormorant Garamond",serif;
  font-size:30px;
  margin:30px 0 12px;
  color:var(--dark);
}

.feature p{
  font-size:12px;
  color:var(--muted);
  line-height:1.8;
}


/* MENU */

.menu-section{
  background:var(--card);
}

.menu-head{
  display:flex;
  justify-content:space-between;
  align-items:end;
  gap:30px;
  margin-bottom:50px;
}

.filters{
  display:flex;
  gap:8px;
  flex-wrap:wrap;
}

.filter{
  border:1px solid var(--line);
  background:transparent;
  color:var(--muted);
  padding:10px 15px;
  cursor:pointer;
  font-size:10px;
  font-weight:700;
  transition:.3s;
}

.filter.active,
.filter:hover{
  background:var(--dark);
  color:white;
  border-color:var(--dark);
}

.menu-grid{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:0 70px;
}

.menu-item{
  display:flex;
  justify-content:space-between;
  gap:20px;
  padding:25px 0;
  border-bottom:1px solid var(--line);
  animation:menuIn .35s ease;
}

@keyframes menuIn{
  from{
    opacity:0;
    transform:translateY(8px)
  }

  to{
    opacity:1;
    transform:none
  }
}

.menu-item h3{
  font-family:"Cormorant Garamond",serif;
  font-size:28px;
  color:var(--dark);
}

.menu-item p{
  color:var(--muted);
  font-size:11px;
  margin-top:5px;
}

.price{
  color:var(--gold);
  font-size:14px;
  font-weight:800;
  white-space:nowrap;
}


/* EXPERIENCE */

.experience{
  background:var(--dark);
  color:white;
}

.experience .section-title{
  color:white;
}

.experience .section-text{
  color:#b9afa0;
}

.experience-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:18px;
  margin-top:60px;
}

.experience-card{
  min-height:300px;
  padding:30px;
  border:1px solid rgba(255,255,255,.13);
  display:flex;
  flex-direction:column;
  justify-content:flex-end;
  position:relative;
  overflow:hidden;
  background:
    radial-gradient(circle at 70% 20%,rgba(196,154,84,.18),transparent 30%);
  transition:.4s;
}

.experience-card:hover{
  transform:translateY(-8px);
  border-color:rgba(196,154,84,.5);
}

.experience-card span{
  color:var(--gold2);
  font-size:10px;
  letter-spacing:3px;
  margin-bottom:auto;
}

.experience-card h3{
  font-family:"Cormorant Garamond",serif;
  font-size:38px;
  margin-bottom:10px;
}

.experience-card p{
  color:#aaa093;
  font-size:12px;
  line-height:1.7;
}


/* RESERVATION */

.reservation{
  background:var(--bg2);
}

.reservation-grid{
  display:grid;
  grid-template-columns:.8fr 1.2fr;
  gap:80px;
  align-items:start;
}

.reservation-info{
  position:sticky;
  top:120px;
}

.reservation-info .section-text{
  margin-top:25px;
}

.reservation-note{
  margin-top:35px;
  padding:22px;
  border-left:2px solid var(--gold);
  background:rgba(255,255,255,.45);
  color:var(--muted);
  font-size:11px;
  line-height:1.8;
}

.form-box{
  background:var(--card);
  padding:35px;
  box-shadow:var(--shadow);
}

.form-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:18px;
}

.field{
  display:flex;
  flex-direction:column;
  gap:8px;
}

.field.full{
  grid-column:1/-1;
}

.field label{
  color:#756d61;
  font-size:10px;
  letter-spacing:1px;
  font-weight:800;
  text-transform:uppercase;
}

.field input,
.field select,
.field textarea{
  width:100%;
  border:1px solid var(--line);
  background:#fffefa;
  padding:14px;
  outline:none;
  color:var(--dark);
  transition:.3s;
}

.field input:focus,
.field select:focus,
.field textarea:focus{
  border-color:var(--gold);
}

.field textarea{
  min-height:120px;
  resize:vertical;
}


/* KİŞİ SEÇİMLERİ */

.people-title{
  margin-top:30px;
  margin-bottom:15px;
  padding-bottom:12px;
  border-bottom:1px solid var(--line);
  font-family:"Cormorant Garamond",serif;
  font-size:32px;
  color:var(--dark);
}

.people-title span{
  color:var(--gold);
}

.people-container{
  display:grid;
  gap:14px;
}

.person-card{
  background:#f7f0e5;
  border:1px solid var(--line);
  padding:22px;
  position:relative;
  animation:personAppear .4s ease both;
}

@keyframes personAppear{
  from{
    opacity:0;
    transform:translateY(15px);
  }

  to{
    opacity:1;
    transform:translateY(0);
  }
}

.person-number{
  display:flex;
  align-items:center;
  gap:10px;
  margin-bottom:18px;
  color:var(--gold);
  font-size:10px;
  letter-spacing:2px;
  font-weight:800;
}

.person-number::after{
  content:"";
  height:1px;
  flex:1;
  background:var(--line);
}

.person-fields{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:14px;
}

.person-field{
  display:flex;
  flex-direction:column;
  gap:7px;
}

.person-field label{
  font-size:9px;
  color:var(--muted);
  text-transform:uppercase;
  letter-spacing:1px;
  font-weight:800;
}

.person-field input,
.person-field select{
  width:100%;
  padding:13px;
  border:1px solid var(--line);
  background:#fffdf8;
  color:var(--dark);
  outline:none;
}

.person-field input:focus,
.person-field select:focus{
  border-color:var(--gold);
}

.form-submit{
  margin-top:22px;
  width:100%;
}

.reservation-result{
  display:none;
  margin-top:20px;
  padding:25px;
  background:#f0e8da;
  border-left:3px solid var(--gold);
}

.reservation-result.show{
  display:block;
}

.reservation-result h3{
  font-family:"Cormorant Garamond",serif;
  font-size:32px;
  margin-bottom:15px;
}

.reservation-result p{
  font-size:12px;
  color:var(--muted);
  line-height:2;
}


/* FAQ */

.faq{
  background:var(--card);
}

.faq-grid{
  display:grid;
  grid-template-columns:.7fr 1.3fr;
  gap:80px;
  align-items:start;
}

.faq-list{
  border-top:1px solid var(--line);
}

.faq-item{
  border-bottom:1px solid var(--line);
}

.faq-question{
  width:100%;
  padding:24px 0;
  background:none;
  border:0;
  display:flex;
  justify-content:space-between;
  align-items:center;
  text-align:left;
  color:var(--dark);
  font-family:"Cormorant Garamond",serif;
  font-size:26px;
  cursor:pointer;
}

.faq-icon{
  font-family:"Manrope",sans-serif;
  font-size:20px;
  color:var(--gold);
  transition:.3s;
}

.faq-answer{
  max-height:0;
  overflow:hidden;
  color:var(--muted);
  line-height:1.8;
  font-size:13px;
  transition:max-height .4s ease,padding .4s ease;
}

.faq-item.open .faq-answer{
  max-height:220px;
  padding:0 0 24px;
}

.faq-item.open .faq-icon{
  transform:rotate(45deg);
}


/* CONTACT */

.contact{
  background:var(--bg2);
}

.contact-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:60px;
}

.contact-list{
  margin-top:40px;
  display:grid;
  gap:20px;
}

.contact-item{
  padding-bottom:20px;
  border-bottom:1px solid var(--line);
}

.contact-item span{
  display:block;
  font-size:9px;
  letter-spacing:2px;
  color:var(--gold);
  text-transform:uppercase;
  margin-bottom:7px;
}

.contact-item strong{
  color:var(--dark);
  font-size:14px;
}

.map-card{
  min-height:430px;
  background:
    linear-gradient(135deg,#dfd0b8,#f7f1e8);
  position:relative;
  overflow:hidden;
  display:flex;
  align-items:center;
  justify-content:center;
  box-shadow:var(--shadow);
}

.map-circle{
  width:230px;
  height:230px;
  border-radius:50%;
  border:1px solid rgba(167,123,50,.35);
  position:relative;
}

.map-circle::before,
.map-circle::after{
  content:"";
  position:absolute;
  inset:35px;
  border:1px solid rgba(167,123,50,.25);
  border-radius:50%;
}

.map-circle::after{
  inset:70px;
}

.map-pin{
  position:absolute;
  left:50%;
  top:50%;
  transform:translate(-50%,-50%);
  width:22px;
  height:22px;
  background:var(--gold);
  border-radius:50% 50% 50% 0;
  rotate:-45deg;
}

.map-label{
  position:absolute;
  bottom:25px;
  left:25px;
  background:rgba(255,253,248,.9);
  padding:15px 18px;
  font-size:11px;
}


/* FOOTER */

footer{
  background:#181512;
  color:white;
  padding:60px 0 30px;
}

.footer-top{
  display:flex;
  justify-content:space-between;
  gap:30px;
  align-items:end;
  padding-bottom:45px;
  border-bottom:1px solid rgba(255,255,255,.12);
}

.footer-logo{
  font-family:"Cormorant Garamond",serif;
  font-size:55px;
  letter-spacing:2px;
}

.footer-sub{
  color:#968d80;
  font-size:11px;
  margin-top:4px;
}

.footer-links{
  display:flex;
  gap:25px;
  flex-wrap:wrap;
}

.footer-links a{
  font-size:10px;
  color:#aaa195;
}

.footer-bottom{
  padding-top:25px;
  display:flex;
  justify-content:space-between;
  gap:20px;
  color:#746d64;
  font-size:9px;
  letter-spacing:.5px;
}

.burax{
  color:#d4ad69;
  font-weight:800;
  letter-spacing:2px;
}

.mobile-call{
  display:none;
}


/* REVEAL */

.reveal{
  opacity:0;
  transform:translateY(35px);
  transition:opacity .8s ease,transform .8s ease;
}

.reveal.visible{
  opacity:1;
  transform:none;
}


/* RESPONSIVE */

@media(max-width:900px){

  .nav-links{
    position:absolute;
    top:82px;
    left:4%;
    width:92%;
    background:rgba(255,253,248,.97);
    backdrop-filter:blur(20px);
    padding:25px;
    flex-direction:column;
    align-items:flex-start;
    gap:20px;
    box-shadow:var(--shadow);
    opacity:0;
    pointer-events:none;
    transform:translateY(-10px);
    transition:.3s;
  }

  .nav-links.open{
    opacity:1;
    pointer-events:auto;
    transform:none;
  }

  .menu-toggle{
    display:block;
  }

  .story-grid,
  .reservation-grid,
  .contact-grid,
  .faq-grid{
    grid-template-columns:1fr;
  }

  .feature-grid{
    grid-template-columns:1fr 1fr;
  }

  .experience-grid{
    grid-template-columns:1fr;
  }

  .reservation-info{
    position:static;
  }

  .menu-head{
    align-items:flex-start;
    flex-direction:column;
  }

  .story-art{
    min-height:400px;
  }

  .faq-grid{
    gap:40px;
  }
}


@media(max-width:600px){

  section{
    padding:80px 0;
  }

  .hero h1{
    font-size:72px;
    letter-spacing:-3px;
  }

  .hero{
    min-height:90vh;
  }

  .feature-grid{
    grid-template-columns:1fr;
  }

  .menu-grid{
    grid-template-columns:1fr;
  }

  .form-grid{
    grid-template-columns:1fr;
  }

  .field.full{
    grid-column:auto;
  }

  .person-fields{
    grid-template-columns:1fr;
  }

  .form-box{
    padding:22px;
  }

  .footer-top,
  .footer-bottom{
    flex-direction:column;
    align-items:flex-start;
  }

  .footer-logo{
    font-size:45px;
  }

  .mobile-call{
    display:block;
    position:fixed;
    bottom:18px;
    right:18px;
    z-index:999;
    background:var(--dark);
    color:white;
    padding:15px 18px;
    border-radius:50px;
    font-size:11px;
    font-weight:800;
    box-shadow:0 12px 30px rgba(0,0,0,.2);
  }

  .loader-brand{
    font-size:52px;
    letter-spacing:5px;
  }

}

</style>
</head>

<body>


<!-- =========================================
     GİRİŞ EKRANI
========================================= -->

<div class="loader">

  <div class="loader-content">

    <div class="loader-brand">
      HAN
    </div>

    <div class="loader-sub">
      ET HOUSE
    </div>

    <div class="loader-line"></div>

  </div>

</div>


<!-- =========================================
     NAVBAR
========================================= -->

<header class="navbar" id="navbar">

  <div class="nav-inner">

    <a href="#anasayfa" class="logo">

      HAN ET HOUSE

      <small>
        MEAT • FIRE • EXPERIENCE
      </small>

    </a>


    <button class="menu-toggle" id="menuToggle">
      ☰
    </button>


    <nav class="nav-links" id="navLinks">

      <a href="#anasayfa">Ana Sayfa</a>

      <a href="#hakkimizda">Hakkımızda</a>

      <a href="#menu">Menü</a>

      <a href="#deneyim">Deneyim</a>

      <a href="#rezervasyon">Rezervasyon</a>

      <a href="#sss">SSS</a>

      <a href="#iletisim">İletişim</a>

      <a href="#rezervasyon" class="nav-btn">
        Rezervasyon Yap
      </a>

    </nav>

  </div>

</header>


<!-- =========================================
     HERO
========================================= -->

<section class="hero" id="anasayfa">

  <div class="hero-bg">

    <div class="orb one"></div>
    <div class="orb two"></div>
    <div class="orb three"></div>

  </div>


  <div class="container">

    <div class="hero-content reveal">

      <div class="hero-kicker">
        TOKAT • PREMIUM STEAK HOUSE
      </div>

      <h1>
        HAN
        <em>ET HOUSE</em>
      </h1>

      <p class="hero-desc">
        Ateşin karakteri, seçkin etlerin lezzeti ve modern
        bir restoran deneyimi. HAN ET HOUSE'da sofranız
        sıradan bir yemek değil, özel bir deneyim olur.
      </p>

      <div class="hero-actions">

        <a href="#menu" class="btn btn-dark">
          Menüyü Keşfet
        </a>

        <a href="#rezervasyon" class="btn btn-light">
          Rezervasyon
        </a>

      </div>

    </div>

  </div>


  <div class="hero-bottom">
    SCROLL TO DISCOVER
  </div>

</section>


<!-- =========================================
     HAKKIMIZDA
========================================= -->

<section class="story" id="hakkimizda">

  <div class="container">

    <div class="story-grid">

      <div class="story-art reveal">

        <div class="story-card">

          <strong>HAN</strong>

          <span>
            Et • Ateş • Lezzet
          </span>

        </div>

      </div>


      <div class="reveal">

        <div class="section-label">
          Hakkımızda
        </div>

        <h2 class="section-title">
          Etin <span>gerçek</span><br>
          karakteri.
        </h2>

        <p class="section-text" style="margin-top:30px;">

          HAN ET HOUSE, kaliteli etleri modern bir restoran
          atmosferiyle buluşturan özel bir lezzet noktasıdır.
          Geleneksel Türk mutfağının güçlü taraflarını,
          özenli sunum ve premium restoran anlayışıyla
          bir araya getirir.

        </p>

        <p class="section-text" style="margin-top:18px;">

          Her tabakta sadelik, kalite ve lezzetin ön planda
          olduğu bir deneyim sunmayı amaçlar.

        </p>

      </div>

    </div>

  </div>

</section>


<!-- =========================================
     ÖZELLİKLER
========================================= -->

<section class="features">

  <div class="container">

    <div class="section-label reveal">
      HAN ET HOUSE FARKI
    </div>

    <h2 class="section-title reveal">
      Sadece yemek değil,<br>
      <span>deneyim.</span>
    </h2>


    <div class="feature-grid">

      <div class="feature reveal">

        <span class="feature-number">
          01
        </span>

        <h3>
          Seçkin Etler
        </h3>

        <p>
          Menüde öne çıkan dana ve kuzu etleriyle
          güçlü bir et deneyimi.
        </p>

      </div>


      <div class="feature reveal">

        <span class="feature-number">
          02
        </span>

        <h3>
          Ateş
        </h3>

        <p>
          Izgara kültürünün karakteristik lezzetini
          modern sunum anlayışıyla buluşturur.
        </p>

      </div>


      <div class="feature reveal">

        <span class="feature-number">
          03
        </span>

        <h3>
          Atmosfer
        </h3>

        <p>
          Özel buluşmalar ve keyifli sofralar için
          şık ve sıcak bir restoran atmosferi.
        </p>

      </div>


      <div class="feature reveal">

        <span class="feature-number">
          04
        </span>

        <h3>
          Lezzet
        </h3>

        <p>
          Ana yemeklerden tatlılara kadar dengeli
          ve zengin bir menü deneyimi.
        </p>

      </div>

    </div>

  </div>

</section>


<!-- =========================================
     MENÜ
========================================= -->

<section class="menu-section" id="menu">

  <div class="container">

    <div class="menu-head">

      <div>

        <div class="section-label reveal">
          Menü
        </div>

        <h2 class="section-title reveal">
          Sofranızı<br>
          <span>seçin.</span>
        </h2>

      </div>


      <div class="filters reveal">

        <button class="filter active" data-filter="all">
          Tümü
        </button>

        <button class="filter" data-filter="et">
          Etler
        </button>

        <button class="filter" data-filter="izgara">
          Kebap & Izgara
        </button>

        <button class="filter" data-filter="tatli">
          Tatlı
        </button>

      </div>

    </div>


    <div class="menu-grid" id="menuGrid">


      <div class="menu-item" data-category="et">

        <div>
          <h3>Dana Antrikot</h3>
          <p>Garnitür ile</p>
        </div>

        <div class="price">
          ₺1.100
        </div>

      </div>


      <div class="menu-item" data-category="et">

        <div>
          <h3>Dana Bonfile</h3>
          <p>Garnitür ile</p>
        </div>

        <div class="price">
          ₺1.100
        </div>

      </div>


      <div class="menu-item" data-category="et">

        <div>
          <h3>Kuzu Pirzola</h3>
          <p>Garnitür ile</p>
        </div>

        <div class="price">
          ₺1.000
        </div>

      </div>


      <div class="menu-item" data-category="et">

        <div>
          <h3>Kuzu Lokum</h3>
          <p>Özel kuzu eti</p>
        </div>

        <div class="price">
          ₺1.150
        </div>

      </div>


      <div class="menu-item" data-category="et">

        <div>
          <h3>Küşleme</h3>
          <p>Kuzu bonfile</p>
        </div>

        <div class="price">
          ₺1.100
        </div>

      </div>


      <div class="menu-item" data-category="izgara">

        <div>
          <h3>Izgara Köfte</h3>
          <p>Garnitür ile</p>
        </div>

        <div class="price">
          ₺550
        </div>

      </div>


      <div class="menu-item" data-category="izgara">

        <div>
          <h3>Adana Kebap</h3>
          <p>Garnitür ile</p>
        </div>

        <div class="price">
          ₺600
        </div>

      </div>


      <div class="menu-item" data-category="izgara">

        <div>
          <h3>Adana Dürüm</h3>
          <p>Yeşillik ve domates</p>
        </div>

        <div class="price">
          ₺300
        </div>

      </div>


      <div class="menu-item" data-category="tatli">

        <div>
          <h3>Ekmek Kadayıfı</h3>
          <p>Geleneksel tatlı</p>
        </div>

        <div class="price">
          ₺170
        </div>

      </div>


      <div class="menu-item" data-category="tatli">

        <div>
          <h3>Fırın Sütlaç</h3>
          <p>Fırında hazırlanır</p>
        </div>

        <div class="price">
          ₺200
        </div>

      </div>


    </div>

  </div>

</section>


<!-- =========================================
     DENEYİM
========================================= -->

<section class="experience" id="deneyim">

  <div class="container">

    <div class="section-label reveal">
      Deneyim
    </div>

    <h2 class="section-title reveal">
      Sofranızın<br>
      <span>hikâyesi.</span>
    </h2>


    <div class="experience-grid">

      <div class="experience-card reveal">

        <span>
          01 / LEZZET
        </span>

        <h3>
          Güçlü Tatlar
        </h3>

        <p>
          Etin doğal karakterini ön plana çıkaran
          güçlü ve dengeli lezzetler.
        </p>

      </div>


      <div class="experience-card reveal">

        <span>
          02 / SOFRA
        </span>

        <h3>
          Özel Anlar
        </h3>

        <p>
          Aile yemeklerinden arkadaş buluşmalarına
          kadar farklı sofralara uygun atmosfer.
        </p>

      </div>


      <div class="experience-card reveal">

        <span>
          03 / HAN
        </span>

        <h3>
          Modern Dokunuş
        </h3>

        <p>
          Geleneksel lezzetleri modern restoran
          anlayışıyla bir araya getiren yaklaşım.
        </p>

      </div>

    </div>

  </div>

</section>


<!-- =========================================
     REZERVASYON
========================================= -->

<section class="reservation" id="rezervasyon">

  <div class="container">

    <div class="reservation-grid">


      <div class="reservation-info reveal">

        <div class="section-label">
          Rezervasyon
        </div>

        <h2 class="section-title">
          Masanızı<br>
          <span>ayırın.</span>
        </h2>

        <p class="section-text">

          Tarih, saat, kişi sayısı ve her misafir için
          ayrı ayrı yemek tercihinizi belirterek
          rezervasyon talebinizi oluşturabilirsiniz.

        </p>

        <div class="reservation-note">

          Kişi sayısını seçtiğinizde her kişi için
          ayrı isim ve yemek seçme alanı otomatik
          olarak oluşturulur.

        </div>

      </div>


      <div class="form-box reveal">

        <form id="reservationForm">


          <div class="form-grid">


            <div class="field">

              <label>
                Rezervasyonu Yapan
              </label>

              <input
                type="text"
                id="name"
                placeholder="Adınız Soyadınız"
                required
              >

            </div>


            <div class="field">

              <label>
                Telefon
              </label>

              <input
                type="tel"
                id="phone"
                placeholder="05XX XXX XX XX"
                required
              >

            </div>


            <div class="field">

              <label>
                Tarih
              </label>

              <input
                type="date"
                id="date"
                required
              >

            </div>


            <div class="field">

              <label>
                Saat
              </label>

              <input
                type="time"
                id="time"
                required
              >

            </div>


            <div class="field">

              <label>
                Kişi Sayısı
              </label>

              <select id="people" required>

                <option value="">
                  Kişi sayısını seçiniz
                </option>

                <option value="1">
                  1 Kişi
                </option>

                <option value="2">
                  2 Kişi
                </option>

                <option value="3">
                  3 Kişi
                </option>

                <option value="4">
                  4 Kişi
                </option>

                <option value="5">
                  5 Kişi
                </option>

                <option value="6">
                  6 Kişi
                </option>

                <option value="7">
                  7 Kişi
                </option>

                <option value="8">
                  8 Kişi
                </option>

                <option value="9">
                  9 Kişi
                </option>

                <option value="10">
                  10 Kişi
                </option>

                <option value="11">
                  11 Kişi
                </option>

                <option value="12">
                  12 Kişi
                </option>

              </select>

            </div>


            <div class="field">

              <label>
                Özel Gün
              </label>

              <select id="occasion">

                <option>
                  Belirtmek istemiyorum
                </option>

                <option>
                  Doğum Günü
                </option>

                <option>
                  Yıldönümü
                </option>

                <option>
                  Aile Yemeği
                </option>

                <option>
                  Arkadaş Buluşması
                </option>

                <option>
                  İş Yemeği
                </option>

                <option>
                  Diğer
                </option>

              </select>

            </div>


          </div>


          <!-- KİŞİLER -->

          <div
            class="people-title"
            id="peopleTitle"
            style="display:none;"
          >
            Misafirleriniz
            <span>ve yemek seçimleri</span>
          </div>


          <div
            class="people-container"
            id="peopleContainer"
          ></div>


          <div class="field full" style="margin-top:20px;">

            <label>
              Genel Not
            </label>

            <textarea
              id="note"
              placeholder="Masa, özel istek veya başka bir notunuz varsa yazabilirsiniz..."
            ></textarea>

          </div>


          <button
            class="btn btn-dark form-submit"
            type="submit"
          >
            Rezervasyon Özeti Oluştur
          </button>


        </form>


        <!-- SONUÇ -->

        <div
          class="reservation-result"
          id="reservationResult"
        >

          <h3>
            Rezervasyon Özeti
          </h3>

          <p id="resultText"></p>

          <br>

          <a
            href="tel:+903562124888"
            class="btn btn-dark"
            style="display:inline-block;"
          >
            İşletmeyi Ara
          </a>

        </div>

      </div>

    </div>

  </div>

</section>


<!-- =========================================
     SSS
========================================= -->

<section class="faq" id="sss">

  <div class="container">

    <div class="faq-grid">


      <div class="reveal">

        <div class="section-label">
          SSS
        </div>

        <h2 class="section-title">
          Merak<br>
          <span>ettikleriniz.</span>
        </h2>

        <p class="section-text" style="margin-top:25px;">

          HAN ET HOUSE hakkında sık sorulan soruların
          cevaplarını burada bulabilirsiniz.

        </p>

      </div>


      <div class="faq-list reveal">


        <div class="faq-item">

          <button class="faq-question">

            Rezervasyon nasıl yapılır?

            <span class="faq-icon">
              +
            </span>

          </button>

          <div class="faq-answer">

            Rezervasyon bölümündeki formu doldurarak
            tarih, saat, kişi sayısı ve her misafir için
            ayrı yemek tercihinizi belirtebilirsiniz.
            Oluşan özet sonrasında işletmeyle iletişime
            geçerek rezervasyonunuzu kesinleştirebilirsiniz.

          </div>

        </div>


        <div class="faq-item">

          <button class="faq-question">

            Her kişi için farklı yemek seçebilir miyim?

            <span class="faq-icon">
              +
            </span>

          </button>

          <div class="faq-answer">

            Evet. Kişi sayısını seçtiğinizde her misafir
            için ayrı isim ve yemek seçim alanı oluşturulur.
            Böylece aynı masadaki herkes farklı bir yemek
            tercihi belirtebilir.

          </div>

        </div>


        <div class="faq-item">

          <button class="faq-question">

            Her kişinin adını kendisi yazabilir mi?

            <span class="faq-icon">
              +
            </span>

          </button>

          <div class="faq-answer">

            Evet. Rezervasyonu yapan kişi, masadaki
            misafirlerin isimlerini ayrı ayrı forma
            yazabilir ve her kişinin yemek tercihini
            belirleyebilir.

          </div>

        </div>


        <div class="faq-item">

          <button class="faq-question">

            HAN ET HOUSE nerede?

            <span class="faq-icon">
              +
            </span>

          </button>

          <div class="faq-answer">

            HAN ET HOUSE, Tokat'ta Sıtkı Ulaşoğlu
            bölgesinde bulunmaktadır. Güncel konum için
            iletişim bölümündeki harita bağlantısını
            kullanabilirsiniz.

          </div>

        </div>


        <div class="faq-item">

          <button class="faq-question">

            Menüde hangi yemekler bulunuyor?

            <span class="faq-icon">
              +
            </span>

          </button>

          <div class="faq-answer">

            Menüde Dana Antrikot, Dana Bonfile, Kuzu
            Pirzola, Kuzu Lokum, Küşleme, Izgara Köfte,
            Adana Kebap, Adana Dürüm ve tatlı seçenekleri
            bulunmaktadır.

          </div>

        </div>


        <div class="faq-item">

          <button class="faq-question">

            İletişim numarası nedir?

            <span class="faq-icon">
              +
            </span>

          </button>

          <div class="faq-answer">

            HAN ET HOUSE'a
            <strong>0356 212 48 88</strong>
            numarasından ulaşabilirsiniz.

          </div>

        </div>


      </div>

    </div>

  </div>

</section>


<!-- =========================================
     İLETİŞİM
========================================= -->

<section class="contact" id="iletisim">

  <div class="container">

    <div class="contact-grid">


      <div class="reveal">

        <div class="section-label">
          İletişim
        </div>

        <h2 class="section-title">
          Bizi<br>
          <span>bulun.</span>
        </h2>


        <div class="contact-list">


          <div class="contact-item">

            <span>
              Adres
            </span>

            <strong>
              Sıtkı Ulaşoğlu Bulvarı, Tokat
            </strong>

          </div>


          <div class="contact-item">

            <span>
              Telefon
            </span>

            <strong>

              <a href="tel:+903562124888">
                0356 212 48 88
              </a>

            </strong>

          </div>


          <div class="contact-item">

            <span>
              Instagram
            </span>

            <strong>
              @han_et_house
            </strong>

          </div>


        </div>

      </div>


      <div class="map-card reveal">

        <div class="map-circle">

          <div class="map-pin"></div>

        </div>


        <div class="map-label">
          TOKAT • HAN ET HOUSE
        </div>


        <a
          href="https://www.google.com/maps/search/?api=1&query=HAN+ET+HOUSE+Tokat"
          target="_blank"
          class="btn btn-dark"
          style="position:absolute;bottom:25px;right:25px;"
        >
          Haritada Aç
        </a>

      </div>


    </div>

  </div>

</section>


<!-- =========================================
     FOOTER
========================================= -->

<footer>

  <div class="container">


    <div class="footer-top">


      <div>

        <div class="footer-logo">
          HAN ET HOUSE
        </div>

        <div class="footer-sub">
          MEAT • FIRE • EXPERIENCE
        </div>

      </div>


      <div class="footer-links">

        <a href="#anasayfa">
          Ana Sayfa
        </a>

        <a href="#menu">
          Menü
        </a>

        <a href="#rezervasyon">
          Rezervasyon
        </a>

        <a href="#sss">
          SSS
        </a>

        <a href="#iletisim">
          İletişim
        </a>

      </div>


    </div>


    <div class="footer-bottom">

      <div>

        © <span id="year"></span>
        HAN ET HOUSE.
        Tüm hakları saklıdır.

      </div>


      <div>

        Website designed & developed by

        <span class="burax">
          BURAX
        </span>

      </div>

    </div>


  </div>

</footer>


<!-- MOBİL ARA -->

<a
  href="tel:+903562124888"
  class="mobile-call"
>
  ☎ Hemen Ara
</a>


<script>


/* =========================================
   NAVBAR
========================================= */

const navbar =
document.getElementById("navbar");

window.addEventListener("scroll",()=>{

  if(window.scrollY > 30){

    navbar.classList.add("scrolled");

  }else{

    navbar.classList.remove("scrolled");

  }

});


/* =========================================
   MOBİL MENÜ
========================================= */

const menuToggle =
document.getElementById("menuToggle");

const navLinks =
document.getElementById("navLinks");

menuToggle.addEventListener("click",()=>{

  navLinks.classList.toggle("open");

});


document.querySelectorAll(".nav-links a")
.forEach(link=>{

  link.addEventListener("click",()=>{

    navLinks.classList.remove("open");

  });

});


/* =========================================
   REVEAL
========================================= */

const observer =
new IntersectionObserver((entries)=>{

  entries.forEach(entry=>{

    if(entry.isIntersecting){

      entry.target.classList.add("visible");

    }

  });

},{
  threshold:.12
});


document.querySelectorAll(".reveal")
.forEach(el=>{

  observer.observe(el);

});


/* =========================================
   MENÜ FİLTRE
========================================= */

const filters =
document.querySelectorAll(".filter");

const menuItems =
document.querySelectorAll(".menu-item");


filters.forEach(filter=>{

  filter.addEventListener("click",()=>{

    filters.forEach(f=>{
      f.classList.remove("active");
    });

    filter.classList.add("active");

    const selected =
    filter.dataset.filter;


    menuItems.forEach(item=>{

      if(
        selected === "all" ||
        item.dataset.category === selected
      ){

        item.style.display = "flex";

      }else{

        item.style.display = "none";

      }

    });

  });

});


/* =========================================
   TARİH
========================================= */

const dateInput =
document.getElementById("date");

const today =
new Date();

const yyyy =
today.getFullYear();

const mm =
String(today.getMonth()+1).padStart(2,"0");

const dd =
String(today.getDate()).padStart(2,"0");

dateInput.min =
`${yyyy}-${mm}-${dd}`;


/* =========================================
   YEMEKLER
========================================= */

const meals = [

  "Dana Antrikot — ₺1.100",

  "Dana Bonfile — ₺1.100",

  "Kuzu Pirzola — ₺1.000",

  "Kuzu Lokum — ₺1.150",

  "Küşleme — ₺1.100",

  "Izgara Köfte — ₺550",

  "Adana Kebap — ₺600",

  "Adana Dürüm — ₺300",

  "Ekmek Kadayıfı — ₺170",

  "Fırın Sütlaç — ₺200"

];


/* =========================================
   KİŞİ SAYISI DEĞİŞİNCE ALAN OLUŞTUR
========================================= */

const peopleSelect =
document.getElementById("people");

const peopleContainer =
document.getElementById("peopleContainer");

const peopleTitle =
document.getElementById("peopleTitle");


peopleSelect.addEventListener("change",()=>{

  const count =
  Number(peopleSelect.value);


  peopleContainer.innerHTML = "";


  if(!count){

    peopleTitle.style.display = "none";

    return;

  }


  peopleTitle.style.display = "block";


  for(let i=1; i<=count; i++){

    const card =
    document.createElement("div");

    card.className =
    "person-card";


    card.style.animationDelay =
    `${(i-1)*0.05}s`;


    card.innerHTML = `

      <div class="person-number">
        KİŞİ ${i}
      </div>

      <div class="person-fields">

        <div class="person-field">

          <label>
            Ad Soyad
          </label>

          <input
            type="text"
            class="person-name"
            data-person="${i}"
            placeholder="Kişinin adı"
            required
          >

        </div>


        <div class="person-field">

          <label>
            Yemek Seçimi
          </label>

          <select
            class="person-meal"
            data-person="${i}"
            required
          >

            <option value="">
              Yemek seçiniz
            </option>

            ${meals.map(meal=>`
              <option value="${meal}">
                ${meal}
              </option>
            `).join("")}

          </select>

        </div>

      </div>

    `;


    peopleContainer.appendChild(card);

  }

});


/* =========================================
   REZERVASYON
========================================= */

const reservationForm =
document.getElementById("reservationForm");

const reservationResult =
document.getElementById("reservationResult");

const resultText =
document.getElementById("resultText");


reservationForm.addEventListener("submit",(e)=>{

  e.preventDefault();


  const name =
  document.getElementById("name").value;

  const phone =
  document.getElementById("phone").value;

  const date =
  document.getElementById("date").value;

  const time =
  document.getElementById("time").value;

  const people =
  document.getElementById("people").value;

  const occasion =
  document.getElementById("occasion").value;

  const note =
  document.getElementById("note").value ||
  "Belirtilmedi";


  const personNames =
  document.querySelectorAll(".person-name");

  const personMeals =
  document.querySelectorAll(".person-meal");


  const reservationNumber =
  "HAN-" +
  Math.floor(
    100000 +
    Math.random()*900000
  );


  let guestsHTML = "";


  personNames.forEach((input,index)=>{

    const guestName =
    input.value;

    const guestMeal =
    personMeals[index].value;


    guestsHTML += `

      <strong>
        ${index+1}. ${guestName}
      </strong>
      — ${guestMeal}
      <br>

    `;

  });


  resultText.innerHTML = `

    <strong>
      Rezervasyon No:
    </strong>
    ${reservationNumber}

    <br>

    <strong>
      Rezervasyonu Yapan:
    </strong>
    ${name}

    <br>

    <strong>
      Telefon:
    </strong>
    ${phone}

    <br>

    <strong>
      Tarih:
    </strong>
    ${date}

    <br>

    <strong>
      Saat:
    </strong>
    ${time}

    <br>

    <strong>
      Kişi Sayısı:
    </strong>
    ${people} kişi

    <br>

    <strong>
      Özel Gün:
    </strong>
    ${occasion}

    <br><br>

    <strong>
      MİSAFİRLER VE YEMEKLER
    </strong>

    <br>

    ${guestsHTML}

    <br>

    <strong>
      Genel Not:
    </strong>
    ${note}

  `;


  reservationResult.classList.add("show");


  reservationResult.scrollIntoView({

    behavior:"smooth",

    block:"center"

  });

});


/* =========================================
   FAQ
========================================= */

document.querySelectorAll(".faq-question")
.forEach(button=>{

  button.addEventListener("click",()=>{

    const item =
    button.parentElement;

    const isOpen =
    item.classList.contains("open");


    document.querySelectorAll(".faq-item")
    .forEach(other=>{

      other.classList.remove("open");

    });


    if(!isOpen){

      item.classList.add("open");

    }

  });

});


/* =========================================
   YIL
========================================= */

document.getElementById("year")
.textContent =
new Date().getFullYear();


</script>

</body>
</html>
