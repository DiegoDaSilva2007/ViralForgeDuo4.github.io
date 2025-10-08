<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>ViralForge Duo — Social Media & Web</title>
  <meta name="description" content="ViralForge Duo — We craft viral campaigns and build stunning websites. Book a call and let’s make your brand unforgettable." />
  <!-- Google Fonts -->
  <link href="C:\Users\Admin\Desktop" rel="stylesheet">
  <style>
    :root{
      --bg:#0f0f0f;
      --card:#131313;
      --accent1:#ff6ec4;
      --accent2:#7873f5;
      --white:#ffffff;
      --muted:#dcdcdc;
      --gradient: linear-gradient(90deg,var(--accent1),var(--accent2));

      /* Added variables for dynamic card hover */
      --card-hover-bg: rgba(241,196,15,0.15); /* default gold */
      --card-hover-border: rgba(241,196,15,0.3); /* default gold */
    }
    *{box-sizing:border-box;margin:0;padding:0}
    html,body{height:100%}
    body{
      font-family: "Poppins", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: var(--bg) url('https://www.transparenttextures.com/patterns/asfalt-dark.png') repeat;
      color:var(--white);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      -webkit-text-size-adjust:100%;
      line-height:1.5;
      scroll-behavior:smooth;
    }
    a{color:inherit;text-decoration:none}
    h1,h2,h3{font-family:"Noto Serif", "Times New Roman", serif; color:var(--accent1); margin-bottom:0.6rem}

/* ===== Container ===== */
.container {
  width: 90%;
  max-width: 1200px; /* keeps it from getting too wide on large screens */
  margin: 0 auto;
  padding: 20px;
}

    nav{
      position:sticky; top:0; z-index:1000;
      display:flex; align-items:center; justify-content:space-between;
      gap:1rem; padding:1rem 2rem;
      background: rgba(15,15,15,0.85);
      border-bottom:2px solid rgba(255,110,196,0.08);
      backdrop-filter: blur(6px);
    }
    .logo{
      display:flex; align-items:center; gap:12px; font-weight:700; color:var(--accent1);
    }
    .logo img{height:44px;width:44px;object-fit:cover;border-radius:8px; box-shadow: 0 6px 20px rgba(255,110,196,0.06)}
    nav ul{display:flex;gap:1.4rem;list-style:none;align-items:center}
    nav a{font-weight:600;opacity:0.95; padding:6px 0; transition:color .18s, opacity .18s}
    nav a:hover, nav a.active{color:var(--accent2); text-decoration:none}

    .hero{
      min-height:88vh;
      display:flex; flex-direction:column; align-items:center; justify-content:center;
      text-align:center; padding:2.2rem;
      position:relative;
    }
    .hero .hero-logo{width:140px; height:auto; border-radius:12px; margin-bottom:1rem; box-shadow: 0 12px 40px rgba(255,110,196,0.07)}
    .hero h1{font-size: clamp(2rem, 5vw, 4rem)}
    .hero p{color:var(--muted); max-width:760px; margin-top:.6rem; font-size clamp:1rem, 2.5vw, 1.5rem}
    .hero .cta-row{margin-top:1.8rem; display:flex; gap:1rem; align-items:center; flex-wrap:wrap}

    .btn{
      display:inline-block; padding:0.8rem 1.6rem; border-radius:10px; font-weight:700; cursor:pointer;
      border:none; background:transparent; color:#0b0b0b;
      background-image: var(--gradient); background-size:200% 200%;
      transition: transform .18s ease, box-shadow .18s ease, background-position .4s;
      box-shadow: 0 6px 18px rgba(0,0,0,0.45);
    }
    .btn:active{transform:translateY(1px)}
    .btn:hover{
      background-position:100% 0;
      box-shadow: 0 10px 30px rgba(255,110,196,0.3), 0 2px 6px rgba(0,0,0,0.6);
      outline: none;
    }
    .btn.ghost{
      background:transparent; color:var(--accent1); border:1px solid rgba(255,110,196,0.12);
      box-shadow:none;
    }
    .btn.ghost:hover{ box-shadow: 0 8px 28px rgba(255,110,196,0.06); color:var(--accent2) }

    section{padding:4.2rem 1.6rem; max-width:1200px; margin:0 auto}
    .container{max-width:1200px;margin:0 auto}
    .section-title{ text-align:center; margin-bottom:2rem}
    .section-title p{color:var(--muted); margin-top:.6rem}

    .grid{display:grid; gap:1.6rem}
    .grid.columns-3{grid-template-columns:repeat(3,1fr)}
    .card{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(0,0,0,0.02));
      border:1px solid rgba(255,110,196,0.04);
      padding:1.6rem; border-radius:12px; text-align:left;
      transition:0.3s;
      position: relative;
      z-index:1;
    }

    /* --- CORRECTED HOVER EFFECT USING THEME VARIABLES --- */
    .grid:hover .card:not(:hover){
      filter: blur(2px);
      transition: filter 0.3s;
    }

    .card:hover{
      filter: blur(0); 
      background: var(--card-hover-bg); /* dynamic hover background */
      border-color: var(--card-hover-border); /* dynamic hover border */
      transform: scale(1.08) translateY(-8px);
      box-shadow: 0 12px 30px rgba(0,0,0,0.35);
      z-index: 10;
    }

    .card h3{margin-bottom:0.25rem}
    .card p{color:var(--muted); margin-bottom:0.8rem}
    .price{font-size:1.45rem; font-weight:800; color:var(--accent2); margin-bottom:0.6rem}
    .features{list-style:none;padding-left:0; color:var(--muted); margin-bottom:1rem}
    .features li{margin:0.45rem 0; font-size:.96rem}

    .skills{
      display:flex; flex-direction:column; gap:25px; max-width:600px; margin:2rem auto;
    }
    .skill-bar{
      background:#222;
      border-radius:50px;
      overflow:hidden;
      height:25px;
    }
    .skill-progress{
      height:100%;
      width:0%;
      background: var(--gradient);
      border-radius:50px;
      transition: width 2s;
    }

   .dropdown { margin-bottom: 1rem; }
    .dropdown-btn {
      width: 100%;
      background: var(--card);
      color: var(--white);
      padding: 0.8rem 1rem;
      font-size: 1.05rem;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      text-align: left;
      display: flex;
      justify-content: space-between;
      align-items: center;
      transition: background 0.2s;
    }
    .dropdown-btn:hover { background: rgba(255,255,255,0.05); }
    .dropdown-content {
      display: none;
      flex-direction: column;
      margin-top: 0.5rem;
      gap: 0.5rem;
    }
    .dropdown-content a {
      padding: 0.5rem 1rem;
      background: var(--card);
      border-radius: 6px;
      color: var(--muted);
      font-size: 0.95rem;
      text-decoration: none;
      transition: background 0.2s, color 0.2s;
    }
    .dropdown-content a:hover { background: var(--accent1); color: var(--white); }
    .dropdown.active .dropdown-content { display: flex; }

    .contact-form{max-width:640px;margin:0 auto}
    .contact-form input,.contact-form textarea{
      width:100%; padding:0.9rem; border-radius:8px; border:1px solid rgba(255,255,255,0.04);
      background: rgba(255,255,255,0.02); color:var(--white); resize:vertical;
    }
    .small{font-size:.9rem;color:var(--muted)}

    footer{padding:2rem;text-align:center;border-top:1px solid rgba(255,110,196,0.05); color:var(--muted)}

    #robotAssistant{
      position:fixed;
      bottom:2rem;
      right:2rem;
      width:90px;
      height:90px;
      border-radius:50%;
      background:var(--gradient);
      box-shadow:0 12px 30px rgba(0,0,0,0.5);
      display:flex;align-items:center;justify-content:center;
      cursor:pointer;
      z-index:10000;
      transition:transform 0.3s, box-shadow 0.3s;
    }
    #robotAssistant:hover{
      transform:scale(1.1);
      box-shadow:0 16px 40px rgba(255,110,196,0.5);
    }
    #robotTooltip{
      position:fixed;
      bottom:7.5rem;
      right:2rem;
      max-width:220px;
      padding:0.7rem 1rem;
      border-radius:10px;
      background: rgba(20,20,20,0.95);
      color:#fff;
      font-size:0.9rem;
      box-shadow:0 8px 25px rgba(0,0,0,0.5);
      opacity:0;
      pointer-events:none;
      transition:opacity 0.3s;
      z-index:10001;
    }

    #themeSwitch{
      position:fixed;
      top:1rem;
      right:1rem;
      padding:0.6rem 1rem;
      border:none;
      border-radius:8px;
      background:var(--accent1);
      color:#fff;
      cursor:pointer;
      z-index:10002;
      font-weight:700;
      box-shadow:0 6px 16px rgba(0,0,0,0.4);
      transition: transform 0.2s, background 0.2s;
    }
    #themeSwitch:hover{transform:scale(1.05)}

    /* Small devices (phones) */
