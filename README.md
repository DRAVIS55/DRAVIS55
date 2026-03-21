<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Samuel Kibunja Macharia — DRAVIS55</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700;800&family=DM+Mono:wght@300;400;500&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet"/>
<style>
:root {
  --bg: #09090b;
  --bg2: #111114;
  --bg3: #18181c;
  --bg4: #212127;
  --border: rgba(255,255,255,0.07);
  --border2: rgba(255,255,255,0.12);
  --text: #f4f4f5;
  --muted: #a1a1aa;
  --hint: #52525b;
  --accent: #38bdf8;
  --accent2: #818cf8;
  --green: #34d399;
  --amber: #fbbf24;
  --coral: #f87171;
  --ff-display: 'Syne', sans-serif;
  --ff-body: 'DM Sans', sans-serif;
  --ff-mono: 'DM Mono', monospace;
}
*{box-sizing:border-box;margin:0;padding:0}
body{background:var(--bg);color:var(--text);font-family:var(--ff-body);font-size:14px;line-height:1.6;min-height:100vh}
a{color:var(--accent);text-decoration:none}
a:hover{text-decoration:underline}

/* ── HERO ── */
.hero{padding:72px 48px 56px;border-bottom:1px solid var(--border);position:relative;overflow:hidden}
.hero::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse 80% 60% at 50% -10%, rgba(56,189,248,0.08), transparent);pointer-events:none}
.hero-inner{max-width:900px;margin:0 auto}
.hero-tag{font-family:var(--ff-mono);font-size:11px;color:var(--accent);letter-spacing:.12em;text-transform:uppercase;margin-bottom:16px;opacity:.85}
.hero h1{font-family:var(--ff-display);font-size:clamp(36px,5vw,56px);font-weight:800;line-height:1.08;letter-spacing:-.02em;margin-bottom:8px}
.hero h1 span{color:var(--accent)}
.hero-sub{font-size:16px;color:var(--muted);margin-bottom:28px;max-width:560px;line-height:1.7}
.hero-links{display:flex;flex-wrap:wrap;gap:10px}
.pill{display:inline-flex;align-items:center;gap:6px;padding:6px 14px;border-radius:999px;border:1px solid var(--border2);font-size:12px;font-family:var(--ff-mono);color:var(--muted);background:var(--bg3);transition:all .18s;white-space:nowrap}
.pill:hover{border-color:var(--accent);color:var(--accent);text-decoration:none;background:rgba(56,189,248,.06)}
.pill svg{width:13px;height:13px;flex-shrink:0}

/* ── LAYOUT ── */
.page{max-width:900px;margin:0 auto;padding:0 48px 80px}
section{padding:56px 0 0}
.section-label{font-family:var(--ff-mono);font-size:10px;letter-spacing:.15em;text-transform:uppercase;color:var(--hint);margin-bottom:28px;display:flex;align-items:center;gap:10px}
.section-label::after{content:'';flex:1;height:1px;background:var(--border)}
h2{font-family:var(--ff-display);font-size:22px;font-weight:700;margin-bottom:20px;letter-spacing:-.01em}

/* ── ABOUT ── */
.about-para{font-size:15px;color:var(--muted);line-height:1.85;max-width:720px;margin-bottom:20px}
.about-para strong{color:var(--text);font-weight:500}
.chips{display:flex;flex-wrap:wrap;gap:8px;margin-top:4px}
.chip{padding:4px 12px;border-radius:6px;font-size:11px;font-family:var(--ff-mono);border:1px solid var(--border2);color:var(--muted);background:var(--bg3)}

/* ── EXPERIENCE ── */
.exp-list{position:relative;padding-left:28px}
.exp-line{position:absolute;left:7px;top:8px;bottom:8px;width:2px;background:linear-gradient(to bottom,var(--accent),var(--accent2),transparent);border-radius:2px;opacity:.35}
.exp-item{position:relative;margin-bottom:0}
.exp-item + .exp-item{margin-top:36px}
.exp-dot{position:absolute;left:-24px;top:6px;width:14px;height:14px;border-radius:50%;border:2px solid var(--accent);background:var(--bg);display:flex;align-items:center;justify-content:center;flex-shrink:0}
.exp-dot-inner{width:5px;height:5px;border-radius:50%;background:var(--accent)}
.exp-dot.muted{border-color:var(--hint)}
.exp-dot.muted .exp-dot-inner{background:var(--hint)}
.exp-card{background:var(--bg2);border:1px solid var(--border);border-radius:12px;padding:20px 22px;transition:border-color .2s}
.exp-card:hover{border-color:var(--border2)}
.exp-header{display:flex;align-items:flex-start;justify-content:space-between;gap:12px;flex-wrap:wrap;margin-bottom:6px}
.exp-title{font-family:var(--ff-display);font-size:15px;font-weight:700;color:var(--text);line-height:1.3}
.exp-org{color:var(--accent);font-size:13px;font-weight:500}
.exp-meta{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:10px}
.tag{padding:3px 9px;border-radius:5px;font-size:11px;font-family:var(--ff-mono);border:1px solid var(--border);color:var(--muted);background:var(--bg3);white-space:nowrap}
.tag.active{border-color:rgba(52,211,153,.3);color:var(--green);background:rgba(52,211,153,.06)}
.tag.ended{border-color:var(--border);color:var(--hint)}
.exp-body{font-size:13px;color:var(--muted);line-height:1.75}
.exp-body strong{color:var(--text);font-weight:500}
.stack-row{display:flex;flex-wrap:wrap;gap:6px;margin-top:12px}
.stag{padding:3px 9px;border-radius:5px;font-size:11px;font-family:var(--ff-mono);background:rgba(56,189,248,.07);border:1px solid rgba(56,189,248,.18);color:var(--accent)}

