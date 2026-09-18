<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Jean Noguera — Systems Engineer</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#0A0A0A; --bg2:#0F172A; --blue:#2563EB; --violet:#7C3AED; --fg:#F5F5F7;
  --muted:#9AA3B2; --line:rgba(255,255,255,.09); --card:#101322;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--fg);font-family:'Inter',system-ui,sans-serif;line-height:1.55;overflow-x:hidden}
h1,h2,h3,.disp{font-family:'Space Grotesk',system-ui,sans-serif}
a{color:inherit;text-decoration:none}
.wrap{max-width:1040px;margin:0 auto;padding:0 24px}
section{padding:96px 0}
.eyebrow{color:var(--muted);font-size:.85rem;margin-bottom:10px}
nav{position:fixed;top:0;left:0;right:0;z-index:50;backdrop-filter:blur(10px);background:rgba(10,10,10,.6);border-bottom:1px solid var(--line)}
nav .wrap{display:flex;justify-content:space-between;align-items:center;padding:16px 24px}
nav .brand{font-family:'Space Grotesk';font-weight:600}
nav .links a{color:var(--muted);margin-left:22px;font-size:.9rem}
nav .links a:hover{color:var(--fg)}

/* HERO */
.hero{min-height:100vh;display:flex;align-items:center;position:relative;padding-top:80px}
.hero:before{content:"";position:absolute;inset:0;background:
  radial-gradient(600px 400px at 15% 20%, rgba(37,99,235,.22), transparent 60%),
  radial-gradient(500px 400px at 85% 75%, rgba(124,58,237,.20), transparent 60%);
  z-index:-1}