@media screen and (max-width: 768px) {
  .navbar ul {
    flex-direction: column;
    gap: 10px;
  }

  .hero {
    padding: 30px 10px;
  }

  .card {
    margin: 10px 0;
  }
}

/* Extra small devices (portrait phones) */
@media screen and (max-width: 480px) {
  .hero h1 {
    font-size: 2rem;
  }

  .hero p {
    font-size: 1rem;
  }

  button {
    width: 100%;
    padding: 12px;
  }
}
	
	/* --- Minigames Dropdown & Mobile Fix --- */
.portfolio-dropdowns {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}
.dropdown { flex: 1 1 200px; }
.dropdown.active .dropdown-content {
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.dropdown-content a {
  text-align: center;
  font-weight: 600;
}

/* --- Rock-Paper-Scissors Styles --- */
.rpsBtn {
  transition: transform 0.2s, box-shadow 0.2s;
  border-radius: 10px;
  border: 2px solid transparent;
}
.rpsBtn:hover {
  transform: scale(1.1);
  box-shadow: 0 8px 25px rgba(255,255,255,0.35);
  border-color: var(--accent2);
}
#minigameContent h2 {
  text-align: center;
  margin-bottom: 0.8rem;
  color: var(--accent2);
}
#minigameContent p { text-align: center; }

/* --- Modal Styling --- */
#minigameModal {
  display:none;
  position:fixed; top:0; left:0;
  width:100%; height:100%;
  background:linear-gradient(135deg,#1f1f1f,#111);
  z-index:100000;
  justify-content:center;
  align-items:center;
  overflow:auto;
  padding:20px;
}
#minigameContent {
  position:relative;
  background:#111;
  padding:25px;
  border-radius:15px;
  max-width:500px;
  width:100%;
  color:#fff;
  box-shadow:0 0 40px rgba(255,110,196,0.4);
}
#closeMinigame {
  position:absolute; top:10px; right:10px;
  background:red; border:none; border-radius:5px;
  color:#fff; padding:5px 10px; cursor:pointer;
}

/* Full-screen particle canvas */
#gold-particles {
  position: fixed;
  inset: 0;
  z-index: 0;             /* keep it behind everything */
  pointer-events: none;   /* clicks pass through */
  display: block;
}

/* === Responsive Media Queries === */

/* Large devices (laptops/desktops) */
@media screen and (min-width: 1200px) {
  .container { width: 95%; padding: 30px; }
  .grid.columns-3 { grid-template-columns: repeat(3, 1fr); }
  .hero h1 { font-size: 4rem; }
  .hero p { font-size: 1.5rem; }
}

/* Medium devices (tablets, 768px – 1199px) */
@media screen and (max-width: 1199px) and (min-width: 768px) {
  .container { width: 95%; padding: 25px; }
  .grid.columns-3 { grid-template-columns: repeat(2, 1fr); gap: 1.2rem; }
  .hero h1 { font-size: 3rem; }
  .hero p { font-size: 1.25rem; }
  .cta-row { flex-direction: column; gap: 0.8rem; }
  nav ul { gap: 1rem; }
  .skill-bar { height: 20px; }
}

/* Small devices (phones, 480px – 767px) */
@media screen and (max-width: 767px) {
  .container { width: 90%; padding: 20px; }
  .grid.columns-3 { grid-template-columns: 1fr; gap: 1rem; }
  .hero h1 { font-size: 2.2rem; line-height: 2.6rem; }
  .hero p { font-size: 1rem; line-height: 1.5rem; }
  .cta-row { flex-direction: column; gap: 0.8rem; width: 100%; }
  .btn { width: 100%; padding: 12px 0; }
  nav ul { flex-direction: column; gap: 0.6rem; margin-right: 0; }
  .skills { max-width: 100%; gap: 18px; }
  .skill-bar { height: 18px; }
  #robotAssistant { width: 70px; height: 70px; bottom: 1rem; right: 1rem; }
  #robotTooltip { bottom: 6rem; right: 1rem; max-width: 180px; font-size: 0.8rem; }
}