/* ── TIMELINE ── */
.tl-grid{display:grid;grid-template-columns:64px 1fr;gap:0}
.tl-year{font-family:var(--ff-mono);font-size:11px;color:var(--hint);padding-top:18px;text-align:right;padding-right:16px;line-height:1}
.tl-col{border-left:2px solid var(--border2);padding-left:20px;padding-bottom:0}
.tl-group{padding:12px 0}
.tl-group + .tl-group{border-top:1px solid var(--border)}
.tl-entry{display:flex;align-items:flex-start;gap:10px;padding:6px 0;position:relative}
.tl-entry::before{content:'';position:absolute;left:-27px;top:14px;width:8px;height:8px;border-radius:50%;border:2px solid var(--border2);background:var(--bg)}
.tl-entry.active::before{border-color:var(--accent);background:rgba(56,189,248,.2)}
.tl-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0;margin-top:5px}
.tl-info{flex:1}
.tl-role{font-size:13px;color:var(--text);font-weight:500}
.tl-place{font-size:12px;color:var(--muted);margin-top:1px}
.tl-badge{font-size:10px;font-family:var(--ff-mono);padding:2px 7px;border-radius:4px;background:rgba(52,211,153,.08);color:var(--green);border:1px solid rgba(52,211,153,.2);margin-left:auto;flex-shrink:0;align-self:flex-start;margin-top:3px}
.tl-badge.done{background:rgba(113,113,122,.08);color:var(--hint);border-color:var(--border)}

/* ── PROJECTS ── */
.proj-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.proj-card{background:var(--bg2);border:1px solid var(--border);border-radius:12px;padding:18px 18px 14px;display:flex;flex-direction:column;gap:10px;transition:border-color .2s,transform .2s}
.proj-card:hover{border-color:var(--border2);transform:translateY(-1px)}
.proj-top{display:flex;align-items:flex-start;justify-content:space-between;gap:8px}
.proj-name{font-family:var(--ff-display);font-size:14px;font-weight:700;color:var(--text);line-height:1.3}
.proj-name a{color:var(--text)}
.proj-name a:hover{color:var(--accent);text-decoration:none}
.proj-status{font-size:10px;font-family:var(--ff-mono);padding:2px 7px;border-radius:4px;flex-shrink:0;margin-top:2px}
.s-live{background:rgba(52,211,153,.08);color:var(--green);border:1px solid rgba(52,211,153,.2)}
.s-dev{background:rgba(251,191,36,.08);color:var(--amber);border:1px solid rgba(251,191,36,.2)}
.s-prod{background:rgba(129,140,248,.08);color:var(--accent2);border:1px solid rgba(129,140,248,.2)}
.proj-desc{font-size:12px;color:var(--muted);line-height:1.65;flex:1}
.proj-desc strong{color:var(--text);font-weight:500}
.proj-stack{display:flex;flex-wrap:wrap;gap:5px}
.pstag{font-size:10px;font-family:var(--ff-mono);padding:2px 7px;border-radius:4px;background:var(--bg3);border:1px solid var(--border);color:var(--hint)}
.cat-label{font-family:var(--ff-display);font-size:13px;font-weight:700;color:var(--muted);margin:28px 0 10px;display:flex;align-items:center;gap:8px}
.cat-label span{font-size:11px;font-weight:400;font-family:var(--ff-mono)}

/* ── TECH ── */
.tech-section{margin-bottom:28px}
.tech-section h4{font-family:var(--ff-mono);font-size:10px;letter-spacing:.12em;text-transform:uppercase;color:var(--hint);margin-bottom:12px;padding-bottom:6px;border-bottom:1px solid var(--border)}
.tech-grid{display:flex;flex-wrap:wrap;gap:8px}
.tech-chip{display:flex;align-items:center;gap:7px;padding:7px 12px;border-radius:8px;border:1px solid var(--border);background:var(--bg2);font-size:12px;font-family:var(--ff-mono);color:var(--muted);transition:all .18s}
.tech-chip:hover{border-color:var(--border2);color:var(--text)}
.tech-chip svg,.tech-chip img{width:15px;height:15px;flex-shrink:0;opacity:.75}

/* ── CERTS ── */
.cert-list{display:flex;flex-direction:column;gap:0}
.cert-item{display:grid;grid-template-columns:1fr auto;gap:16px;align-items:center;padding:14px 0;border-bottom:1px solid var(--border)}
.cert-item:first-child{border-top:1px solid var(--border)}
.cert-name{font-size:13px;color:var(--text);font-weight:500}
.cert-issuer{font-size:12px;color:var(--muted);margin-top:2px}
.cert-badge{font-size:10px;font-family:var(--ff-mono);padding:3px 9px;border-radius:5px;background:rgba(129,140,248,.08);color:var(--accent2);border:1px solid rgba(129,140,248,.18);white-space:nowrap}