.hero .eyebrow{color:var(--blue)}
.hero h1{font-size:clamp(2.6rem,6vw,4.4rem);font-weight:700;letter-spacing:-.02em;line-height:1.05}
.hero .role{color:var(--muted);font-size:1.15rem;margin-top:14px;max-width:560px}
.hero p.lead{margin-top:22px;font-size:1.05rem;color:#D6D9E3;max-width:600px}
.cta-row{display:flex;flex-wrap:wrap;gap:12px;margin-top:34px}
.btn{padding:12px 22px;border-radius:8px;font-size:.9rem;font-weight:500;border:1px solid var(--line);transition:transform .15s ease}
.btn:hover{transform:translateY(-2px)}
.btn.primary{background:linear-gradient(135deg,var(--blue),var(--violet));border:none}
.btn.ghost{background:transparent;color:var(--fg)}

/* ABOUT */
.about-grid{display:grid;grid-template-columns:1.3fr 1fr;gap:56px}
.about-grid p{color:#C7CBD6;margin-bottom:16px}
.stats{display:grid;grid-template-columns:1fr 1fr;gap:18px}
.stat{border:1px solid var(--line);border-radius:12px;padding:18px;background:var(--card)}
.stat .num{font-family:'Space Grotesk';font-size:1.8rem;font-weight:700;color:var(--blue)}
.stat .lbl{color:var(--muted);font-size:.82rem;margin-top:4px}

/* EXPERTISE */
.exp-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
.exp-card{border:1px solid var(--line);border-radius:12px;padding:22px;background:var(--card)}
.exp-card h3{font-size:1.02rem;margin-bottom:8px}
.exp-card p{color:var(--muted);font-size:.87rem}

/* STACK */
.stack-grid{display:flex;flex-wrap:wrap;gap:10px}
.chip{border:1px solid var(--line);border-radius:999px;padding:8px 16px;font-size:.83rem;color:#D6D9E3;background:var(--card)}

/* TIMELINE */
.timeline{position:relative;padding-left:28px;border-left:2px solid var(--line)}
.t-item{position:relative;margin-bottom:34px}
.t-item:before{content:"";position:absolute;left:-34px;top:4px;width:12px;height:12px;border-radius:50%;background:var(--blue);box-shadow:0 0 0 4px rgba(37,99,235,.18)}
.t-item.goal:before{background:var(--violet);box-shadow:0 0 0 4px rgba(124,58,237,.18)}
.t-item h3{font-size:1.02rem}
.t-item p{color:var(--muted);font-size:.87rem;margin-top:2px}

/* CERTS */
.cert-list{display:grid;gap:10px}
.cert-row{display:flex;justify-content:space-between;align-items:center;border:1px solid var(--line);border-radius:10px;padding:14px 18px;background:var(--card);font-size:.9rem}
.cert-row .org{color:var(--muted);font-size:.82rem}

/* CONTACT */
.contact-row{display:flex;flex-wrap:wrap;gap:14px;margin-top:24px}
footer{padding:40px 0;color:var(--muted);font-size:.8rem;border-top:1px solid var(--line);text-align:center}

@media(max-width:760px){
  .about-grid{grid-template-columns:1fr}
  .exp-grid{grid-template-columns:1fr 1fr}
}
@media(max-width:480px){ .exp-grid{grid-template-columns:1fr} }
</style>
</head>
<body>

<nav><div class="wrap">
  <span class="brand">JN</span>
  <div class="links">
    <a href="#about">About</a><a href="#expertise">Expertise</a><a href="#journey">Journey</a><a href="#certs">Certifications</a><a href="#contact">Contact</a>
  </div>
</div></nav>

<section class="hero"><div class="wrap">
  <div class="eyebrow">Barranquilla, Colombia</div>
  <h1>Jean Noguera</h1>
  <div class="role">Systems Engineer · Senior Service Desk Analyst · Microsoft 365 Specialist</div>
  <p class="lead">I turn enterprise technology problems into calm, working systems — supporting Microsoft ecosystems, cloud environments and security-conscious infrastructure at scale.</p>
  <div class="cta-row">
    <a class="btn primary" href="#contact">Schedule a conversation</a>
    <a class="btn ghost" href="#certs">See certifications</a>
    <a class="btn ghost" href="https://www.linkedin.com/in/ingenierojeannoguera/">Connect on LinkedIn</a>
  </div>
</div></section>

<section id="about"><div class="wrap about-grid">
  <div>
    <div class="eyebrow">Who I am</div>
    <h2 style="font-size:1.8rem;margin-bottom:16px">Enterprise support, built on an engineering foundation</h2>
    <p>I support end users and infrastructure across calls, chat, email and ticketing systems — keeping Microsoft 365, Azure, Intune and Active Directory environments running smoothly for the people who depend on them.</p>
    <p>My background in Systems Engineering and Telematics Network Security shapes how I approach every ticket: not just closing it, but understanding the system behind it. I'm currently completing a postgraduate degree in Information Security, aiming toward Cloud Engineering and Cybersecurity.</p>
  </div>
  <div class="stats">
    <div class="stat"><div class="num">15+</div><div class="lbl">Enterprise technologies</div></div>
    <div class="stat"><div class="num">7</div><div class="lbl">Certifications</div></div>
    <div class="stat"><div class="num">4</div><div class="lbl">Support channels</div></div>
    <div class="stat"><div class="num">2</div><div class="lbl">Languages</div></div>
  </div>
</div></section>

<section id="expertise"><div class="wrap">
  <div class="eyebrow">Expertise</div>
  <h2 style="font-size:1.8rem;margin-bottom:24px">Where I add value</h2>
  <div class="exp-grid">
    <div class="exp-card"><h3>Microsoft Ecosystem</h3><p>365, Exchange, Teams, Intune, Entra ID, Active Directory</p></div>
    <div class="exp-card"><h3>Cloud Technologies</h3><p>Azure administration and cloud-based service delivery</p></div>
    <div class="exp-card"><h3>Enterprise Support</h3><p>Ticketing, SLAs, escalation paths, customer satisfaction</p></div>
    <div class="exp-card"><h3>Identity & Access</h3><p>Entra ID, Active Directory, access provisioning</p></div>
    <div class="exp-card"><h3>Networking & Infra</h3><p>VPN, VDI, Citrix, core networking fundamentals</p></div>
    <div class="exp-card"><h3>Security Operations</h3><p>SOC fundamentals, security best practices, SOAR basics</p></div>
  </div>
</div></section>

<section id="stack"><div class="wrap">
  <div class="eyebrow">Tools I work in daily</div>
  <div class="stack-grid">
    <span class="chip">Microsoft 365</span><span class="chip">Azure</span><span class="chip">Intune</span>
    <span class="chip">Entra ID</span><span class="chip">Active Directory</span><span class="chip">Citrix</span>
    <span class="chip">Jira</span><span class="chip">SysAid</span><span class="chip">SAP</span>
    <span class="chip">NinjaOne</span><span class="chip">TeamViewer</span><span class="chip">VPN</span>
    <span class="chip">VDI</span><span class="chip">ManageEngine</span>
  </div>
</div></section>

<section id="journey"><div class="wrap">
  <div class="eyebrow">Career journey</div>
  <h2 style="font-size:1.8rem;margin-bottom:28px">From technician to engineer</h2>
  <div class="timeline">
    <div class="t-item"><h3>System Technician — SENA</h3><p>Foundations in hardware, networking and support</p></div>
    <div class="t-item"><h3>Systems Engineering Student — Universidad Simón Bolívar</h3><p>Engineering and telematics network security</p></div>
    <div class="t-item"><h3>Jr. Service Desk Analyst → Service Desk Analyst</h3><p>Enterprise support across Microsoft environments</p></div>
    <div class="t-item"><h3>Senior Service Desk Analyst</h3><p>Current role — leading resolution, mentoring, process improvement</p></div>
    <div class="t-item goal"><h3>Next: Cloud Engineer or Cybersecurity Professional</h3><p>Postgraduate degree in Information Security in progress</p></div>
  </div>
</div></section>

<section id="certs"><div class="wrap">
  <div class="eyebrow">Certifications</div>
  <h2 style="font-size:1.8rem;margin-bottom:24px">Credentials</h2>
  <div class="cert-list">
    <div class="cert-row"><span>Microsoft 365 Fundamentals (MS-900)</span><span class="org">Microsoft</span></div>
    <div class="cert-row"><span>Jira Service Management Fundamentals</span><span class="org">Atlassian</span></div>
    <div class="cert-row"><span>Security Operations Fundamentals</span><span class="org">Google</span></div>
    <div class="cert-row"><span>SOAR Fundamentals</span><span class="org">Google</span></div>
    <div class="cert-row"><span>Networking Basics</span><span class="org">Cisco</span></div>
    <div class="cert-row"><span>Operating Systems Basics</span><span class="org">Cisco</span></div>
    <div class="cert-row"><span>Computer Hardware Basics</span><span class="org">Cisco</span></div>
  </div>
</div></section>

<section id="contact"><div class="wrap">
  <div class="eyebrow">Get in touch</div>
  <h2 style="font-size:1.8rem">Let's talk</h2>
  <p style="color:var(--muted);margin-top:12px;max-width:520px">Open to recruitment conversations, technical networking and career opportunities in Cloud, Infrastructure and Information Security.</p>
  <div class="contact-row">
    <a class="btn primary" href="mailto:jeannoguera@outlook.es">Email me</a>
    <a class="btn ghost" href="https://www.linkedin.com/in/ingenierojeannoguera/">LinkedIn</a>
  </div>
</div></section>

<footer>Jean Noguera — Barranquilla, Colombia</footer>
</body>
</html>