/* Extra small devices (portrait phones, max 480px) */
@media screen and (max-width: 480px) {
  .hero h1 { font-size: 2rem; }
  .hero p { font-size: 0.95rem; }
  nav ul { gap: 0.5rem; font-size: 0.9rem; }
  .cta-row { gap: 0.6rem; }
  .btn { font-size: 0.9rem; padding: 10px 0; }
  .skills { gap: 14px; }
  .skill-bar { height: 16px; }
  .section-title h2 { font-size: 1.6rem; }
  .card { padding: 1rem; }
  .price { font-size: 1.25rem; }
}

	
	
  </style>
</head>
<body>
<canvas id="gold-particles"></canvas>
<!-- NAVIGATION BAR -->
<nav style="position: fixed; top: 0; left: 0; right: 0; z-index: 1000; display: flex; align-items: center; justify-content: space-between; background-color: black; padding: 10px 40px;">
  <!-- Logo Section -->
  <div class="logo" style="display: flex; align-items: center; gap: 10px;">
    <img src="logo.png" alt="Logo" style="height: 45px;" />
    <div style="color: white; font-weight: bold; font-size: 18px;">ViralForge Duo</div>
  </div>

  <!-- Navigation Links -->
  <ul style="display: flex; justify-content: center; list-style: none; margin: 0; padding: 0; gap: 25px; flex: 1; margin-right: 60px;">
    <li><a href="#home" class="nav-link active" style="color: white; text-decoration: none;">Home</a></li>
    <li><a href="#services" class="nav-link" style="color: white; text-decoration: none;">Services</a></li>
    <li><a href="#pricing" class="nav-link" style="color: white; text-decoration: none;">Pricing</a></li>
    <li><a href="#portfolio" class="nav-link" style="color: white; text-decoration: none;">Portfolio</a></li>
    <li><a href="#about" class="nav-link" style="color: white; text-decoration: none;">About</a></li>
    <li><a href="#contact" class="nav-link" style="color: white; text-decoration: none;">Contact</a></li>
  </ul>

  <!-- Theme Switcher -->
  <button id="themeSwitch" style="margin-left: 20px;">Switch Theme</button>
</nav>

<!-- HERO -->
<header id="home" class="hero">
  <img src="logo.png" alt="ViralForge large logo with slogan" class="hero-logo">
  <h1>We Forge Digital Greatness — crafted for creators, built for connection.</h1>
  <p>We combine creative storytelling, performance marketing and pixel-perfect design to help brands get noticed, booked and remembered. If you want consistent leads, scalable campaigns and websites that convert — you’re in the right place.</p>

  <div class="cta-row">
    <button class="btn" onclick="location.href='#contact'">Book a Call</button>
    <a class="btn ghost" href="#portfolio">View Work</a>
  </div>
</header>

  <!-- SERVICES -->
  <section id="services" class="container">
    <div class="section-title">
      <h2>Our Services</h2>
      <p>From single-project launches to full-service campaigns — we help brands reach real people and real results.</p>
    </div>

    <div class="grid columns-3" style="margin-top:1rem">
      <div class="card">
        <h3>Social Media Ads</h3>
        <p>Create targeted paid campaigns for Facebook, Instagram & TikTok that scale at profit.</p>
        <ul class="features">
          <li>A/B ad creative & copy</li>
          <li>Audience research & targeting</li>
          <li>Weekly performance reports</li>
        </ul>
        <div class="small">Ideal if you want consistent leads & sales from social platforms.</div>
      </div>

      <div class="card">
        <h3>Website Creation</h3>
        <p>Fast, responsive sites built for conversions — landing pages, portfolios, and full sites.</p>
        <ul class="features">
          <li>SEO-friendly structure</li>
          <li>Mobile-first responsive design</li>
          <li>CMS or static builds (your choice)</li>
        </ul>
        <div class="small">Perfect for brands that need a professional online presence fast.</div>
      </div>

      <div class="card">
        <h3>Website Maintenance & Support</h3>
        <p>Keep your site secure, updated and fast — we handle updates so you don’t have to.</p>
        <ul class="features">
          <li>Security & uptime checks</li>
          <li>Speed optimisation</li>
          <li>Content updates & backups</li>
        </ul>
        <div class="small">A great add-on for clients who want ongoing peace of mind.</div>
      </div>
    </div>
</br>
 <h2 align="center">Our Skills</h2>

    <!-- Skills Section -->
    <div class="skills">
      <div>
        <p>HTML / CSS / JS</p>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 95%;"></div>
        </div>
      </div>
      <div>
        <p>Responsive Design</p>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 90%;"></div>
        </div>
      </div>
      <div>
        <p>Web Animations</p>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 85%;"></div>
        </div>
      </div>
      <div>
        <p>Editing Skills</p>
        <div class="skill-bar">
          <div class="skill-progress" style="width: 98%;"></div>
        </div>
      </div>
    </div>
  </section>

  <!-- PRICING -->
  <section id="pricing" class="container" style="padding-top:2rem">
    <div class="section-title">
      <h2>Pricing & Packages</h2>
      <p>Simple, transparent pricing so you can pick the package that fits your goals.</p>
    </div>

    <div class="grid columns-3" style="margin-top:1rem">
      <!-- Starter -->
      <div class="card">
        <h3>Starter</h3>
        <p class="price">R5,000</p>
        <p>Launch a clean, high-converting presence for your business.</p>
        <ul class="features">
          <li>Single-page or 3-page website</li>
          <li>Basic on-page SEO</li>
          <li>Social profile setup (1 platform)</li>
          <li>1 round of revisions</li>
        </ul>
        <button class="btn" onclick="book('Starter',5000)">Choose Starter</button>
      </div>

      <!-- Growth -->
      <div class="card">
        <h3>Growth</h3>
        <p class="price">R10,000</p>
        <p>For brands ready to scale — website + social campaigns that start converting.</p>
        <ul class="features">
          <li>5–8 page responsive website</li>
          <li>Ad campaign setup (1 platform)</li>
          <li>Monthly performance report (1 month)</li>
          <li>2 rounds of revisions</li>
        </ul>
        <button class="btn" onclick="book('Growth',10000)">Choose Growth</button>
      </div>

      <!-- Premium -->
      <div class="card">
        <h3>Premium</h3>
        <p class="price">R15,000</p>
        <p>Full-service marketing & design for brands who want sustained growth.</p>
        <ul class="features">
          <li>Custom website + SEO groundwork</li>
          <li>Multi-platform ad campaigns</li>
          <li>Monthly optimisation & reporting (3 months)</li>
          <li>Priority support</li>
        </ul>
        <button class="btn" onclick="book('Premium',15000)">Choose Premium</button>
      </div>
    </div>
  </section>

 <!-- Portfolio -->