/* ── FOOTER ── */
.footer{border-top:1px solid var(--border);padding:40px 48px;text-align:center}
.footer-inner{max-width:900px;margin:0 auto}
.footer-motto{font-family:var(--ff-display);font-size:20px;font-weight:700;margin-bottom:20px;letter-spacing:-.01em}
.footer-motto span{color:var(--accent)}
.footer-links{display:flex;justify-content:center;flex-wrap:wrap;gap:10px}

/* ── FADE IN ── */
@keyframes fadeUp{from{opacity:0;transform:translateY(14px)}to{opacity:1;transform:none}}
.hero-inner,.page section{animation:fadeUp .5s ease both}
.page section:nth-child(1){animation-delay:.05s}
.page section:nth-child(2){animation-delay:.1s}
.page section:nth-child(3){animation-delay:.15s}
.page section:nth-child(4){animation-delay:.2s}
.page section:nth-child(5){animation-delay:.25s}
.page section:nth-child(6){animation-delay:.3s}

@media(max-width:600px){
  .hero{padding:48px 20px 40px}
  .page{padding:0 20px 60px}
  .proj-grid{grid-template-columns:1fr}
}
</style>
</head>
<body>

<!-- ═══ HERO ═══ -->
<header class="hero">
  <div class="hero-inner">
    <p class="hero-tag">DRAVIS55 &nbsp;·&nbsp; Nairobi, Kenya &nbsp;·&nbsp; BSc CS @ Chuka University '27</p>
    <h1>Samuel<br><span>Kibunja</span> Macharia</h1>
    <p class="hero-sub">Co-Founder & CTO at DravTech IT Solutions. Building AI-driven systems, civic tech, and scalable platforms across Eastern Africa.</p>
    <div class="hero-links">
      <a class="pill" href="https://github.com/DRAVIS55" target="_blank">
        <svg fill="currentColor" viewBox="0 0 24 24"><path d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"/></svg>
        DRAVIS55
      </a>
      <a class="pill" href="https://www.linkedin.com/in/samuelkibunja/" target="_blank">
        <svg fill="currentColor" viewBox="0 0 24 24"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
        LinkedIn
      </a>
      <a class="pill" href="https://x.com/samuelkibu87288" target="_blank">
        <svg fill="currentColor" viewBox="0 0 24 24"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-4.714-6.231-5.401 6.231H2.744l7.73-8.835L1.254 2.25H8.08l4.253 5.622zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
        @samuelkibu87288
      </a>
      <a class="pill" href="mailto:samuelkibunja55@gmail.com">
        <svg fill="currentColor" viewBox="0 0 24 24"><path d="M1.5 8.67v8.58a3 3 0 003 3h15a3 3 0 003-3V8.67l-8.928 5.493a3 3 0 01-3.144 0L1.5 8.67z"/><path d="M22.5 6.908V6.75a3 3 0 00-3-3h-15a3 3 0 00-3 3v.158l9.714 5.978a1.5 1.5 0 001.572 0L22.5 6.908z"/></svg>
        samuelkibunja55@gmail.com
      </a>
      <a class="pill" href="https://wa.me/254758067458" target="_blank">
        <svg fill="currentColor" viewBox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
        +254 758 067 458
      </a>
    </div>
  </div>
</header>

<div class="page">

<!-- ═══ ABOUT ═══ -->
<section>
  <p class="section-label">About</p>
  <p class="about-para">
    I'm a Computer Science student at <strong>Chuka University</strong> (BSc, Class of 2027) and Co-Founder & CTO of <strong>DravTech IT Solutions</strong>. I build intelligent, scalable systems — from AI scheduling engines that eliminate university timetable conflicts, to multi-channel NGO platforms, civic news aggregators, and full-stack hotel management systems.
  </p>
  <p class="about-para">
    My work spans the full stack: <strong>Django, React, Node.js, FastAPI</strong> on the backend and frontend; <strong>PostgreSQL, MySQL, MongoDB</strong> for data; and AI/ML pipelines for scheduling, personalisation, and market prediction. I'm actively advancing in <strong>Cybersecurity, Blockchain/Web3</strong>, and <strong>Quantitative Finance</strong>.
  </p>
  <div class="chips">
    <span class="chip">Full-Stack Engineering</span>
    <span class="chip">AI/ML Systems</span>
    <span class="chip">Cybersecurity</span>
    <span class="chip">Blockchain &amp; Web3</span>
    <span class="chip">Quantitative Finance</span>
    <span class="chip">Civic Tech</span>
  </div>
</section>

