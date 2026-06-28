<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>République du Bénin — Portail Politique National</title>
  <link rel="preconnect" href="https://fonts.googleapis.com"/>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
  <link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=Inter:wght@300;400;500;600&family=DM+Serif+Display:ital@0;1&display=swap" rel="stylesheet"/>
  <style>
    *,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
    :root{
      --g:#008751;--y:#FCD116;--r:#E8112D;
      --dark:#070C10;--dark2:#0D1520;--dark3:#131E2B;
      --slate:#1E2D3D;--mid:#2A3F54;
      --accent:#00D4FF;--accent2:#FFB800;
      --text:#E8EDF2;--muted:#7A8FA0;--rule:rgba(255,255,255,0.07);
      --syne:'Syne',sans-serif;--inter:'Inter',sans-serif;--dm:'DM Serif Display',serif;
    }
    html{scroll-behavior:smooth;font-size:16px}
    body{font-family:var(--inter);background:var(--dark);color:var(--text);-webkit-font-smoothing:antialiased;overflow-x:hidden}

    .ticker{background:var(--g);height:36px;display:flex;align-items:center;overflow:hidden}
    .ticker-label{background:var(--y);color:#000;font-family:var(--syne);font-size:.65rem;font-weight:700;letter-spacing:.15em;text-transform:uppercase;padding:0 1.25rem;height:100%;display:flex;align-items:center;flex-shrink:0}
    .ticker-track{display:flex;animation:ticker 40s linear infinite;white-space:nowrap;gap:4rem}
    .ticker-track span{font-size:.72rem;letter-spacing:.08em;color:rgba(255,255,255,.9)}
    .ticker-track span::before{content:'◆';margin-right:.75rem;opacity:.5}
    @keyframes ticker{0%{transform:translateX(0)}100%{transform:translateX(-50%)}}

    nav{position:sticky;top:0;z-index:200;background:rgba(7,12,16,.95);backdrop-filter:blur(20px);border-bottom:1px solid var(--rule)}
    .nav-inner{max-width:1400px;margin:0 auto;padding:0 2.5rem;height:68px;display:flex;align-items:center;justify-content:space-between;gap:2rem}
    .nav-logo{display:flex;align-items:center;gap:.75rem;text-decoration:none}
    .nav-logo-flag{font-size:1.4rem}
    .nav-logo-text{font-family:var(--syne);font-size:1rem;font-weight:800;color:var(--text);letter-spacing:.02em;line-height:1.1}
    .nav-logo-text small{display:block;font-size:.6rem;font-weight:400;color:var(--muted);letter-spacing:.15em;text-transform:uppercase}
    .nav-links{display:flex;gap:.25rem;list-style:none}
    .nav-links a{font-size:.72rem;font-weight:600;letter-spacing:.1em;text-transform:uppercase;color:var(--muted);text-decoration:none;padding:.5rem .85rem;border-radius:4px;transition:all .2s}
    .nav-links a:hover{color:var(--text);background:var(--rule)}
    .nav-cta{background:var(--g);color:#fff;font-family:var(--syne);font-size:.72rem;font-weight:700;letter-spacing:.1em;text-transform:uppercase;border:none;padding:.55rem 1.25rem;cursor:pointer;transition:background .2s}
    .nav-cta:hover{background:#006b40}

    .hero{position:relative;min-height:100vh;display:flex;flex-direction:column;justify-content:flex-end;overflow:hidden;padding-bottom:5rem}
    .hero-bg{position:absolute;inset:0;background:radial-gradient(ellipse 80% 60% at 60% 40%,rgba(0,135,81,.18) 0%,transparent 60%),radial-gradient(ellipse 60% 80% at 10% 80%,rgba(0,212,255,.08) 0%,transparent 50%),linear-gradient(170deg,#070C10 0%,#0D1520 50%,#070C10 100%)}
    .hero-grid{position:absolute;inset:0;background-image:linear-gradient(var(--rule) 1px,transparent 1px),linear-gradient(90deg,var(--rule) 1px,transparent 1px);background-size:60px 60px;mask-image:radial-gradient(ellipse 80% 80% at 50% 50%,black 30%,transparent 80%)}
    .hero-flag-bg{position:absolute;right:-5%;top:50%;transform:translateY(-50%);font-size:32vw;opacity:.025;pointer-events:none;user-select:none;filter:blur(2px)}
    .hero-content{position:relative;z-index:2;max-width:1400px;margin:0 auto;padding:0 2.5rem;width:100%}
    .hero-eyebrow{display:inline-flex;align-items:center;gap:.6rem;font-size:.68rem;font-weight:600;letter-spacing:.2em;text-transform:uppercase;color:var(--accent);margin-bottom:2rem}
    .hero-eyebrow::before{content:'';display:block;width:24px;height:1px;background:var(--accent)}
    .hero-title{font-family:var(--syne);font-size:clamp(3rem,6vw,7rem);font-weight:800;line-height:.95;letter-spacing:-.02em;color:#fff;margin-bottom:1.5rem;max-width:900px}
    .hero-title .line2{color:transparent;-webkit-text-stroke:1px rgba(255,255,255,.25)}
    .hero-title .accent{color:var(--y)}
    .hero-lead{font-size:1.05rem;color:var(--muted);max-width:560px;line-height:1.8;margin-bottom:3.5rem;font-weight:300}
    .hero-actions{display:flex;gap:1rem;flex-wrap:wrap;margin-bottom:5rem}
    .btn-primary{display:inline-flex;align-items:center;gap:.6rem;background:var(--g);color:#fff;font-family:var(--syne);font-size:.78rem;font-weight:700;letter-spacing:.1em;text-transform:uppercase;text-decoration:none;padding:.85rem 2rem;transition:all .2s}
    .btn-primary:hover{background:#006b40;transform:translateY(-1px)}
    .btn-secondary{display:inline-flex;align-items:center;gap:.6rem;background:transparent;color:var(--text);font-family:var(--syne);font-size:.78rem;font-weight:700;letter-spacing:.1em;text-transform:uppercase;text-decoration:none;padding:.85rem 2rem;border:1px solid rgba(255,255,255,.15);transition:all .2s}
    .btn-secondary:hover{border-color:var(--accent);color:var(--accent)}
    .hero-kpis{display:grid;grid-template-columns:repeat(4,1fr);gap:0;border-top:1px solid var(--rule)}
    .kpi{padding:2rem 0;border-right:1px solid var(--rule)}
    .kpi:last-child{border-right:none}
    .kpi-num{font-family:var(--syne);font-size:2.8rem;font-weight:800;line-height:1;color:#fff;margin-bottom:.35rem}
    .kpi-num span{font-size:1.5rem;color:var(--y)}
    .kpi-label{font-size:.68rem;letter-spacing:.12em;text-transform:uppercase;color:var(--muted)}

    .breaking{background:var(--dark2);border-top:3px solid var(--r);border-bottom:1px solid var(--rule);padding:1rem 2.5rem;display:flex;align-items:center;gap:1.5rem}
    .breaking-badge{background:var(--r);color:#fff;font-family:var(--syne);font-size:.62rem;font-weight:800;letter-spacing:.15em;text-transform:uppercase;padding:.35rem .75rem;flex-shrink:0}
    .breaking-text{font-size:.82rem;color:rgba(255,255,255,.7);line-height:1.5}
    .breaking-text strong{color:#fff}

    .wrapper{max-width:1400px;margin:0 auto;padding:0 2.5rem}
    .sec-header{display:flex;align-items:flex-end;justify-content:space-between;margin-bottom:3rem;padding-bottom:1.5rem;border-bottom:1px solid var(--rule)}
    .sec-tag{font-size:.65rem;font-weight:700;letter-spacing:.2em;text-transform:uppercase;color:var(--accent);margin-bottom:.6rem}
    .sec-title{font-family:var(--syne);font-size:clamp(1.6rem,2.5vw,2.4rem);font-weight:800;line-height:1.1;color:#fff}
    .sec-link{font-size:.72rem;font-weight:600;letter-spacing:.1em;text-transform:uppercase;color:var(--muted);text-decoration:none;transition:color .2s;flex-shrink:0}
    .sec-link:hover{color:var(--accent)}

    /* HISTOIRE */
    .histoire{padding:6rem 0}
    .timeline-modern{display:grid;grid-template-columns:1fr;gap:0;position:relative}
    .timeline-modern::before{content:'';position:absolute;left:120px;top:0;bottom:0;width:1px;background:linear-gradient(to bottom,transparent,var(--g) 10%,var(--y) 50%,var(--r) 90%,transparent)}
    .tl-item{display:grid;grid-template-columns:120px 1fr;gap:0;padding:2.5rem 0;border-bottom:1px solid var(--rule);position:relative}
    .tl-item:last-child{border-bottom:none}
    .tl-year{font-family:var(--syne);font-size:1rem;font-weight:800;color:var(--muted);padding-right:2rem;padding-top:.2rem;text-align:right;line-height:1}
    .tl-dot{position:absolute;left:112px;top:2.85rem;width:17px;height:17px;border-radius:50%;background:var(--dark);border:2px solid var(--g);z-index:1}
    .tl-item:nth-child(3) .tl-dot{border-color:var(--y)}
    .tl-item:nth-child(5) .tl-dot{border-color:var(--accent)}
    .tl-item:nth-child(7) .tl-dot{border-color:var(--r)}
    .tl-body{padding-left:3rem}
    .tl-tag{display:inline-block;font-size:.6rem;font-weight:700;letter-spacing:.15em;text-transform:uppercase;padding:.2rem .6rem;margin-bottom:.6rem;border-radius:2px}
    .tl-tag.ind{background:rgba(0,135,81,.15);color:var(--g)}
    .tl-tag.coup{background:rgba(232,17,45,.15);color:var(--r)}
    .tl-tag.demo{background:rgba(0,212,255,.15);color:var(--accent)}
    .tl-tag.mod{background:rgba(252,209,22,.15);color:var(--y)}
    .tl-h{font-family:var(--syne);font-size:1.15rem;font-weight:700;color:#fff;margin-bottom:.5rem;line-height:1.2}
    .tl-p{font-size:.88rem;color:var(--muted);line-height:1.8}

    /* INSTITUTIONS */
    .institutions{padding:6rem 0;background:var(--dark2)}
    .inst-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1px;background:var(--rule)}
    .inst-card{background:var(--dark2);padding:2.5rem;transition:background .25s;position:relative;overflow:hidden}
    .inst-card::before{content:'';position:absolute;inset:0;background:linear-gradient(135deg,rgba(0,135,81,.05) 0%,transparent 60%);opacity:0;transition:opacity .25s}
    .inst-card:hover{background:var(--dark3)}
    .inst-card:hover::before{opacity:1}
    .inst-icon{width:48px;height:48px;border-radius:8px;background:rgba(0,135,81,.12);border:1px solid rgba(0,135,81,.2);display:flex;align-items:center;justify-content:center;font-size:1.4rem;margin-bottom:1.5rem}
    .inst-name{font-family:var(--syne);font-size:1rem;font-weight:700;color:#fff;margin-bottom:.5rem;line-height:1.3}
    .inst-abbr{font-size:.65rem;letter-spacing:.15em;text-transform:uppercase;color:var(--accent);margin-bottom:.75rem;font-weight:600}
    .inst-desc{font-size:.85rem;color:var(--muted);line-height:1.8}

    /* PARTIS */
    .partis-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:1.5rem}
    .parti-card{background:var(--dark2);border:1px solid var(--rule);padding:2.5rem;position:relative;overflow:hidden;transition:border-color .25s}
    .parti-card::after{content:'';position:absolute;top:0;left:0;right:0;height:3px}
    .parti-card:nth-child(1)::after{background:var(--g)}
    .parti-card:nth-child(2)::after{background:var(--accent)}
    .parti-card:nth-child(3)::after{background:var(--y)}
    .parti-card:nth-child(4)::after{background:var(--r)}
    .parti-card:hover{border-color:rgba(255,255,255,.15)}
    .parti-header{display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:1rem;gap:1rem}
    .parti-name{font-family:var(--syne);font-size:1.1rem;font-weight:700;color:#fff;line-height:1.3}
    .parti-badge{flex-shrink:0;font-size:.6rem;font-weight:700;letter-spacing:.12em;text-transform:uppercase;padding:.3rem .7rem;border-radius:2px}
    .badge-power{background:rgba(0,135,81,.15);color:var(--g);border:1px solid rgba(0,135,81,.3)}
    .badge-opp{background:rgba(0,212,255,.1);color:var(--accent);border:1px solid rgba(0,212,255,.2)}
    .parti-sigle{font-size:.68rem;letter-spacing:.12em;text-transform:uppercase;color:var(--muted);margin-bottom:.75rem}
    .parti-desc{font-size:.88rem;color:rgba(255,255,255,.55);line-height:1.8}

    /* ENJEUX */
    .enjeux{padding:6rem 0;background:var(--dark2)}
    .enjeux-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1.5rem}
    .enjeu-card{background:var(--dark3);border:1px solid var(--rule);padding:2rem;transition:all .25s}
    .enjeu-card:hover{border-color:rgba(0,212,255,.2);transform:translateY(-3px);box-shadow:0 12px 40px rgba(0,0,0,.3)}
    .enjeu-icon{font-size:1.5rem;margin-bottom:.75rem}
    .enjeu-title{font-family:var(--syne);font-size:1rem;font-weight:700;color:#fff;margin-bottom:.75rem;line-height:1.3}
    .enjeu-text{font-size:.83rem;color:var(--muted);line-height:1.8}
    .enjeu-status{display:inline-flex;align-items:center;gap:.4rem;font-size:.62rem;font-weight:600;letter-spacing:.1em;text-transform:uppercase;margin-top:1rem;padding:.3rem .65rem;border-radius:2px}
    .status-critical{background:rgba(232,17,45,.12);color:var(--r);border:1px solid rgba(232,17,45,.2)}
    .status-active{background:rgba(252,209,22,.12);color:var(--y);border:1px solid rgba(252,209,22,.2)}
    .status-progress{background:rgba(0,212,255,.1);color:var(--accent);border:1px solid rgba(0,212,255,.2)}
    .status-dot{width:5px;height:5px;border-radius:50%;background:currentColor}

    /* CONSTITUTION */
    .constitution{padding:6rem 0}
    .const-layout{display:grid;grid-template-columns:1fr 1fr;gap:4rem;align-items:center}
    .const-doc{background:var(--dark2);border:1px solid var(--rule);padding:3rem;position:relative;overflow:hidden}
    .const-date{font-family:var(--dm);font-size:3.5rem;font-style:italic;color:var(--y);margin-bottom:.5rem;line-height:1}
    .const-subtitle{font-family:var(--syne);font-size:.72rem;font-weight:700;letter-spacing:.2em;text-transform:uppercase;color:var(--muted);margin-bottom:2rem}
    .const-pillars{display:flex;flex-direction:column;gap:1px;background:var(--rule)}
    .const-pillar{background:var(--dark2);padding:1rem 1.25rem;display:flex;align-items:center;gap:1rem}
    .pillar-bar{width:3px;height:32px;flex-shrink:0;border-radius:2px}
    .pillar-bar.g{background:var(--g)}.pillar-bar.y{background:var(--y)}.pillar-bar.r{background:var(--r)}.pillar-bar.a{background:var(--accent)}
    .pillar-text{font-size:.82rem;color:rgba(255,255,255,.65);line-height:1.5}
    .const-text{font-size:.9rem;color:var(--muted);line-height:1.9}
    .const-text p{margin-bottom:1rem}
    .const-articles{display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-top:2rem}
    .article-item{background:var(--dark2);border:1px solid var(--rule);padding:1.25rem;transition:border-color .2s}
    .article-item:hover{border-color:rgba(0,135,81,.4)}
    .art-num{font-family:var(--syne);font-size:.68rem;font-weight:700;letter-spacing:.12em;text-transform:uppercase;color:var(--g);margin-bottom:.4rem}
    .art-title{font-size:.82rem;font-weight:600;color:#fff;margin-bottom:.3rem}
    .art-desc{font-size:.75rem;color:var(--muted);line-height:1.6}

    /* PRESIDENCE */
    .presidence{padding:6rem 0;background:var(--dark2)}
    .pres-layout{display:grid;grid-template-columns:5fr 4fr;gap:4rem;align-items:center}
    .pres-badge{display:inline-flex;align-items:center;gap:.5rem;background:rgba(0,135,81,.1);border:1px solid rgba(0,135,81,.2);padding:.4rem 1rem;font-size:.65rem;font-weight:700;letter-spacing:.15em;text-transform:uppercase;color:var(--g);margin-bottom:1.5rem}
    .pres-name{font-family:var(--syne);font-size:clamp(2rem,3.5vw,3.5rem);font-weight:800;color:#fff;line-height:1.05;margin-bottom:.5rem}
    .pres-title-sub{font-size:.88rem;color:var(--muted);margin-bottom:2rem;font-weight:300}
    .pres-bio{font-size:.9rem;color:rgba(255,255,255,.55);line-height:1.9;margin-bottom:2.5rem}
    .pres-stats{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem}
    .pres-stat{background:var(--dark3);border:1px solid var(--rule);padding:1.25rem;text-align:center}
    .pres-stat-n{font-family:var(--syne);font-size:1.6rem;font-weight:800;color:var(--y);line-height:1}
    .pres-stat-l{font-size:.65rem;letter-spacing:.1em;text-transform:uppercase;color:var(--muted);margin-top:.3rem}
    .pres-card-visual{background:var(--dark3);border:1px solid var(--rule);padding:2.5rem;display:flex;flex-direction:column;gap:1.5rem}
    .pres-card-title{font-family:var(--syne);font-size:.72rem;font-weight:700;letter-spacing:.15em;text-transform:uppercase;color:var(--muted);padding-bottom:1rem;border-bottom:1px solid var(--rule)}
    .mandate-bar{position:relative;height:6px;background:rgba(255,255,255,.07);border-radius:3px;overflow:hidden;margin-bottom:.4rem}
    .mandate-fill{position:absolute;left:0;top:0;bottom:0;background:linear-gradient(90deg,var(--g),var(--y));width:60%;border-radius:3px}
    .mandate-label{display:flex;justify-content:space-between;font-size:.68rem;color:var(--muted)}
    .timeline-mini{display:flex;flex-direction:column;gap:.75rem}
    .mini-item{display:flex;gap:.75rem;align-items:flex-start;font-size:.78rem}
    .mini-dot{width:8px;height:8px;border-radius:50%;background:var(--g);flex-shrink:0;margin-top:.2rem}
    .mini-item:nth-child(2) .mini-dot{background:var(--accent)}
    .mini-item:nth-child(3) .mini-dot{background:var(--y)}
    .mini-year{color:var(--muted);flex-shrink:0;font-weight:600;min-width:35px}
    .mini-text{color:rgba(255,255,255,.6)}

    /* ══ BIOGRAPHIE ROCK — REDESIGN COMPLET ══ */
    .bio-section{padding:0;background:var(--dark);position:relative;overflow:hidden}
    .bio-top-band{background:var(--g);height:4px;width:100%}
    .bio-inner{display:grid;grid-template-columns:420px 1fr;min-height:700px}

    /* Photo side */
    .bio-photo-col{position:relative;overflow:hidden}
    .bio-photo-col img{width:100%;height:100%;object-fit:cover;object-position:center top;display:block;filter:brightness(.92) contrast(1.05)}
    .bio-photo-overlay{position:absolute;inset:0;background:linear-gradient(to right,transparent 60%,var(--dark) 100%),linear-gradient(to top,rgba(7,12,16,.7) 0%,transparent 40%)}
    .bio-photo-badge{position:absolute;bottom:2.5rem;left:2rem;right:2rem}
    .bio-photo-name{font-family:var(--syne);font-size:1.5rem;font-weight:800;color:#fff;line-height:1.1;text-shadow:0 2px 12px rgba(0,0,0,.5)}
    .bio-photo-role{font-size:.7rem;letter-spacing:.15em;text-transform:uppercase;color:var(--y);margin-top:.35rem;font-weight:600}

    /* Content side */
    .bio-content-col{padding:4rem 4rem 4rem 3rem;display:flex;flex-direction:column;justify-content:center;position:relative}
    .bio-content-col::before{content:'RSH';position:absolute;right:-1rem;top:50%;transform:translateY(-50%);font-family:var(--syne);font-size:18rem;font-weight:800;color:rgba(0,135,81,.04);pointer-events:none;line-height:1;letter-spacing:-.04em}
    .bio-eyebrow{display:inline-flex;align-items:center;gap:.6rem;font-size:.65rem;font-weight:700;letter-spacing:.22em;text-transform:uppercase;color:var(--g);margin-bottom:1.25rem}
    .bio-eyebrow::before{content:'';display:block;width:20px;height:1px;background:var(--g)}
    .bio-headline{font-family:var(--syne);font-size:clamp(2rem,3vw,3rem);font-weight:800;color:#fff;line-height:1.0;letter-spacing:-.02em;margin-bottom:.4rem}
    .bio-headline .hl{color:var(--y)}
    .bio-role-line{font-size:.85rem;color:var(--g);font-weight:600;letter-spacing:.04em;margin-bottom:2.5rem;padding-bottom:2.5rem;border-bottom:1px solid var(--rule)}
    .bio-para{font-size:.93rem;color:rgba(255,255,255,.58);line-height:2;margin-bottom:1rem}
    .bio-para strong{color:rgba(255,255,255,.85);font-weight:600}
    .bio-quote-block{border-left:2px solid var(--g);padding:1.25rem 1.5rem;margin:2rem 0;background:rgba(0,135,81,.04)}
    .bio-quote-block p{font-family:var(--dm);font-size:1.1rem;font-style:italic;color:rgba(255,255,255,.45);line-height:1.7}
    .bio-quote-block cite{display:block;font-size:.65rem;letter-spacing:.15em;text-transform:uppercase;color:var(--g);margin-top:.75rem;font-style:normal}
    .bio-pillars-row{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem;margin-top:2.5rem}
    .bio-pillar-item{background:var(--dark2);border:1px solid var(--rule);padding:1.25rem;transition:border-color .2s;text-align:center}
    .bio-pillar-item:hover{border-color:rgba(0,135,81,.4)}
    .bio-pillar-emoji{font-size:1.4rem;margin-bottom:.5rem}
    .bio-pillar-word{font-family:var(--syne);font-size:.85rem;font-weight:700;color:#fff;margin-bottom:.2rem}
    .bio-pillar-sub{font-size:.7rem;color:var(--muted);line-height:1.5}

    /* FOOTER */
    footer{background:var(--dark);border-top:1px solid var(--rule)}
    .footer-top{padding:4rem 0;display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:3rem}
    .footer-brand p{font-size:.85rem;color:var(--muted);line-height:1.8;margin-top:1rem;max-width:280px}
    .footer-col-title{font-family:var(--syne);font-size:.68r