<section id="portfolio" class="container">
  <div class="section-title">
    <h2>Portfolio</h2>
    <p>TO BE CONTINUED!</p>
  </div>

  <!-- Sub-headings with dropdowns -->
  <div class="portfolio-dropdowns" style="margin-top:1rem;">
    <div class="dropdown">
      <button class="dropdown-btn">Minigames ▼</button>
      <div class="dropdown-content">
        <a href="#">Rock, Paper, Scissors</a>
        <a href="#">Flappy Bird</a>
      </div>
    </div>

    <div class="dropdown">
      <button class="dropdown-btn">3D Models ▼</button>
      <div class="dropdown-content">
        <a href="#">Add 3D Model 1</a>
        <a href="#">Add 3D Model 2</a>
      </div>
    </div>

    <div class="dropdown">
      <button class="dropdown-btn">Buttons ▼</button>
      <div class="dropdown-content">
        <a href="#">Button Example 1</a>
        <a href="#">Button Example 2</a>
      </div>
    </div>
  </div>
</section>


  <!-- ABOUT -->
  <section id="about" class="container">
    <div class="section-title">
      <h2>About ViralForge Duo</h2>
      <p>We’re Rikus & team — a tight-knit creative studio focused on growth, aesthetics and measurable impact.</p>
    </div>

    <p style="color:var(--muted);max-width:900px;margin:0 auto;text-align:center">
      We turn ideas into attention: strategy-first thinking, eye-catching creative and marketing that turns viewers into customers. Our approach is tailored, transparent and focused on your business goals — not vanity metrics.
    </p>
  </section>

  <!-- CONTACT -->
<section id="contact" class="container">
  <div class="section-title">
    <h2>Contact & Bookings</h2>
    <p>Ready to start? Book a call, send a message, or hit us on WhatsApp for a quick quote.</p>
  </div>

  <div class="contact-form" style="margin-top:1rem">
    <form id="contactForm" action="mailto:ViralForgeDuo@gmail.com" method="post" enctype="text/plain">
      <input id="name" name="name" type="text" placeholder="Your name" required>
      <input id="email" name="email" type="email" placeholder="Email address" required>
      <textarea id="message" name="message" rows="5" placeholder="Tell us about your project" required></textarea>

      <div style="display:flex;gap:10px;margin-top:.6rem;flex-wrap:wrap">
        <button class="btn" type="submit">Send Message</button>
        <a class="btn ghost" href="https://wa.me/27660542468" target="_blank" rel="noopener">Chat on WhatsApp</a>
      </div>

      <div id="formMessage" class="small" style="margin-top:.6rem"></div>
    </form>
  </div>
</section>

<footer>
  <div>&copy; <span id="year"></span> ViralForge Duo — All rights reserved.</div>
</footer>

<!-- Robot Assistant -->
<div id="robotAssistant">🤖</div>
<div id="robotTooltip">Hi, I'm your digital assistant!</div>

<script>
  // set copyright year
  document.getElementById('year').textContent = new Date().getFullYear();

  // Smooth scroll & active nav highlight
  const navLinks = document.querySelectorAll('.nav-link');
  navLinks.forEach(link => {
    link.addEventListener('click', e => {
      e.preventDefault();
      document.querySelector(link.getAttribute('href')).scrollIntoView({behavior:'smooth', block:'start'});
      navLinks.forEach(l=>l.classList.remove('active')); link.classList.add('active');
    });
  });

  // Minimal active link on scroll
  window.addEventListener('scroll', () => {
    const curPos = window.scrollY + 150;
    document.querySelectorAll('section').forEach(section => {
      if(curPos >= section.offsetTop && curPos < section.offsetTop + section.offsetHeight){
        navLinks.forEach(l=>l.classList.remove('active'));
        const a = document.querySelector('a[href="#'+section.id+'"]');
        if(a) a.classList.add('active');
      }
    });
    updateRobotTooltip();
  });

  // package booking helper
  function book(pkg, price){
    const msg = `Hi — I'm interested in the ${pkg} package (${price}). Please contact me to discuss next steps.`;
    document.getElementById('message').value = msg;
    location.href = '#contact';
    document.getElementById('name').focus();
  }

  // Skills animation
  const skillBars = document.querySelectorAll('.skill-progress');
  window.addEventListener('load', () => {
    skillBars.forEach(bar => {
      const width = bar.style.width;
      bar.style.width = '0%';
      setTimeout(() => { bar.style.width = width; }, 100);
    });
  });

  // Robot Tooltip
  const robot = document.getElementById('robotAssistant');
  const tooltip = document.getElementById('robotTooltip');

  robot.addEventListener('mouseenter', () => tooltip.style.opacity = 1);
  robot.addEventListener('mouseleave', () => tooltip.style.opacity = 0);

  const sections = [
    {id:'home', text:'Welcome! I’m your digital assistant.'},
    {id:'services', text:'Here are all our services: Social Media, Website Creation, and Maintenance.'},
    {id:'pricing', text:'These are our pricing packages and estimated project ranges.'},
    {id:'portfolio', text:'Check out our portfolio of recent projects!'},
    {id:'about', text:'Learn about ViralForge Duo and our approach.'},
    {id:'contact', text:'Contact us for inquiries or bookings!'}
  ];

  function updateRobotTooltip(){
    const scrollPos = window.scrollY + window.innerHeight/2;
    let currentText = 'Hi, I’m your digital assistant!';
    sections.forEach(section => {
      const el = document.getElementById(section.id);
      if(el && scrollPos >= el.offsetTop && scrollPos < el.offsetTop + el.offsetHeight){
        currentText = section.text;
      }
    });
    tooltip.textContent = currentText;
  }

   // Toggle dropdowns
    document.querySelectorAll('.dropdown-btn').forEach(btn => {
      btn.addEventListener('click', () => {
        const parent = btn.parentElement;
        parent.classList.toggle('active');
      });
    });



  // Theme Switcher
  const themeSwitchBtn = document.getElementById('themeSwitch');
  let goldTheme = true;
  document.documentElement.style.setProperty('--accent1', '#f1c40f'); // gold
  document.documentElement.style.setProperty('--accent2', '#f39c12');
  document.documentElement.style.setProperty('--card-hover-bg', 'rgba(241,196,15,0.15)');
  document.documentElement.style.setProperty('--card-hover-border', 'rgba(241,196,15,0.3)');
  themeSwitchBtn.style.background = '#f1c40f';

  themeSwitchBtn.addEventListener('click', () => {
    if(goldTheme){
      document.documentElement.style.setProperty('--accent1', '#9b59b6'); // purple
      document.documentElement.style.setProperty('--accent2', '#8e44ad');
      document.documentElement.style.setProperty('--card-hover-bg', 'rgba(155,89,182,0.15)'); // purple hover
      document.documentElement.style.setProperty('--card-hover-border', 'rgba(155,89,182,0.3)');
      themeSwitchBtn.style.background = '#9b59b6';
      goldTheme = false;
    } else {
      document.documentElement.style.setProperty('--accent1', '#f1c40f'); // gold
      document.documentElement.style.setProperty('--accent2', '#f39c12');
      document.documentElement.style.setProperty('--card-hover-bg', 'rgba(241,196,15,0.15)');
      document.documentElement.style.setProperty('--card-hover-border', 'rgba(241,196,15,0.3)');
      themeSwitchBtn.style.background = '#f1c40f';
      goldTheme = true;
    }
  });
  
  
  
  