<!-- ═══ EXPERIENCE ═══ -->
<section>
  <p class="section-label">Experience</p>

  <div class="exp-list">
    <div class="exp-line"></div>

    <!-- KEPSA -->
    <div class="exp-item">
      <div class="exp-dot"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">KFA Director &amp; Data Verifier</div>
            <div class="exp-org">Kenya Private Sector Alliance (KEPSA)</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag active">Sep 2024 – Present</span>
          <span class="tag">Contract</span>
          <span class="tag">Tharaka Nithi County · Remote</span>
        </div>
        <div class="exp-body">
          Leading field operations as <strong>KFA Director for Tharaka Nithi County</strong> within Kenya's premier business alliance. Validates and improves SME data accuracy supporting financial inclusion, credit scoring, and capital allocation models. Delivers structured field reports and stakeholder engagement across the county.
        </div>
      </div>
    </div>

    <!-- Skills Trainer -->
    <div class="exp-item">
      <div class="exp-dot muted"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">Software &amp; Digital Skills Trainer</div>
            <div class="exp-org">Digital Stationery &amp; Printers Cyber, Chuka</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag ended">Sep 2023 – Sep 2025</span>
          <span class="tag">Part-time</span>
          <span class="tag">Chuka · On-site</span>
        </div>
        <div class="exp-body">
          Delivered practical, hands-on digital and programming skills training across multiple technologies over two years. Bridged theoretical knowledge with real-world application, improving technical proficiency and employability for dozens of students.
        </div>
      </div>
    </div>

    <!-- Lowlands -->
    <div class="exp-item">
      <div class="exp-dot"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">Full-Stack Developer</div>
            <div class="exp-org">Lowlands Hotel &amp; Spa</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag active">2024 – Present</span>
          <span class="tag">Contract</span>
          <span class="tag">Tharaka Nithi · Remote</span>
        </div>
        <div class="exp-body">
          Rebuilt the hotel website from a static site to a modern full-stack platform. Delivered JWT-secured REST API with <strong>5-role RBAC</strong>, multi-role staff dashboard with analytics, online booking with real-time availability checking, contact CMS with reply-by-email, and Docker-ready production infrastructure.
        </div>
        <div class="stack-row">
          <span class="stag">React</span><span class="stag">Vite</span><span class="stag">Node.js</span><span class="stag">Express</span><span class="stag">MySQL</span><span class="stag">JWT</span><span class="stag">Docker</span>
        </div>
      </div>
    </div>

    <!-- TISC -->
    <div class="exp-item">
      <div class="exp-dot"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">System Developer</div>
            <div class="exp-org">TISC, Chuka University</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag active">Oct 2025 – Present</span>
          <span class="tag">Seasonal</span>
          <span class="tag">Remote</span>
        </div>
        <div class="exp-body">
          Built an AI scheduling system achieving <strong>0% timetable conflicts</strong>. Reduced scheduling time from 3–5 hours to <strong>&lt;10 seconds</strong> and API response from ~1000ms to <strong>5ms</strong> (200× improvement). Eliminated ~95% of manual scheduling workload university-wide.
        </div>
        <div class="stack-row">
          <span class="stag">Django</span><span class="stag">Python</span><span class="stag">AI/ML</span><span class="stag">Constraint Solving</span>
        </div>
      </div>
    </div>

    <!-- DravTech -->
    <div class="exp-item">
      <div class="exp-dot"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">Co-Founder &amp; CTO</div>
            <div class="exp-org">DravTech IT Solutions</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag active">Sep 2025 – Present</span>
          <span class="tag">Part-time</span>
          <span class="tag">Nairobi · Remote</span>
        </div>
        <div class="exp-body">
          Spearheading technology vision and product architecture for a growing tech startup. Delivered scalable platforms serving hundreds of active users with high reliability, driving innovation through AI-powered and real-time systems.
        </div>
      </div>
    </div>

    <!-- Grassroot -->
    <div class="exp-item">
      <div class="exp-dot"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">Webmaster</div>
            <div class="exp-org">Grassroot Development Organisation Kenya</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag active">Sep 2025 – Present</span>
          <span class="tag">Part-time</span>
          <span class="tag">Kenya · Remote</span>
        </div>
        <div class="exp-body">
          Led development of a scalable digital platform for grassroots NGO operations. Engineered multi-channel donation integrations: <strong>PayPal, M-Pesa, card payments, Sui Blockchain</strong>. Manages cloud infrastructure, security, and system availability.
        </div>
        <div class="stack-row">
          <span class="stag">Django</span><span class="stag">M-Pesa API</span><span class="stag">PayPal</span><span class="stag">Sui Blockchain</span>
        </div>
      </div>
    </div>

    <!-- LEZOL -->
    <div class="exp-item">
      <div class="exp-dot"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">Full-Stack Developer</div>
            <div class="exp-org">LEZOL Engineering</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag active">Jan 2026 – Present</span>
          <span class="tag">Contract</span>
          <span class="tag">Nairobi · Remote</span>
        </div>
        <div class="exp-body">
          Architecting a production-ready e-commerce platform to digitise end-to-end engineering business operations, built for real-world transaction volume and long-term growth.
        </div>
        <div class="stack-row">
          <span class="stag">Node.js</span><span class="stag">React</span><span class="stag">E-commerce</span>
        </div>
      </div>
    </div>

    <!-- Hope & Home -->
    <div class="exp-item">
      <div class="exp-dot"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">Full-Stack Developer</div>
            <div class="exp-org">Hope &amp; HomeKe</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag active">Jan 2026 – Present</span>
          <span class="tag">Contract</span>
          <span class="tag">Nairobi · Remote</span>
        </div>
        <div class="exp-body">
          Delivered a production-ready e-commerce platform for a growing interior décor brand, with interactive UI/UX enabling seamless product discovery and ordering.
        </div>
        <div class="stack-row">
          <span class="stag">Django</span><span class="stag">E-commerce</span><span class="stag">UI/UX</span>
        </div>
      </div>
    </div>

    <!-- Boyvate -->
    <div class="exp-item">
      <div class="exp-dot muted"><div class="exp-dot-inner"></div></div>
      <div class="exp-card">
        <div class="exp-header">
          <div>
            <div class="exp-title">Presiding Officer / Oversight Chair</div>
            <div class="exp-org">Boyvate NGO</div>
          </div>
        </div>
        <div class="exp-meta">
          <span class="tag ended">Feb 2026 – Mar 2026</span>
          <span class="tag">Apprenticeship</span>
        </div>
        <div class="exp-body">
          Strengthened governance and accountability through structured oversight and leadership. Promoted transparency and integrity in organisational decision-making frameworks.
        </div>
      </div>
    </div>

  </div>
