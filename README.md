# my.halo.ventures.index.html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Halo Ventures — Built for Those Who Are Built for More</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{--black:#000;--white:#FFF;--orange:#E14C11;--grey:#8A8A8A;--line:#E6E6E6;--line-dark:#1E1E1E;}
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{font-family:'Inter',sans-serif;background:var(--white);color:var(--black);-webkit-font-smoothing:antialiased;}
  ::selection{background:var(--orange);color:var(--white);}
  .mono{font-family:'IBM Plex Mono',monospace;}
  .serif-i{font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;}
  .wrap{max-width:1120px;margin:0 auto;padding:0 32px;}
  .kicker{font-family:'IBM Plex Mono',monospace;font-size:12px;letter-spacing:.14em;text-transform:uppercase;display:flex;align-items:center;gap:12px;}
  .kicker .dot{width:8px;height:8px;border-radius:50%;background:var(--orange);flex:none;}
  .dark .kicker{color:#B8B8B8;}
  .light .kicker{color:#5A5A5A;}
  section{padding:110px 0;}
  .dark{background:var(--black);color:var(--white);}
  .light{background:var(--white);color:var(--black);}
  h1,h2{font-weight:600;letter-spacing:-.02em;}
  h1{font-size:clamp(46px,7vw,92px);line-height:1.02;}
  h2{font-size:clamp(32px,4.4vw,56px);line-height:1.08;}
  h1 .serif-i,h2 .serif-i{color:var(--orange);letter-spacing:0;}
  .sub{font-size:18px;line-height:1.6;max-width:600px;}
  .dark .sub{color:#C9C9C9;}
  .light .sub{color:#4A4A4A;}
  nav{position:fixed;top:0;left:0;right:0;z-index:50;background:rgba(0,0,0,.85);backdrop-filter:blur(10px);border-bottom:1px solid var(--line-dark);}
  .nav-in{max-width:1120px;margin:0 auto;padding:18px 32px;display:flex;justify-content:space-between;align-items:center;}
  .brand{font-family:'IBM Plex Mono',monospace;font-size:12px;letter-spacing:.18em;color:var(--white);}
  .brand span{color:var(--orange);}
  .nav-links{display:flex;gap:28px;}
  .nav-links a{font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.12em;color:#A0A0A0;text-decoration:none;text-transform:uppercase;transition:color .2s;}
  .nav-links a:hover,.nav-links a:focus-visible{color:var(--white);}
  a:focus-visible{outline:2px solid var(--orange);outline-offset:3px;}
  @media(max-width:720px){.nav-links{display:none;}}

  .hero{min-height:100vh;display:flex;flex-direction:column;justify-content:center;padding:160px 0 60px;position:relative;background-image:radial-gradient(circle,#141414 1px,transparent 1px);background-size:26px 26px;}
  .hero .kicker{justify-content:center;margin-bottom:44px;}
  .hero-inner{text-align:center;max-width:980px;margin:0 auto;}
  .hero h1{margin-bottom:30px;}
  .hero-rule{width:140px;height:3px;background:var(--orange);border:1px solid var(--white);margin:0 auto 26px;}
  .hero-statement{font-family:'Instrument Serif',serif;font-style:italic;font-size:clamp(16px,2vw,21px);font-weight:400;color:#8E9196;margin-bottom:20px;white-space:nowrap;}
  @media(max-width:560px){.hero-statement{white-space:normal;}}
  .hero .sub{margin:0 auto;}
  .hero-foot{margin-top:auto;padding-top:70px;text-align:center;font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.24em;color:#6A6A6A;text-transform:uppercase;}

  .btn{display:inline-block;font-family:'IBM Plex Mono',monospace;font-size:13px;letter-spacing:.12em;text-transform:uppercase;text-decoration:none;padding:16px 36px;border:1px solid #4A4A4A;border-radius:999px;color:var(--white);transition:all .25s;}
  .btn:hover,.btn:focus-visible{border-color:var(--orange);color:var(--orange);}
  .btn.solid{background:var(--orange);border-color:var(--orange);color:var(--white);}
  .btn.solid:hover{background:#C43F0B;color:var(--white);}
  .choice{display:flex;gap:18px;justify-content:center;flex-wrap:wrap;}
  .btn.ghost{background:var(--white);border-color:var(--white);color:var(--black);}
  .btn.ghost:hover{background:#E9E9E9;border-color:#E9E9E9;color:var(--black);}

  .stat-grid{display:grid;grid-template-columns:1fr 1fr;gap:24px;margin-top:64px;}
  @media(max-width:820px){.stat-grid{grid-template-columns:1fr;}}
  .stat-card{border:1px solid var(--line);padding:40px 36px;background:#FDFDFD;}
  .stat-num{font-family:'Instrument Serif',serif;font-size:clamp(56px,7vw,92px);line-height:1;}
  .stat-num em{font-style:italic;color:var(--orange);}
  .stat-label{margin-top:14px;font-size:15px;line-height:1.55;color:#4A4A4A;max-width:340px;}
  .black-box{background:var(--black);color:var(--white);border-radius:22px;padding:44px 42px;font-size:19px;line-height:1.6;grid-row:span 2;display:flex;flex-direction:column;justify-content:center;gap:20px;}
  .black-box strong{color:var(--white);font-weight:600;}

  .cards3{display:grid;grid-template-columns:repeat(3,1fr);gap:22px;margin-top:64px;}
  @media(max-width:860px){.cards3{grid-template-columns:1fr;}}
  .d-card{background:#0C0C0C;border:1px solid var(--line-dark);border-radius:18px;padding:38px 32px;}
  .d-card .mono-h{font-family:'IBM Plex Mono',monospace;font-size:15px;letter-spacing:.04em;margin-bottom:14px;display:block;}
  .d-card .num{color:var(--orange);margin-right:10px;}
  .d-card p{font-size:15px;line-height:1.62;color:#B8B8B8;}
  .rhetorical{margin-top:90px;text-align:center;font-family:'Instrument Serif',serif;font-style:italic;font-size:clamp(22px,3vw,34px);line-height:1.4;color:var(--white);}
  .rhetorical .q{color:var(--orange);}

  /* values */
  .bushido{text-align:center;font-family:'Instrument Serif',serif;font-style:italic;font-size:clamp(24px,3.4vw,40px);line-height:1.35;max-width:860px;margin:0 auto;color:var(--black);}
  .bushido-attr{text-align:center;margin-top:18px;font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.2em;color:#9A9A9A;text-transform:uppercase;}
  .values{display:grid;grid-template-columns:repeat(3,1fr);gap:2px;background:var(--line);border:1px solid var(--line);margin-top:80px;}
  @media(max-width:860px){.values{grid-template-columns:1fr;}}
  .value{background:var(--white);padding:44px 36px 30px;display:flex;flex-direction:column;}
  .value-foot{margin-top:auto;padding-top:22px;font-family:'IBM Plex Mono',monospace;font-size:10px;letter-spacing:.12em;text-transform:uppercase;color:#8E9196;border-top:1px solid var(--line);}
  .value-foot::before{content:"// ";color:var(--orange);}
  .value ul{margin-bottom:26px;}
  .value h3{font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;font-size:30px;color:var(--orange);margin-bottom:22px;}
  .value ul{list-style:none;}
  .value li{font-size:14.5px;line-height:1.55;color:#333;padding:11px 0;border-top:1px solid var(--line);}
  .value li:first-child{border-top:none;padding-top:0;}
  .value li b{color:var(--black);}

  /* transform */
  .transform{text-align:center;}
  .transform h2{margin:26px 0 70px;}
  .split{display:grid;grid-template-columns:1fr auto 1fr;gap:40px;align-items:center;max-width:960px;margin:0 auto;}
  @media(max-width:760px){.split{grid-template-columns:1fr;gap:26px;}}
  .split .side{font-size:clamp(19px,2.4vw,26px);font-weight:500;line-height:1.4;color:var(--white);}
  .split .side em{font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;color:var(--orange);}
  .split .divid{font-family:'IBM Plex Mono',monospace;color:var(--orange);font-size:22px;}
  .split .l{text-align:right;} .split .r{text-align:left;}
  @media(max-width:760px){.split .l,.split .r{text-align:center;}}

  .profiles{display:grid;grid-template-columns:repeat(2,1fr);gap:2px;background:var(--line);border:1px solid var(--line);margin-top:64px;}
  @media(max-width:760px){.profiles{grid-template-columns:1fr;}}
  .profile{background:var(--white);padding:36px 34px;}
  .profile h3{font-size:17px;font-weight:600;margin-bottom:10px;}
  .profile h3 .tick{color:var(--orange);margin-right:8px;}
  .profile p{font-size:14.5px;line-height:1.6;color:#555;}
  .arch-label{margin-top:56px;font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.18em;color:var(--orange);text-transform:uppercase;}
  .profiles{margin-top:22px !important;}
  .nonneg{margin-top:40px;border-left:3px solid var(--orange);padding:6px 0 6px 24px;font-size:16px;line-height:1.65;color:#333;max-width:720px;}

  /* playbook */
  .pb-lead{max-width:720px;margin:26px 0 0;}
  .ratio-block{margin-top:56px;text-align:center;}
  .ratio-num{font-family:'Instrument Serif',serif;font-size:clamp(70px,10vw,130px);line-height:1;color:var(--white);}
  .ratio-num span{color:var(--orange);}
  .ratio-cap{margin-top:16px;font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.14em;color:var(--orange);text-transform:uppercase;}
  .ninety{margin-top:70px;background:#0C0C0C;border:1px solid var(--line-dark);border-radius:22px;padding:52px 48px;display:grid;grid-template-columns:auto 1fr;gap:48px;align-items:center;}
  @media(max-width:820px){.ninety{grid-template-columns:1fr;gap:24px;padding:40px 32px;}}
  .ninety .big{font-family:'Instrument Serif',serif;font-size:clamp(80px,10vw,140px);line-height:1;color:var(--white);}
  .ninety .big em{font-style:italic;color:var(--orange);}
  .ninety p{font-size:16.5px;line-height:1.65;color:#C9C9C9;}
  .ninety p b{color:var(--white);}

  .offer-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:24px;margin-top:64px;}
  @media(max-width:820px){.offer-grid{grid-template-columns:1fr;}}
  .offer{border:1px solid var(--line);padding:40px 36px;position:relative;}
  .offer .o-num{font-family:'Instrument Serif',serif;font-style:italic;font-size:30px;color:var(--orange);position:absolute;top:30px;right:34px;}
  .offer h3{font-size:19px;font-weight:600;margin-bottom:12px;max-width:80%;}
  .offer p{font-size:15px;line-height:1.62;color:#4A4A4A;}

  table.income{width:100%;border-collapse:collapse;margin-top:70px;}
  table.income caption{text-align:left;font-family:'IBM Plex Mono',monospace;font-size:12px;letter-spacing:.14em;text-transform:uppercase;color:#5A5A5A;padding-bottom:18px;}
  table.income th,table.income td{padding:22px 8px;border-bottom:1px solid var(--line);text-align:left;}
  table.income th{font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.12em;text-transform:uppercase;color:#8A8A8A;font-weight:500;border-bottom:1px solid var(--black);}
  table.income td.y{font-family:'Instrument Serif',serif;font-size:26px;}
  table.income td.amt{font-size:20px;font-weight:600;}
  table.income td.amt em{font-style:normal;color:var(--orange);}
  table.income td.note{font-size:14px;color:#666;line-height:1.5;}
  .equity{margin-top:46px;font-size:clamp(19px,2.4vw,24px);font-weight:500;letter-spacing:-.01em;}
  .equity em{font-family:'Instrument Serif',serif;font-style:italic;font-weight:400;color:var(--orange);}
  .fineprint{margin-top:20px;font-size:12px;color:#9A9A9A;line-height:1.6;max-width:760px;}

  .not-list{margin-top:60px;display:grid;gap:2px;}
  .not-item{background:#0C0C0C;border-left:3px solid var(--orange);padding:26px 30px;font-size:17px;line-height:1.6;color:#D8D8D8;}
  .not-item strong{color:var(--white);}
  .culture-quote{margin-top:72px;text-align:center;font-family:'Instrument Serif',serif;font-style:italic;font-size:clamp(24px,3.4vw,38px);line-height:1.35;max-width:820px;margin-left:auto;margin-right:auto;color:var(--white);}
  .culture-attr{text-align:center;margin-top:20px;font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.18em;color:#7A7A7A;text-transform:uppercase;}

  .builder{display:grid;grid-template-columns:1.1fr .9fr;gap:70px;align-items:center;margin-top:60px;}
  @media(max-width:860px){.builder{grid-template-columns:1fr;}}
  .pullquote{font-family:'Instrument Serif',serif;font-style:italic;font-size:clamp(24px,3vw,34px);line-height:1.4;border-left:3px solid var(--orange);padding-left:28px;color:#1A1A1A;}
  .bio p{font-size:15.5px;line-height:1.7;color:#3A3A3A;margin-bottom:16px;}
  .bio .name{font-weight:600;font-size:17px;margin-top:6px;}
  .bio .role{font-family:'IBM Plex Mono',monospace;font-size:11px;letter-spacing:.14em;text-transform:uppercase;color:#8A8A8A;margin-top:4px;}

  .final{text-align:center;padding:150px 0;}
  .final h2{max-width:860px;margin:0 auto 26px;}
  .final .sub{margin:0 auto 52px;}
  footer{background:var(--black);border-top:1px solid var(--line-dark);padding:44px 0;}
  .foot-in{max-width:1120px;margin:0 auto;padding:0 32px;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:18px;}
  .foot-in .brand{font-size:11px;}
  .foot-note{font-family:'IBM Plex Mono',monospace;font-size:10px;letter-spacing:.1em;color:#5A5A5A;}
  @media(prefers-reduced-motion:no-preference){
    .reveal{opacity:0;transform:translateY(18px);transition:opacity .7s ease,transform .7s ease;}
    .reveal.in{opacity:1;transform:none;}
  }
</style>
</head>
<body>

<nav>
  <div class="nav-in">
    <div class="brand">HALO <span>//</span> VENTURES</div>
    <div class="nav-links">
      <a href="#window">The Window</a>
      <a href="#values">Values</a>
      <a href="#playbook">The Playbook</a>
      <a href="#standard">The Standard</a>
    </div>
  </div>
</nav>

<!-- HERO -->
<section class="dark hero">
  <div class="wrap hero-inner">
    <div class="kicker"><span class="dot"></span>01 &nbsp;·&nbsp; THE QUESTION</div>
    <h1 class="reveal">What if there was no <span class="serif-i">ceiling?</span></h1>
    <div class="hero-rule reveal"></div>
    <p class="hero-statement reveal">Built for those&#8230; that are built for more.</p>
    <p class="sub reveal">Helping high-achievers in capped careers discover their potential.</p>
  </div>
  <div class="hero-foot">WHERE PURPOSE MEETS POTENTIAL</div>
</section>

<!-- THE WINDOW -->
<section class="light" id="window">
  <div class="wrap">
    <div class="kicker"><span class="dot"></span>02 &nbsp;·&nbsp; THE WINDOW</div>
    <h2 style="margin-top:28px;" class="reveal">The greatest demand.<br>The shortest <span class="serif-i">supply.</span></h2>
    <div class="stat-grid">
      <div class="stat-card reveal">
        <div class="stat-num">$124<em>T</em></div>
        <div class="stat-label">In generational wealth changes hands by 2048 — roughly $17 billion moving every single day.</div>
      </div>
      <div class="black-box reveal">
        <p><strong>Demand is climbing while supply falls.</strong></p>
        <p>Nearly half of all advisors retire in the next decade. Families need integrated planning more than ever — and there are fewer people to deliver it.</p>
        <p>For builders with proven track records, this is the widest opening the industry has offered in 30 years.</p>
      </div>
      <div class="stat-card reveal">
        <div class="stat-num">100<em>K</em></div>
        <div class="stat-label">Projected advisor shortage by 2034, with 40% of today's advisors retiring out of the business.</div>
      </div>
      <div class="stat-card reveal" style="grid-column:1;">
        <div class="stat-num">$240<em>T</em></div>
        <div class="stat-label">The national retirement gap — while the average personal savings rate sits frozen near 4%.</div>
      </div>
      <div class="stat-card reveal">
        <div class="stat-num">70<em>%</em></div>
        <div class="stat-label">Of generational wealth is lost by the second generation without real planning. 90% by the third.</div>
      </div>
    </div>
  </div>
</section>

<!-- THE CEILING -->
<section class="dark" id="ceiling">
  <div class="wrap">
    <div class="kicker"><span class="dot"></span>03 &nbsp;·&nbsp; THE CEILING</div>
    <h2 style="margin-top:28px;max-width:820px;" class="reveal">High performers don't stop performing.<br>The structure stops <span class="serif-i">paying.</span></h2>
    <div class="cards3">
      <div class="d-card reveal">
        <span class="mono-h"><span class="num">1.</span>The Earnings Ceiling</span>
        <p>Pay is capped by a salary band or a comp committee. The top is visible from the seat — and getting better at the job doesn't move it.</p>
      </div>
      <div class="d-card reveal">
        <span class="mono-h"><span class="num">2.</span>The Autonomy Ceiling</span>
        <p>Growth requires permission. Someone else sets the territory, the calendar, and the strategy — executing a vision they didn't write.</p>
      </div>
      <div class="d-card reveal">
        <span class="mono-h"><span class="num">3.</span>The Meaning Ceiling</span>
        <p>The work stops passing the pillow test. At the end of the day, there's no family whose life is better because of what got done.</p>
      </div>
    </div>
    <p class="rhetorical reveal">What would happen to your company<br>if you didn't show up to work <span class="q">tomorrow?</span></p>
  </div>
</section>

<!-- VALUES -->
<section class="light" id="values">
  <div class="wrap">
    <div class="kicker" style="justify-content:center;"><span class="dot"></span>04 &nbsp;·&nbsp; THE VALUES</div>
    <div style="margin-top:56px;">
      <p class="bushido reveal">"A culture is not a set of beliefs.<br>It's a set of actions."</p>
      <p class="bushido-attr">~ BUSHIDO</p>
    </div>
    <div class="values">
      <div class="value reveal">
        <h3>Integrity</h3>
        <ul>
          <li>We do what's right over what's fast, fun, or easy.</li>
          <li>We choose courage over comfort.</li>
          <li>We practice our values, not just preach them.</li>
        </ul>
        <p class="value-foot">Hard conversations are a professional responsibility.</p>
      </div>
      <div class="value reveal">
        <h3>Growth</h3>
        <ul>
          <li>We embrace adversity with optimism &amp; ownership.</li>
          <li>We focus on what's controllable and get better every day.</li>
          <li>We believe in potential &amp; deliver results.</li>
        </ul>
        <p class="value-foot">One day. One brick. One percent better.</p>
      </div>
      <div class="value reveal">
        <h3>Community</h3>
        <ul>
          <li>We build for the long-term.</li>
          <li>We are one team.</li>
          <li>We win big, and celebrate bigger.</li>
        </ul>
        <p class="value-foot">For generations to come.</p>
      </div>
    </div>
  </div>
</section>

<!-- TRANSFORMING -->
<section class="dark transform">
  <div class="wrap">
    <div class="kicker" style="justify-content:center;"><span class="dot"></span>05 &nbsp;·&nbsp; THE MISSION</div>
    <h2 class="reveal">Transforming finance <span class="serif-i">forever.</span></h2>
    <div class="split reveal">
      <div class="side l">We partner with <em>generational talent</em></div>
      <div class="divid">//</div>
      <div class="side r">to deliver <em>multi-generational results.</em></div>
    </div>
  </div>
</section>

<!-- WHO WE RECRUIT -->
<section class="light" id="who">
  <div class="wrap">
    <div class="kicker"><span class="dot"></span>06 &nbsp;·&nbsp; FOUNDER PROFILES</div>
    <h2 style="margin-top:28px;" class="reveal">Who we <span class="serif-i">partner with.</span></h2>
    <p class="sub" style="margin-top:26px;">We coach high-achievers who want to build a business. 94% of our top-performing advisors transitioned from other industries. This is not a job — or a way out of a bad career. It is about taking full ownership and building something real.</p>
    <p class="arch-label reveal">// FOUNDER ARCHETYPES</p>
    <div class="profiles">
      <div class="profile reveal">
        <h3><span class="tick">//</span>Women Leaders</h3>
        <p>High-performing women from corporate, sales, or professional services backgrounds. Female-led practices report higher client retention and longer advisor tenure. Women are projected to control $34 trillion in wealth by 2030, and families increasingly seek advisors who understand their unique dynamics, values, and life transitions.</p>
      </div>
      <div class="profile reveal">
        <h3><span class="tick">//</span>Military Veterans &amp; Leaders</h3>
        <p>Those who have thrived in high-stakes environments requiring discipline, systems thinking, mission execution, and leadership under uncertainty. Financial advisory runs on a daily operating system: consistent prospecting, client service rituals, and long-cycle relationship management. Veterans bring the operating cadence and resilience this business demands.</p>
      </div>
      <div class="profile reveal">
        <h3><span class="tick">//</span>"President's Club" Parents &amp; Revenue Drivers</h3>
        <p>Elite performers from relationship-driven industries — medical devices, technology, healthcare, biotechnology, and enterprise sales. Established pipeline discipline, consultative selling, and closing complex deals in competitive arenas.</p>
      </div>
      <div class="profile reveal">
        <h3><span class="tick">//</span>Mission-Driven Parents &amp; High-Achieving Professionals</h3>
        <p>Leaders in education, talent development, operations, recruiting, management, or athletics who have hit the corporate ceiling where higher compensation demands more time away from family. Execution of the business model offers full calendar ownership, uncapped income potential, and the ability to build an asset that serves clients while creating lasting family and community value.</p>
      </div>
    </div>
    <div class="nonneg reveal">
      <strong>Non-negotiable:</strong> a proven ability to build relationships, a logic-driven mind, long-term thinking, and evidence of having built something before. We invest for decades in the people we recruit — so we select slowly and on purpose.
    </div>
  </div>
</section>

<!-- THE PLAYBOOK -->
<section class="dark" id="playbook">
  <div class="wrap">
    <div class="kicker"><span class="dot"></span>07 &nbsp;·&nbsp; THE PLAYBOOK</div>
    <h2 style="margin-top:28px;" class="reveal">Proven <span class="serif-i">playbook.</span></h2>
    <p class="sub pb-lead reveal">Hope is not a plan. We run the One Card System — a training and development playbook designed specifically for career changers, converting proven skill from one industry into a practice that serves families for generations.</p>
    <div class="ratio-block reveal">
      <div class="ratio-num">10<span>:</span>3<span>:</span>1</div>
      <div class="ratio-cap">10 QUALIFIED SUSPECTS &nbsp;//&nbsp; 3 FACTFINDERS &nbsp;//&nbsp; 1 NEW CLIENT &nbsp;—&nbsp; TRUE PREDICTABILITY</div>
    </div>
    <div class="ninety reveal">
      <div class="big">90<em>.</em></div>
      <p><b>The first 90 days decide the trajectory.</b> Habits, skills, results — in that order. The expectation is simple: run the playbook to a tee. It takes 90 days to build a pipeline, and the reps invested early compound for an entire career.</p>
    </div>
    <div class="cards3">
      <div class="d-card reveal">
        <span class="mono-h"><span class="num">→</span>The 99 Club</span>
        <p>Front-loaded mastery: 33 client meetings a month in the first quarter — 30% more learning reps than the industry standard. More reps, faster pattern recognition, earlier wins.</p>
      </div>
      <div class="d-card reveal">
        <span class="mono-h"><span class="num">→</span>Never Work Alone</span>
        <p>Joint work with senior advisors on real cases from week one. Watch what right looks like, then run it — with a coach in the room until one isn't needed.</p>
      </div>
      <div class="d-card reveal">
        <span class="mono-h"><span class="num">→</span>Own the Outcome</span>
        <p>Clients stay an average of 42 years and buy roughly 20 times. The book compounds instead of churning — and becomes a seven-figure asset the advisor owns.</p>
      </div>
    </div>
  </div>
</section>

<!-- THE PARTNERSHIP -->
<section class="light" id="offer">
  <div class="wrap">
    <div class="kicker"><span class="dot"></span>08 &nbsp;·&nbsp; THE PARTNERSHIP</div>
    <h2 style="margin-top:28px;" class="reveal">In business for yourself.<br>Never by <span class="serif-i">yourself.</span></h2>
    <div class="offer-grid">
      <div class="offer reveal">
        <span class="o-num">i.</span>
        <h3>Institutional Strength</h3>
        <p>Build on a platform, not from scratch. Our partners plug directly into the financial strength, compliance infrastructure, technology, and development resources of one of the industry's most established institutions. The credibility is already built — the focus stays on clients.</p>
      </div>
      <div class="offer reveal">
        <span class="o-num">ii.</span>
        <h3>The Development System</h3>
        <p>Structured training built for career changers — wealth management taught from the ground up, layered onto the relationship skill a prior industry already proved.</p>
      </div>
      <div class="offer reveal">
        <span class="o-num">iii.</span>
        <h3>Uncapped Economics</h3>
        <p>We invest in the partners we develop. In addition to enhanced commissions, we add a monthly business stipend throughout your first year — plus 16 residual income streams, fully funded pensions, and a book of business that becomes a seven-figure asset you own.</p>
      </div>
      <div class="offer reveal">
        <span class="o-num">iv.</span>
        <h3>Founder Coaching</h3>
        <p>Direct feedback from operators who have built before. Positioning, acquisition systems, and metrics-driven reviews — thinking like a business owner, not a practitioner.</p>
      </div>
    </div>

    <table class="income reveal">
      <caption>// The Trajectory</caption>
      <tr><th>Stage</th><th>Income Range</th><th>What's Happening</th></tr>
      <tr>
        <td class="y">Year 1</td>
        <td class="amt">$85K – <em>$200K+</em></td>
        <td class="note">Foundation. Positioning defined, first clients acquired, pipeline built.</td>
      </tr>
      <tr>
        <td class="y">Year 3</td>
        <td class="amt">$274K – <em>$427K+</em></td>
        <td class="note">Scaling. Repeatable process proven, recurring revenue becomes meaningful.</td>
      </tr>
      <tr>
        <td class="y">Year 5</td>
        <td class="amt">$424K – <em>$750K+</em></td>
        <td class="note">Leverage. Team in place, income heavily recurring, practice value compounding.</td>
      </tr>
      <tr>
        <td class="y">Year 10</td>
        <td class="amt">$864K+ <em>avg</em></td>
        <td class="note">Ownership. Average income $864,000+ per year. Top quartile: $1,445,000+.</td>
      </tr>
    </table>
    <p class="equity reveal">Build real equity. Everything you build <em>compounds.</em></p>
    <p class="fineprint">Income figures reflect ranges achieved by advisors in this system and are not guarantees. Building a practice takes disciplined execution over years, not months.</p>
  </div>
</section>

<!-- THE STANDARD -->
<section class="dark" id="standard">
  <div class="wrap">
    <div class="kicker"><span class="dot"></span>09 &nbsp;·&nbsp; THE STANDARD</div>
    <h2 style="margin-top:28px;" class="reveal">Courage over <span class="serif-i">comfort.</span></h2>
    <div class="not-list">
      <div class="not-item reveal"><strong>We are not a 9-to-5.</strong> We are builders, founders, and mission-driven leaders solving multigenerational problems with the businesses we build. That does not happen overnight.</div>
      <div class="not-item reveal"><strong>We are not comfortable.</strong> High standards are the baseline. Feedback is direct. The bar rises with every client served and every person hired.</div>
      <div class="not-item reveal"><strong>We are not transactional.</strong> We select slowly, partner for the long term, and think in generations — decades, not quarters.</div>
      <div class="not-item reveal"><strong>We are not for everyone.</strong> This is mutual selection. We are for founders — and founders are not for everyone.</div>
    </div>
    <p class="culture-quote reveal">"Every time we win, we win as a team. Every time we lose, we lose as a team. We do not focus on individual credit."</p>
    <p class="culture-attr">— The Lake Oswego Standard</p>
  </div>
</section>

<!-- THE BUILDER -->
<section class="light" id="builder">
  <div class="wrap">
    <div class="kicker"><span class="dot"></span>10 &nbsp;·&nbsp; THE BUILDER</div>
    <div class="builder">
      <div class="bio reveal">
        <p>Chris Hedum is the Head of Growth at our Lake Oswego private client group, where he helps professionals from outside the financial services industry build advisory businesses.</p>
        <p>Before this, Chris spent nearly a decade in tech and venture capital. He worked with founders at early-stage startups, helping them go to market, grow revenue, and raise funding. He thrived in this high-pressure and competitive world, helping founders raise more than $140 million in his tenure.</p>
        <p>When his daughter was born, his priorities changed. The work he was doing stopped passing the "pillow test." And he didn't want to keep missing moments he'd never get back, doing work that no longer aligned with his values.</p>
        <p>Today, Chris is a father of two — and spends every day working with high-achieving professionals who have decided to bet on themselves. He applies the same principles he used with startup founders — clear positioning, focused strategy, and disciplined execution — to help advisors build businesses designed to serve clients for generations.</p>
        <p>Chris lives in Portland with his wife and two daughters. Outside of work, he enjoys spending time with his family and playing rugby.</p>
        <p class="name">Chris Hedum</p>
        <p class="role">Head of Growth · Lake Oswego</p>
      </div>
      <div class="pullquote reveal">"I didn't want to keep missing moments I'd never get back, doing work that I wasn't proud to be doing."</div>
    </div>
  </div>
</section>

<!-- FINAL -->
<section class="dark final">
  <div class="wrap">
    <div class="kicker" style="justify-content:center;"><span class="dot"></span>11 &nbsp;·&nbsp; THE FIRST BRICK</div>
    <h2 style="margin-top:28px;">The best talent doesn't want a job.<br>They want to <span class="serif-i">build.</span></h2>
    <p class="sub">Selection is mutual, deliberate, and slow on purpose. We invest for decades in the people we choose.</p>
    <div class="choice">
      <a href="#" class="btn ghost" onclick="return false;" title="Nothing changes here.">COMFORT</a>
      <a href="mailto:Christopher.hedum@nm.com" class="btn solid">COURAGE</a>
    </div>
  </div>
</section>

<footer>
  <div class="foot-in">
    <div class="brand">HALO <span>//</span> VENTURES</div>
    <div class="foot-note">LAKE OSWEGO &nbsp;·&nbsp; WHERE PURPOSE MEETS POTENTIAL &nbsp;·&nbsp; © 2026</div>
  </div>
</footer>

<script>
  const io = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{ if(e.isIntersecting){ e.target.classList.add('in'); io.unobserve(e.target);} });
  },{threshold:0.12});
  document.querySelectorAll('.reveal').forEach(el=>io.observe(el));
</script>
</body>
</html>