</script>
<!-- Minigames Modal -->
<div id="minigameModal">
  <div id="minigameContent">
    <button id="closeMinigame">X</button>
    <div id="minigameInner"></div>
  </div>
</div>

<script>
const dropdownLinks = document.querySelectorAll('.dropdown-content a');
const modal = document.getElementById('minigameModal');
const modalInner = document.getElementById('minigameInner');
const closeBtn = document.getElementById('closeMinigame');

closeBtn.addEventListener('click', () => {
  modal.style.display = 'none';
  modalInner.innerHTML = '';
});

dropdownLinks.forEach(link => {
  link.addEventListener('click', e => {
    e.preventDefault();
    const text = link.textContent.trim();
    if(text === "Rock, Paper, Scissors"){
      openRPS();
    } else if(text === "Flappy Bird"){
      openFlappy();
    }
  });
});

/* --- ROCK PAPER SCISSORS --- */
function openRPS(){
  modal.style.display = 'flex';
  modalInner.innerHTML = `
    <h2 style="text-align:center; margin-bottom:10px;">Rock Paper Scissors</h2>
    <p style="text-align:center;">Choose your move:</p>
    <div style="display:flex; gap:20px; justify-content:center; flex-wrap:wrap; margin:20px 0;">
      <img src="Rock.png" alt="Rock" class="rpsBtn" style="width:120px; max-width:30vw; cursor:pointer;">
      <img src="Paper.jpg" alt="Paper" class="rpsBtn" style="width:120px; max-width:30vw; cursor:pointer;">
      <img src="Scissors.jpg" alt="Scissors" class="rpsBtn" style="width:120px; max-width:30vw; cursor:pointer;">
    </div>
    <p id="rpsResult" style="margin-top:15px; font-weight:bold; text-align:center;"></p>
    <p style="margin-top:10px; text-align:center;">Score — You: <span id="rpsUser">0</span> | Bot: <span id="rpsBot">0</span></p>
  `;


  let userScore = 0, botScore = 0;
  const buttons = modalInner.querySelectorAll('.rpsBtn');
  const resultP = document.getElementById('rpsResult');
  const userSpan = document.getElementById('rpsUser');
  const botSpan = document.getElementById('rpsBot');

  buttons.forEach(btn => {
    btn.addEventListener('click', () => {
      const userChoice = btn.alt;
      const choices = ["Rock","Paper","Scissors"];
      const botChoice = choices[Math.floor(Math.random()*3)];
      let outcome = '';

      if(userChoice === botChoice){
        outcome = "Draw!";
      } else if(
        (userChoice === "Rock" && botChoice === "Scissors") ||
        (userChoice === "Paper" && botChoice === "Rock") ||
        (userChoice === "Scissors" && botChoice === "Paper")
      ){
        outcome = "You win!";
        userScore++;
      } else {
        outcome = "Bot wins!";
        botScore++;
      }

      resultP.textContent = `You chose ${userChoice}, Bot chose ${botChoice}. ${outcome}`;
      userSpan.textContent = userScore;
      botSpan.textContent = botScore;
    });
  });
}