</section>

<!-- ═══ TIMELINE ═══ -->
<section>
  <p class="section-label">Career Timeline</p>
  <div class="tl-grid">

    <div class="tl-year">2023</div>
    <div class="tl-col">
      <div class="tl-group">
        <div class="tl-entry">
          <div class="tl-info">
            <div class="tl-role">Skills Trainer · Digital Stationery &amp; Printers Cyber</div>
            <div class="tl-place">Chuka · On-site</div>
          </div>
          <span class="tl-badge done">Completed Sep 2025</span>
        </div>
      </div>
    </div>

    <div class="tl-year">2024</div>
    <div class="tl-col">
      <div class="tl-group">
        <div class="tl-entry active">
          <div class="tl-info">
            <div class="tl-role">KFA Director &amp; Data Verifier · KEPSA</div>
            <div class="tl-place">Tharaka Nithi County · Remote</div>
          </div>
          <span class="tl-badge">Ongoing</span>
        </div>
        <div class="tl-entry active">
          <div class="tl-info">
            <div class="tl-role">Full-Stack Developer · Lowlands Hotel &amp; Spa</div>
            <div class="tl-place">Tharaka Nithi · Remote</div>
          </div>
          <span class="tl-badge">Ongoing</span>
        </div>
      </div>
    </div>

    <div class="tl-year">2025</div>
    <div class="tl-col">
      <div class="tl-group">
        <div class="tl-entry active">
          <div class="tl-info">
            <div class="tl-role">System Developer · TISC, Chuka University</div>
            <div class="tl-place">Remote · Oct 2025</div>
          </div>
          <span class="tl-badge">Ongoing</span>
        </div>
        <div class="tl-entry active">
          <div class="tl-info">
            <div class="tl-role">Co-Founder &amp; CTO · DravTech IT Solutions</div>
            <div class="tl-place">Nairobi · Sep 2025</div>
          </div>
          <span class="tl-badge">Ongoing</span>
        </div>
        <div class="tl-entry active">
          <div class="tl-info">
            <div class="tl-role">Webmaster · Grassroot Development Organisation Kenya</div>
            <div class="tl-place">Kenya · Sep 2025</div>
          </div>
          <span class="tl-badge">Ongoing</span>
        </div>
      </div>
    </div>

    <div class="tl-year">2026</div>
    <div class="tl-col">
      <div class="tl-group">
        <div class="tl-entry active">
          <div class="tl-info">
            <div class="tl-role">Full-Stack Developer · LEZOL Engineering</div>
            <div class="tl-place">Nairobi · Jan 2026</div>
          </div>
          <span class="tl-badge">Ongoing</span>
        </div>
        <div class="tl-entry active">
          <div class="tl-info">
            <div class="tl-role">Full-Stack Developer · Hope &amp; HomeKe</div>
            <div class="tl-place">Nairobi · Jan 2026</div>
          </div>
          <span class="tl-badge">Ongoing</span>
        </div>
        <div class="tl-entry">
          <div class="tl-info">
            <div class="tl-role">Presiding Officer · Boyvate NGO</div>
            <div class="tl-place">Feb 2026</div>
          </div>
          <span class="tl-badge done">Completed Mar 2026</span>
        </div>
      </div>
    </div>

  </div>
</section>

<!-- ═══ PROJECTS ═══ -->
<section>
  <p class="section-label">Projects</p>

  <div class="cat-label">🎓 University &amp; Campus Systems</div>
  <div class="proj-grid">
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://chukauniversitytimetabling.pythonanywhere.com/" target="_blank">Chuka University Timetabling</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">AI-driven class scheduling. <strong>0% conflicts</strong>, 3–5 hrs → &lt;10 sec, 1000ms → <strong>5ms</strong> response time. Deployed university-wide.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">Python</span><span class="pstag">AI</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://samuelkibunja.pythonanywhere.com/" target="_blank">MultApp — Campus Super App</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Unified student hub: timetables, exams, notes, mess menus, and Comrade Corner for campus music & culture.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">JavaScript</span><span class="pstag">REST</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://afya-wise-connect.vercel.app/" target="_blank">Afya Wise Connect</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Mental health + radio platform with AI-adaptive content. Partnered with Chuka Radio. Emergency integration with Chuka University Dispensary.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">AI/ML</span><span class="pstag">Vercel</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://samuelkibunja.pythonanywhere.com/hostels/" target="_blank">Hostel Finder</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Smart student house hunting with heuristic matching algorithms, integrated maps, and 3D directional views campus to hostel.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">Maps API</span><span class="pstag">3D</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://dravtechattachmentassistant.pythonanywhere.com/" target="_blank">Attachment Assistant</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Daily-scraped internship listings, AI curation, profile-based ranking, and in-platform email applications directly to companies.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">Scraping</span><span class="pstag">AI</span><span class="pstag">Email</span></div>
    </div>
  </div>

  <div class="cat-label">💬 Communication &amp; Community</div>
  <div class="proj-grid">
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://samuelkibunja.pythonanywhere.com/chat/" target="_blank">UniChat</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Secure real-time messaging for intra/inter-university use. Any-size doc sharing, group chats, and polls. Open to all universities.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">WebSocket</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://samuelkibunja.pythonanywhere.com/confessions/" target="_blank">Confession &amp; Guidance</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Anonymous counselling, mentorship & rehabilitation platform. Full identity anonymisation. Counsellor interaction and contact exchange built-in.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">REST</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://samuelkibunja.pythonanywhere.com/religion/" target="_blank">Religion Connect</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Interdenominational platform for all faiths — upload content, plan events, schedule prayers and meetings. Every religion in one space.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">CMS</span></div>
    </div>
  </div>

  <div class="cat-label">📰 News, Politics &amp; Civic Tech</div>
  <div class="proj-grid">
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://newshubke.pythonanywhere.com/" target="_blank">NewsHub KE</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">AI news aggregation: multi-source scraping, story linking, video summaries per topic, historical timelines, and ML personalisation.</p>
      <div class="proj-stack"><span class="pstag">React</span><span class="pstag">Django</span><span class="pstag">AI/ML</span><span class="pstag">Scraping</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://samuelkibunja.pythonanywhere.com/politics/" target="_blank">Politics Pulse</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Aggregates and groups political news by topic into one clean interactive feed. A clear window into Kenya's political landscape.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">Scraping</span></div>
    </div>
  </div>

  <div class="cat-label">🏗️ Engineering, Finance &amp; Marketplace</div>
  <div class="proj-grid">
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://projectteam2025.pythonanywhere.com/" target="_blank">Construction Management System</a></div>
        <span class="proj-status s-dev">Migrating to Java</span>
      </div>
      <p class="proj-desc">End-to-end construction ops: IoT sensors, AI/ML for material cost optimisation, structural compliance, real-time analytics, predictive project tracking.</p>
      <div class="proj-stack"><span class="pstag">Java</span><span class="pstag">Django</span><span class="pstag">IoT</span><span class="pstag">AI/ML</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name">Forex Predictor &amp; Quant Engine</div>
        <span class="proj-status s-dev">In Development</span>
      </div>
      <p class="proj-desc">Real-time market data crawling, quantitative analysis, and custom ML model for currency movement prediction with algorithmic trading logic.</p>
      <div class="proj-stack"><span class="pstag">Python</span><span class="pstag">ML</span><span class="pstag">Quant Finance</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://github.com/DRAVIS55" target="_blank">Java Currency Converter &amp; Predictor</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Real-time converter with <strong>54% forecasting accuracy</strong> via ML algorithms and live financial API feeds.</p>
      <div class="proj-stack"><span class="pstag">Java</span><span class="pstag">ML</span><span class="pstag">Finance APIs</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://samuelkibunja.pythonanywhere.com/marketplace/" target="_blank">Campus Marketplace</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Student second-hand marketplace with algorithmic listing verification before items go live. Clean, categorised UI.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">JavaScript</span></div>
    </div>
  </div>

  <div class="cat-label">🏢 Client &amp; Commercial Projects</div>
  <div class="proj-grid">
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="http://lowlandshotel.com" target="_blank">Lowlands Hotel &amp; Spa</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Full rebuild: luxury responsive UI, JWT REST API, <strong>5-role dashboard</strong>, online booking with availability, contact CMS, Docker-ready infrastructure.</p>
      <div class="proj-stack"><span class="pstag">React</span><span class="pstag">Vite</span><span class="pstag">Node.js</span><span class="pstag">MySQL</span><span class="pstag">Docker</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="http://www.hopeandhomeke.com" target="_blank">Hope and Home KE</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">E-commerce platform for an interior décor brand with interactive UI/UX and seamless product discovery and ordering.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">E-commerce</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://solaryora.pythonanywhere.com/" target="_blank">Soyanala Solar</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">Online marketplace for a solar energy company. Customers browse, compare, and purchase solar products directly from the platform.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">E-commerce</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name"><a href="https://glassgrow.pythonanywhere.com/" target="_blank">Grassroot Development Kenya</a></div>
        <span class="proj-status s-live">Live</span>
      </div>
      <p class="proj-desc">NGO platform with <strong>PayPal, M-Pesa, card, and Sui Blockchain</strong> donation channels. Real-time CMS and cloud infrastructure.</p>
      <div class="proj-stack"><span class="pstag">Django</span><span class="pstag">M-Pesa</span><span class="pstag">Blockchain</span></div>
    </div>
    <div class="proj-card">
      <div class="proj-top">
        <div class="proj-name">LEZOL Engineering Platform</div>
        <span class="proj-status s-prod">In Production</span>
      </div>
      <p class="proj-desc">Production e-commerce platform digitising engineering business operations end-to-end with scalable architecture for real-world transactions.</p>
      <div class="proj-stack"><span class="pstag">Node.js</span><span class="pstag">React</span></div>
    </div>
  </div>
</section>