/* --- ADVANCED FLAPPY BIRD (Mario-inspired, drawn shapes, sounds, coins, powerups) --- */
function openFlappy(){
  modal.style.display = 'flex';
  modalInner.innerHTML = `
    <h2>Flappy Bird Deluxe — Mushroom Run</h2>
    <canvas id="flappyCanvas" width="350" height="500" style="background:linear-gradient(to bottom,#7ec8ff,#4facfe); display:block; margin:auto; border-radius:12px;"></canvas>
    <p style="text-align:center;">Score: <span id="flappyScore">0</span> | Best: <span id="bestScore">0</span></p>
    <p style="text-align:center; font-size:0.8rem; margin-top:5px;">Press <strong>SPACE</strong> or tap to jump! (M toggles sound)</p>
    <div style="text-align:center; margin-top:6px;">
      <button id="flappyToggleSound" style="padding:6px 10px;border-radius:8px;border:none;background:#ffd54a;cursor:pointer;">Mute</button>
    </div>
  `;

  const canvas = document.getElementById('flappyCanvas');
  const ctx = canvas.getContext('2d');
  const scoreEl = document.getElementById('flappyScore');
  const bestEl = document.getElementById('bestScore');
  const soundBtn = document.getElementById('flappyToggleSound');

  const W = canvas.width, H = canvas.height;
  // Game variables
  let bird = { x:80, y:H/2, w:30, h:26, dy:0, rot:0, flapTimer:0 };
  let gravity = 0.55, jump = -9.2;
  let pipes = [], coins = [], particles = [], powerups = [];
  let frame = 0, score = 0, best = parseInt(localStorage.getItem('flappyBest') || '0', 10);
  let speed = 2.6, baseGap = 120, spawnRate = 120;
  let playing = false, gameOver = false;
  let audioOn = true;

  bestEl.textContent = best;

  // WebAudio simple synth
  const AudioCtx = window.AudioContext || window.webkitAudioContext;
  const audioCtx = AudioCtx ? new AudioCtx() : null;
  function playBeep(freq=440, type='sine', t=0.08, vol=0.08){
    if(!audioOn || !audioCtx) return;
    const o = audioCtx.createOscillator();
    const g = audioCtx.createGain();
    o.type = type; o.frequency.value = freq;
    g.gain.value = vol;
    o.connect(g); g.connect(audioCtx.destination);
    o.start();
    g.gain.exponentialRampToValueAtTime(0.0001, audioCtx.currentTime + t);
    setTimeout(()=>{ try{ o.stop(); o.disconnect(); g.disconnect(); }catch(e){} }, (t+0.02)*1000);
  }
  function playMultiChord(freqs, type='sine', t=0.12, vol=0.06){
    if(!audioOn || !audioCtx) return;
    freqs.forEach((f, i) => setTimeout(()=> playBeep(f, type, t, vol), i*10));
  }

  // Utility
  const rand = (a,b) => Math.random()*(b-a)+a;
  const clamp = (v,a,b) => Math.max(a, Math.min(b, v));

  // Parallax layers (clouds and hills)
  const layers = [
    { speed: 0.18, items: [] },
    { speed: 0.45, items: [] },
    { speed: 1.0, items: [] }
  ];
  function initParallax(){
    layers[0].items = Array.from({length:6}, (_,i)=>({ x:i*(W/3)+rand(0,60), y:40+rand(0,30), s:30+rand(8,30) }));
    layers[1].items = Array.from({length:5}, (_,i)=>({ x:i*(W/2)+rand(0,80), y:120+rand(0,30), s:50+rand(10,40) }));
    layers[2].items = Array.from({length:4}, (_,i)=>({ x:i*(W/1.5)+rand(0,100), y:220+rand(0,30), s:70+rand(20,40) }));
  }
  initParallax();

  // Particles
  function spawnParticle(x,y,color,life=520){
    particles.push({ x, y, vx:rand(-2,2), vy:rand(-3.5,-0.4), r:rand(2,5), color, life, born:performance.now() });
  }

  // Spawn pipe and sometimes coin cluster or power-up (mushroom)
  function spawnPipe(){
    const top = rand(44, 230);
    const gap = baseGap + rand(-14, 24) * (1 + Math.floor(score/12) * 0.05);
    const bottom = H - top - gap - 40; // ground height considered
    pipes.push({ x: W + 12, w:54, top, bottom, passed:false });

    // coins cluster sometimes if gap allows
    if(Math.random() < 0.6 && gap > 80){
      const cx = W + 12 + 24;
      const coinCount = Math.floor(rand(1,4));
      for(let i=0;i<coinCount;i++){
        coins.push({ x: cx + i*(18), y: top + gap/2 - (coinCount*8) + i*8, r:6, collected:false });
      }
    }
    // small chance spawn powerup mushroom between pipes (gives score multiplier)
    if(Math.random() < 0.08){
      const puY = top + gap/2 + rand(-16,16);
      powerups.push({ x: W + 12 + 10, y: puY, r:9, taken:false, born: performance.now() });
    }
  }

  // Reset game state
  function resetGame(){
    bird.y = H/2; bird.dy = 0; bird.rot = 0; bird.flapTimer = 0;
    pipes = []; coins = []; particles = []; powerups = [];
    frame = 0; score = 0; speed = 2.6; baseGap = 120; spawnRate = 120;
    playing = false; gameOver = false;
    scoreEl.textContent = score;
    initParallax();
  }

  // Draw background (sky + parallax items)
  function drawBackground(){
    const grad = ctx.createLinearGradient(0,0,0,H);
    grad.addColorStop(0, '#7ec8ff'); grad.addColorStop(1, '#4facfe');
    ctx.fillStyle = grad; ctx.fillRect(0,0,W,H);

    // parallax layers (clouds/hills)
    layers.forEach((layer, idx) => {
      layer.items.forEach(it => {
        it.x -= layer.speed * speed * 0.32;
        if(it.x < -200) it.x = W + rand(0,100);
        if(idx < 2){
          // cloud
          ctx.fillStyle = idx === 0 ? '#ffffff' : 'rgba(255,255,255,0.9)';
          ctx.beginPath(); ctx.ellipse(it.x, it.y, it.s, it.s*0.6, 0, 0, Math.PI*2); ctx.fill();
        } else {
          // distant hill (green)
          ctx.fillStyle = '#79d18a';
          ctx.beginPath();
          ctx.moveTo(it.x - it.s, it.y + it.s/2);
          ctx.quadraticCurveTo(it.x, it.y - it.s/1.2, it.x + it.s, it.y + it.s/2);
          ctx.closePath(); ctx.fill();
        }
      });
    });
  }

  // Draw ground with tile blocks (Mario-ish)
  function drawGround(){
    ctx.fillStyle = '#8b5a2b';
    ctx.fillRect(0,H-40,W,40);
    // brick tiles
    const tileW = 26;
    for(let i=0;i < W; i += tileW){
      ctx.fillStyle = '#b5651d';
      ctx.fillRect(i, H-40, tileW-6, 18);
      // small top edge
      ctx.fillStyle = '#5b391f';
      ctx.fillRect(i, H-22, tileW-6, 6);
    }
  }

  // Draw pipes (green warp pipes)
  function drawPipes(){
    pipes.forEach(p => {
      // body
      ctx.fillStyle = '#2c8b3a';
      ctx.fillRect(p.x, 0, p.w, p.top);
      ctx.fillRect(p.x, H - p.bottom, p.w, p.bottom);
      // rim caps
      ctx.fillStyle = '#1e5e2b';
      ctx.fillRect(p.x - 6, p.top - 16, p.w + 12, 16);
      ctx.fillRect(p.x - 6, H - p.bottom, p.w + 12, 16);
      // subtle lines
      ctx.strokeStyle = 'rgba(0,0,0,0.08)';
      ctx.lineWidth = 1;
      for(let y = 0; y < p.top; y += 18){
        ctx.beginPath(); ctx.moveTo(p.x, y+9); ctx.lineTo(p.x + p.w, y+9); ctx.stroke();
      }
    });
  }

  // Draw coins
  function drawCoins(){
    coins.forEach(c => {
      if(c.collected) return;
      ctx.save();
      ctx.translate(c.x, c.y);
      ctx.beginPath();
      ctx.fillStyle = '#ffd54a';
      ctx.ellipse(0, 0, c.r, c.r*0.86, 0, 0, Math.PI*2);
      ctx.fill();
      ctx.fillStyle = '#fff';
      ctx.font = '8px monospace';
      ctx.textAlign = 'center';
      ctx.fillText('C', 0, 3);
      ctx.restore();
    });
  }

  // Draw powerups (mushroom)
  function drawPowerups(now){
    powerups.forEach(pu => {
      if(pu.taken) return;
      // bobbing
      const bob = Math.sin((now - pu.born)/300) * 4;
      ctx.save();
      ctx.translate(pu.x, pu.y + bob);
      // stem
      ctx.fillStyle = '#fff7e6';
      ctx.fillRect(-3, 3, 6, 6);
      // cap
      ctx.beginPath();
      ctx.fillStyle = '#ff4d4d';
      ctx.ellipse(0, -2, pu.r+2, pu.r, 0, 0, Math.PI*2);
      ctx.fill();
      ctx.fillStyle = '#fff';
      ctx.font = '8px sans-serif';
      ctx.textAlign = 'center';
      ctx.fillText('M', 0, 2);
      ctx.restore();
    });
  }

  // Draw bird with Mario-style cap
  function drawBird(now){
    ctx.save();
    ctx.translate(bird.x, bird.y);
    ctx.rotate(bird.rot);
    // body
    ctx.fillStyle = '#ff6b6b';
    ctx.beginPath(); ctx.ellipse(0,0, bird.w/2, bird.h/2, 0, 0, Math.PI*2); ctx.fill();
    // belly
    ctx.fillStyle = '#ffe6e6'; ctx.beginPath(); ctx.ellipse(4,2, bird.w/3.2, bird.h/3.6, 0, 0, Math.PI*2); ctx.fill();
    // cap (Mario-ish)
    ctx.fillStyle = '#c62828'; ctx.beginPath(); ctx.ellipse(-7,-8, 14,6, 0, Math.PI, 0); ctx.fill();
    // visor
    ctx.fillStyle = '#7b1f1f'; ctx.fillRect(-12,-6,12,4);
    // eye
    ctx.fillStyle = '#111'; ctx.beginPath(); ctx.arc(4,-2,3,0,Math.PI*2); ctx.fill();
    // small wing flap animation
    const flap = Math.sin(bird.flapTimer) * 6;
    ctx.fillStyle = '#ff9b9b';
    ctx.beginPath(); ctx.ellipse(-bird.w/2 + 3, flap, 6, 10, Math.PI/3, 0, Math.PI*2); ctx.fill();
    ctx.restore();
  }

  // Draw particles
  function drawParticles(now){
    const keep = [];
    particles.forEach(p => {
      const age = now - p.born;
      const t = age / p.life;
      if(t >= 1) return;
      p.x += p.vx; p.y += p.vy + t*0.4;
      ctx.globalAlpha = 1 - t;
      ctx.fillStyle = p.color;
      ctx.beginPath(); ctx.ellipse(p.x, p.y, p.r*(1-t), p.r*(1-t), 0, 0, Math.PI*2); ctx.fill();
      ctx.globalAlpha = 1;
      keep.push(p);
    });
    particles = keep;
  }

  // Update physics & game logic
  function update(now){
    if(!playing) return;

    // spawn pipes occasionally
    if(frame % Math.round(spawnRate) === 0) spawnPipe();

    // update pipes
    pipes.forEach(p => {
      p.x -= speed;
      // score passing detection
      if(!p.passed && p.x + p.w < bird.x - 2){
        p.passed = true;
        score += 1;
        scoreEl.textContent = score;
        playBeep(880, 'sine', 0.04, 0.06);
        // difficulty curve
        if(score % 5 === 0){
          speed += 0.14;
          spawnRate = Math.max(86, spawnRate - 4);
          baseGap = Math.max(92, baseGap - 3);
        }
      }
    });
    // remove off-screen
    pipes = pipes.filter(p => p.x + p.w > -60);

    // update coins
    coins.forEach(c => {
      c.x -= speed;
      if(!c.collected){
        const dx = c.x - bird.x, dy = c.y - bird.y;
        if(Math.hypot(dx, dy) < c.r + bird.w/3){
          c.collected = true;
          score += 2;
          scoreEl.textContent = score;
          playMultiChord([1200,1500], 'square', 0.08, 0.06);
          // coin particles
          for(let i=0;i<10;i++) spawnParticle(c.x, c.y, '#ffd54a', 520);
        }
      }
    });
    coins = coins.filter(c => c.x > -40 && !c.collected);

    // update powerups
    powerups.forEach(pu => {
      pu.x -= speed;
      if(!pu.taken && Math.hypot(pu.x - bird.x, pu.y - bird.y) < pu.r + bird.w/3){
        pu.taken = true;
        // spawn particles and give temporary multiplier (double points for 8 sec)
        for(let i=0;i<18;i++) spawnParticle(pu.x, pu.y, '#ff6b6b', 700);
        playMultiChord([900,1200,1600], 'sawtooth', 0.14, 0.06);
        // implement simple score boost: immediate +5 and speed tweak
        score += 5; scoreEl.textContent = score;
        speed *= 0.92;
        setTimeout(()=> { speed /= 0.92; }, 8000);
      }
    });
    powerups = powerups.filter(pu => pu.x > -40 && !pu.taken);

    // bird physics
    bird.dy += gravity;
    bird.dy = clamp(bird.dy, -12, 14);
    bird.y += bird.dy;
    bird.rot = clamp(bird.dy * 0.045, -0.9, 1.2);
    bird.flapTimer += 0.18;

    // collisions with pipes
    for(const p of pipes){
      const bx1 = bird.x - bird.w/2, bx2 = bird.x + bird.w/2;
      const by1 = bird.y - bird.h/2, by2 = bird.y + bird.h/2;
      const px1 = p.x, px2 = p.x + p.w;
      if(bx2 > px1 && bx1 < px2 && by1 < p.top){
        hit(); return;
      }
      if(bx2 > px1 && bx1 < px2 && by2 > H - p.bottom - 40){
        hit(); return;
      }
    }
    // ground or ceiling
    if(bird.y + bird.h/2 > H - 40 || bird.y - bird.h/2 < 0){
      hit(); return;
    }

    frame++;
  }

  // handle hit / game over
  function hit(){
    if(gameOver) return;
    gameOver = true;
    playing = false;
    // big particle burst
    for(let i=0;i<30;i++) spawnParticle(bird.x + rand(-10,10), bird.y + rand(-10,10), '#ff6b6b', 900);
    playMultiChord([160,240,320], 'sawtooth', 0.28, 0.18);
    if(score > best){
      best = score;
      localStorage.setItem('flappyBest', best);
      bestEl.textContent = best;
    }
    // small delay then allow restart on click/space
    setTimeout(()=>{}, 60);
  }

  // Render loop
  let last = performance.now();
  function render(now){
    const dt = now - last;
    last = now;

    // clear
    ctx.clearRect(0,0,W,H);

    // background & scenery
    drawBackground();
    drawPipes();
    drawCoins();
    drawPowerups(now);
    drawGround();
    drawBird(now);
    drawParticles(now);

    // overlay screens
    if(!playing && !gameOver){
      // start screen overlay
      ctx.fillStyle = 'rgba(0,0,0,0.28)'; ctx.fillRect(0,0,W,H);
      ctx.fillStyle = '#fff'; ctx.textAlign = 'center';
      ctx.font = '18px sans-serif';
      ctx.fillText('Press SPACE or TAP to start', W/2, H/2 - 10);
      ctx.font = '13px sans-serif';
      ctx.fillText('Collect coins and mushrooms for bonuses!', W/2, H/2 + 14);
    }
    if(gameOver){
      ctx.fillStyle = 'rgba(0,0,0,0.45)'; ctx.fillRect(0,0,W,H);
      ctx.fillStyle = '#fff'; ctx.textAlign = 'center';
      ctx.font = '22px sans-serif'; ctx.fillText('Game Over', W/2, H/2 - 18);
      ctx.font = '14px sans-serif'; ctx.fillText(`Score: ${score}   Best: ${best}`, W/2, H/2 + 6);
      ctx.fillText('Click or press SPACE to try again', W/2, H/2 + 34);
    }

    // update logic while rendering
    update(now);

    requestAnimationFrame(render);
  }

  // Start the loop
  resetGame();
  requestAnimationFrame(render);

  // Controls
  function resumeAudio(){
    if(audioCtx && audioCtx.state === 'suspended') audioCtx.resume();
  }

  function flapAction(){
    if(gameOver){
      // restart
      resetGame();
      playing = true;
      return;
    }
    if(!playing){
      playing = true;
      // ensure immediate pipe spawn a little after start
      frame = 2;
    }
    bird.dy = jump;
    bird.flapTimer += 1.2;
    playBeep(920, 'triangle', 0.06, 0.08);
  }

  document.addEventListener('keydown', function(e){
    if(e.code === 'Space' || e.code === 'ArrowUp'){
      e.preventDefault();
      resumeAudio();
      flapAction();
    } else if(e.code === 'KeyM'){
      audioOn = !audioOn;
      soundBtn.textContent = audioOn ? 'Mute' : 'Unmute';
    }
  });

  canvas.addEventListener('click', function(e){
    resumeAudio();
    flapAction();
  });
  canvas.addEventListener('touchstart', function(e){
    e.preventDefault();
    resumeAudio();
    flapAction();
  }, { passive:false });

  // toggle sound button
  soundBtn.addEventListener('click', function(){
    audioOn = !audioOn;
    soundBtn.textContent = audioOn ? 'Mute' : 'Unmute';
  });

  // expose small helper to stop the game if modal closes (optional)
  // if your modal has a close button that sets modal.style.display = 'none' you can also call:
  // resetGame(); to reset everything when modal closes
}