<!-- ═══ TECH STACK ═══ -->
<section>
  <p class="section-label">Tech Stack</p>

  <div class="tech-section">
    <h4>Languages</h4>
    <div class="tech-grid">
      <span class="tech-chip"><svg viewBox="0 0 24 24" fill="none"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>Python</span>
      <span class="tech-chip"><svg viewBox="0 0 24 24" fill="none"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>JavaScript</span>
      <span class="tech-chip"><svg viewBox="0 0 24 24" fill="none"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>TypeScript</span>
      <span class="tech-chip"><svg viewBox="0 0 24 24" fill="none"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>Java</span>
      <span class="tech-chip"><svg viewBox="0 0 24 24" fill="none"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>C++</span>
      <span class="tech-chip"><svg viewBox="0 0 24 24" fill="none"><path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>PHP</span>
    </div>
  </div>

  <div class="tech-section">
    <h4>Frameworks &amp; Backend</h4>
    <div class="tech-grid">
      <span class="tech-chip">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M11.146 0h3.924l.858 3.357L18.79 2.16l2.776 2.777-1.16 2.86L24 8.95v3.924l-3.357.853 1.16 2.86-2.776 2.777-2.86-1.16-.854 3.356h-3.924l-.853-3.357-2.86 1.16-2.777-2.776 1.157-2.86L0 12.875V8.95l3.357-.854L2.2 5.234l2.777-2.777 2.86 1.16z"/></svg>
        Django
      </span>
      <span class="tech-chip">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M11.572 0c-.176 0-.31.001-.358.007a19.76 19.76 0 01-.364.033C7.443.346 4.25 2.185 2.228 5.012a11.875 11.875 0 00-2.119 5.243c-.096.659-.108.854-.108 1.747s.012 1.089.108 1.748c.652 4.506 3.86 8.292 8.209 9.695.779.25 1.6.422 2.534.525.363.04 1.935.04 2.299 0 1.611-.178 2.977-.577 4.323-1.264.207-.106.247-.134.219-.158-.02-.013-.9-1.193-1.955-2.62l-1.919-2.592-2.404-3.558a338.739 338.739 0 00-2.422-3.556c-.009-.002-.018 1.579-.023 3.51-.007 3.38-.01 3.515-.052 3.595a.426.426 0 01-.206.214c-.075.037-.14.044-.495.044H7.81l-.108-.068a.438.438 0 01-.157-.171l-.05-.106.006-4.703.007-4.705.072-.092a.645.645 0 01.174-.143c.096-.047.134-.052.54-.052.479 0 .558.019.683.155.023.026 1.333 1.994 2.913 4.395l4.63 6.948 1.86 2.793c.106.164.181.282.188.296.009.016-.062.055-.18.109a8.636 8.636 0 01-1.064.384c-.617.164-1.217.257-1.946.295-.306.015-1.112.01-1.4-.008a10.368 10.368 0 01-3.83-.99 10.487 10.487 0 01-4.516-4.516 10.293 10.293 0 01-.991-3.832c-.041-.523-.041-1.42.001-1.957a10.308 10.308 0 016.001-8.69A10.28 10.28 0 0112.05 1.78c.373-.02 1.246-.02 1.607 0a10.326 10.326 0 014.23 1.13.645.645 0 01.2.172l.05.086-.019 4.68-.021 4.682-1.41-2.126a1748.74 1748.74 0 00-2.821-4.248c-.7-1.048-1.282-1.918-1.294-1.933-.016-.02-.023 1.31-.027 3.664l-.007 3.689H14.2l.01-5.022c.008-4.814.01-5.02.054-5.096a.435.435 0 01.194-.2c.082-.038.13-.046.453-.046.359 0 .37.002.466.06l.1.06L17.46 8.3l2.017 3.049.015-4.718.017-4.717.082-.084.084-.084h.562c.486 0 .573.003.645.033.1.04.168.102.213.195.03.064.033.26.033 5.067v4.997l-.065.093c-.103.145-.273.217-.535.217-.292 0-.427-.044-.574-.187-.038-.037-1.153-1.71-2.476-3.718L15.09 4.74c-.006-.008-.01 1.55-.012 3.46l-.006 3.47H8.5L6.47 4.86c-.016-.024-.026.97-.027 3.337l-.006 3.337-.108.005-.108.006-1.08.016c-.73.011-1.1.009-1.13-.006-.027-.014-.067-.053-.088-.087l-.04-.062V3.85l.04-.07a.484.484 0 01.114-.14c.066-.052.11-.068.266-.09.098-.014.677-.02 1.288-.013l1.11.012 2.035 3.065c2.188 3.293 3.054 4.598 3.072 4.602a1.256 1.256 0 00.051.003V.05l.007-.028A.527.527 0 0111.572 0z"/></svg>
        Next.js
      </span>
      <span class="tech-chip">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M14.23 12.004a2.236 2.236 0 0 1-2.235 2.236 2.236 2.236 0 0 1-2.236-2.236 2.236 2.236 0 0 1 2.235-2.236 2.236 2.236 0 0 1 2.236 2.236zm2.648-10.69c-1.346 0-3.107.96-4.888 2.622-1.78-1.653-3.542-2.602-4.887-2.602-.41 0-.783.093-1.106.278-1.375.793-1.683 3.264-.973 6.365C1.98 8.917 0 10.42 0 12.004c0 1.59 1.99 3.097 5.043 4.03-.704 3.113-.39 5.588.988 6.38.32.187.69.275 1.102.275 1.345 0 3.107-.96 4.888-2.624 1.78 1.654 3.542 2.603 4.887 2.603.41 0 .783-.09 1.106-.275 1.374-.792 1.683-3.263.973-6.365C22.02 15.096 24 13.59 24 12.004c0-1.59-1.99-3.097-5.043-4.032.704-3.11.39-5.587-.988-6.38a2.167 2.167 0 0 0-1.092-.278zm-.005 1.09c.074 0 .14.018.192.048.464.276.382 1.95-.27 4.202A23.49 23.49 0 0 0 12 6.498a23.49 23.49 0 0 0-4.795.826C6.562 5.006 6.48 3.33 6.942 3.055c.05-.03.118-.048.19-.048.72 0 2.027.929 3.622 2.485a23.782 23.782 0 0 1 2.247 2.651 23.782 23.782 0 0 1 2.248-2.65c1.594-1.557 2.9-2.486 3.623-2.486zm-13.726.187c.08 0 .167.02.253.063.464.276.382 1.95-.27 4.202A23.49 23.49 0 0 0 .604 12.004c0 1.284 1.402 2.5 3.734 3.349-.286 1.256-.39 2.4-.295 3.32a5.266 5.266 0 0 1-.074.025C1.98 15.098 0 13.59 0 12.004c0-1.59 1.99-3.097 5.043-4.032a9.16 9.16 0 0 1 .104-.323c.704-3.11.39-5.588-.988-6.38a2.167 2.167 0 0 0-1.092-.277zm.001 0a2.14 2.14 0 0 0-.005 0z"/></svg>
        React
      </span>
      <span class="tech-chip">Node.js</span>
      <span class="tech-chip">FastAPI</span>
      <span class="tech-chip">Express.js</span>
    </div>
  </div>

  <div class="tech-section">
    <h4>Databases</h4>
    <div class="tech-grid">
      <span class="tech-chip">PostgreSQL</span>
      <span class="tech-chip">MySQL</span>
      <span class="tech-chip">MongoDB</span>
      <span class="tech-chip">Firebase</span>
    </div>
  </div>

  <div class="tech-section">
    <h4>Tools &amp; Platforms</h4>
    <div class="tech-grid">
      <span class="tech-chip">Docker</span>
      <span class="tech-chip">Git</span>
      <span class="tech-chip">Linux</span>
      <span class="tech-chip">AWS</span>
      <span class="tech-chip">Nginx</span>
      <span class="tech-chip">VS Code</span>
    </div>
  </div>

  <div class="tech-section">
    <h4>Blockchain &amp; Web3</h4>
    <div class="tech-grid">
      <span class="tech-chip">Solidity</span>
      <span class="tech-chip">Web3.js</span>
      <span class="tech-chip">Sui Blockchain</span>
    </div>
  </div>
</section>

<!-- ═══ CERTIFICATIONS ═══ -->
<section>
  <p class="section-label">Certifications</p>
  <div class="cert-list">
    <div class="cert-item">
      <div>
        <div class="cert-name">Django Full-Stack Development</div>
        <div class="cert-issuer">eMobilis</div>
      </div>
      <span class="cert-badge">Full-Stack</span>
    </div>
    <div class="cert-item">
      <div>
        <div class="cert-name">MERN Stack Development</div>
        <div class="cert-issuer">Edureka</div>
      </div>
      <span class="cert-badge">Full-Stack</span>
    </div>
    <div class="cert-item">
      <div>
        <div class="cert-name">CCST Networking Certification</div>
        <div class="cert-issuer">Cisco</div>
      </div>
      <span class="cert-badge">Networking</span>
    </div>
    <div class="cert-item">
      <div>
        <div class="cert-name">Data Analysis Certification</div>
        <div class="cert-issuer">KESAP Researchers</div>
      </div>
      <span class="cert-badge">Data</span>
    </div>
    <div class="cert-item">
      <div>
        <div class="cert-name">Software Engineering</div>
        <div class="cert-issuer">PLP Academy</div>
      </div>
      <span class="cert-badge">Engineering</span>
    </div>
    <div class="cert-item">
      <div>
        <div class="cert-name">AutoScheduler Pitch — MUSTIEW 2025</div>
        <div class="cert-issuer">Meru University</div>
      </div>
      <span class="cert-badge">Achievement</span>
    </div>
  </div>
</section>

</div><!-- /page -->

<!-- ═══ FOOTER ═══ -->
<footer class="footer">
  <div class="footer-inner">
    <p class="footer-motto">Code. <span>Innovate.</span> Secure.</p>
    <div class="footer-links">
      <a class="pill" href="mailto:samuelkibunja55@gmail.com">Email</a>
      <a class="pill" href="https://www.linkedin.com/in/samuelkibunja/" target="_blank">LinkedIn</a>
      <a class="pill" href="https://github.com/DRAVIS55" target="_blank">GitHub</a>
      <a class="pill" href="https://x.com/samuelkibu87288" target="_blank">Twitter / X</a>
      <a class="pill" href="https://wa.me/254758067458" target="_blank">WhatsApp</a>
    </div>
  </div>
</footer>

</body>
</html>