(function () {
  const canvas = document.getElementById('gold-particles');
  const ctx = canvas.getContext('2d');

  function resize() {
    const dpr = window.devicePixelRatio || 1;
    canvas.width = window.innerWidth * dpr;
    canvas.height = window.innerHeight * dpr;
    ctx.setTransform(dpr, 0, 0, dpr, 0, 0);
  }
  window.addEventListener('resize', resize);
  resize();

  const GOLD = ['#D4AF37', '#C49A2C', '#FFD36E'];
  function rand(min, max) { return Math.random() * (max - min) + min; }

  class Particle {
    constructor() { this.reset(true); }
    reset(initial = false) {
      this.x = rand(0, window.innerWidth);
      this.y = initial ? rand(0, window.innerHeight) : window.innerHeight + 10;
      this.size = rand(1.5, 4.5);
      this.speedY = rand(0.2, 0.6);
      this.hSpeed = rand(-0.2, 0.2);
      this.opacity = rand(0.4, 0.9);
      this.color = GOLD[Math.floor(rand(0, GOLD.length))];
      this.glow = this.size * 4;
    }
    update() {
      this.y -= this.speedY * 2;
      this.x += this.hSpeed;
      if (this.y < -10) this.reset();
    }
    draw() {
      ctx.save();
      ctx.globalAlpha = this.opacity;
      ctx.shadowBlur = this.glow;
      ctx.shadowColor = this.color;
      ctx.fillStyle = this.color;
      ctx.beginPath();
      ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
      ctx.fill();
      ctx.restore();
    }
  }

  let particles = [];
  function createParticles() {
    const count = Math.round((window.innerWidth * window.innerHeight) / 35000);
    particles = Array.from({ length: count }, () => new Particle());
  }
  createParticles();

  function animate() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    particles.forEach(p => { p.update(); p.draw(); });
    requestAnimationFrame(animate);
  }
  animate();
})();

</script>


</body>
</html>
