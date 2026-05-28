[hct-ub-partnership.html](https://github.com/user-attachments/files/28333614/hct-ub-partnership.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>MSN in Critical Care for Elderly Patients | HCT × University of Barcelona</title>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Playfair+Display:wght@600;700&display=swap" rel="stylesheet" />
  <style>
    /* ─── Design Tokens ─────────────────────────────────────────── */
    :root {
      --navy:        #1A2D4A;
      --navy-deep:   #0F1C30;
      --teal:        #00B4C8;
      --teal-dark:   #008FA0;
      --teal-light:  #E4F7FA;
      --teal-mid:    #B2EBF2;
      --ub-red:      #C1272D;
      --ub-red-dark: #961F23;
      --white:       #FFFFFF;
      --off-white:   #F8FAFB;
      --gray-100:    #F3F4F6;
      --gray-200:    #E5E7EB;
      --gray-400:    #9CA3AF;
      --gray-600:    #4B5563;
      --gray-800:    #1F2937;
      --shadow-sm:   0 1px 3px rgba(0,0,0,.08), 0 1px 2px rgba(0,0,0,.06);
      --shadow-md:   0 4px 16px rgba(0,0,0,.10);
      --shadow-lg:   0 10px 32px rgba(0,0,0,.14);
      --radius:      12px;
      --radius-lg:   20px;
    }

    /* ─── Reset & Base ───────────────────────────────────────────── */
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      font-family: 'Inter', sans-serif;
      color: var(--gray-800);
      background: var(--white);
      line-height: 1.6;
    }
    img { display: block; max-width: 100%; }
    a { color: inherit; text-decoration: none; }

    /* ─── Utility ────────────────────────────────────────────────── */
    .container { max-width: 1120px; margin: 0 auto; padding: 0 24px; }
    .section-label {
      display: inline-block;
      font-size: .75rem;
      font-weight: 700;
      letter-spacing: .12em;
      text-transform: uppercase;
      color: var(--teal);
      margin-bottom: 12px;
    }
    .section-label.light { color: var(--teal-mid); }
    .section-title {
      font-family: 'Playfair Display', serif;
      font-size: clamp(1.75rem, 3.5vw, 2.5rem);
      line-height: 1.2;
      color: var(--navy);
    }
    .section-title.light { color: var(--white); }
    .section-intro {
      font-size: 1.05rem;
      color: var(--gray-600);
      max-width: 660px;
      margin-top: 16px;
    }
    .section-intro.light { color: rgba(255,255,255,.8); }
    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 14px 28px;
      border-radius: 8px;
      font-weight: 600;
      font-size: .95rem;
      cursor: pointer;
      border: 2px solid transparent;
      transition: all .2s;
    }
    .btn-primary {
      background: var(--teal);
      color: var(--white);
    }
    .btn-primary:hover { background: var(--teal-dark); transform: translateY(-1px); box-shadow: var(--shadow-md); }
    .btn-outline {
      background: transparent;
      color: var(--white);
      border-color: rgba(255,255,255,.5);
    }
    .btn-outline:hover { border-color: var(--white); background: rgba(255,255,255,.08); }
    .btn-navy {
      background: var(--navy);
      color: var(--white);
    }
    .btn-navy:hover { background: var(--navy-deep); transform: translateY(-1px); box-shadow: var(--shadow-md); }

    /* ─── Top Bar ────────────────────────────────────────────────── */
    .top-bar {
      background: var(--navy-deep);
      color: rgba(255,255,255,.65);
      font-size: .78rem;
      padding: 8px 0;
      text-align: center;
      letter-spacing: .02em;
    }
    .top-bar strong { color: var(--teal); }

    /* ─── Site Header ────────────────────────────────────────────── */
    .site-header {
      background: var(--white);
      border-bottom: 1px solid var(--gray-200);
      position: sticky;
      top: 0;
      z-index: 100;
      box-shadow: var(--shadow-sm);
    }
    .header-inner {
      display: flex;
      align-items: center;
      justify-content: space-between;
      height: 68px;
    }
    .header-logo img {
      height: 44px;
      width: auto;
    }
    .header-logo .logo-fallback {
      display: flex;
      align-items: center;
      gap: 10px;
    }
    .logo-mark {
      background: var(--teal);
      color: var(--white);
      font-weight: 800;
      font-size: 1.1rem;
      padding: 6px 10px;
      border-radius: 6px;
    }
    .logo-text { font-weight: 700; font-size: 1rem; color: var(--navy); line-height: 1.2; }
    .logo-text span { display: block; font-weight: 400; font-size: .72rem; color: var(--gray-400); }
    .site-nav { display: flex; align-items: center; gap: 28px; }
    .site-nav a {
      font-size: .88rem;
      font-weight: 500;
      color: var(--gray-600);
      transition: color .15s;
    }
    .site-nav a:hover { color: var(--navy); }
    .site-nav a.active {
      color: var(--teal-dark);
      font-weight: 600;
      border-bottom: 2px solid var(--teal);
      padding-bottom: 2px;
    }
    .header-cta { display: flex; align-items: center; gap: 12px; }

    /* ─── Breadcrumb ─────────────────────────────────────────────── */
    .breadcrumb {
      background: var(--gray-100);
      padding: 10px 0;
      font-size: .8rem;
      color: var(--gray-400);
    }
    .breadcrumb ol { display: flex; align-items: center; gap: 6px; list-style: none; }
    .breadcrumb li::after { content: "/"; margin-left: 6px; }
    .breadcrumb li:last-child::after { content: ""; }
    .breadcrumb a { color: var(--teal-dark); font-weight: 500; }
    .breadcrumb li:last-child { color: var(--gray-600); font-weight: 500; }

    /* ─── Hero ───────────────────────────────────────────────────── */
    .hero {
      background: linear-gradient(135deg, var(--navy-deep) 0%, var(--navy) 45%, #1E4060 100%);
      position: relative;
      overflow: hidden;
      padding: 80px 0 90px;
    }
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%2300B4C8' fill-opacity='0.04'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
    }
    .hero::after {
      content: '';
      position: absolute;
      right: -120px;
      top: -80px;
      width: 600px;
      height: 600px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(0,180,200,.12) 0%, transparent 70%);
      pointer-events: none;
    }
    .hero-inner {
      position: relative;
      z-index: 1;
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 48px;
      align-items: center;
    }
    .hero-badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: rgba(0,180,200,.15);
      border: 1px solid rgba(0,180,200,.3);
      color: var(--teal-mid);
      font-size: .78rem;
      font-weight: 600;
      letter-spacing: .08em;
      text-transform: uppercase;
      padding: 6px 14px;
      border-radius: 100px;
      margin-bottom: 20px;
    }
    .hero-badge .dot {
      width: 6px; height: 6px; border-radius: 50%;
      background: var(--teal);
      animation: pulse 2s ease-in-out infinite;
    }
    @keyframes pulse {
      0%, 100% { opacity: 1; transform: scale(1); }
      50% { opacity: .5; transform: scale(1.3); }
    }
    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(2rem, 4vw, 3rem);
      color: var(--white);
      line-height: 1.2;
      margin-bottom: 20px;
    }
    .hero h1 em {
      font-style: normal;
      color: var(--teal);
    }
    .hero-subtitle {
      font-size: 1.1rem;
      color: rgba(255,255,255,.75);
      max-width: 540px;
      margin-bottom: 32px;
      line-height: 1.7;
    }
    .hero-actions { display: flex; gap: 14px; flex-wrap: wrap; }
    .hero-stats {
      display: flex;
      gap: 32px;
      margin-top: 48px;
      padding-top: 32px;
      border-top: 1px solid rgba(255,255,255,.1);
    }
    .stat { text-align: left; }
    .stat-number {
      font-size: 1.75rem;
      font-weight: 800;
      color: var(--teal);
      line-height: 1;
    }
    .stat-label { font-size: .8rem; color: rgba(255,255,255,.55); margin-top: 4px; }

    /* Partnership logos card */
    .partner-card {
      background: rgba(255,255,255,.06);
      border: 1px solid rgba(255,255,255,.12);
      border-radius: var(--radius-lg);
      padding: 32px 28px;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 20px;
      backdrop-filter: blur(12px);
      min-width: 240px;
    }
    .partner-card .divider {
      display: flex;
      align-items: center;
      gap: 12px;
      color: rgba(255,255,255,.4);
      font-size: .75rem;
      font-weight: 600;
      letter-spacing: .1em;
      width: 100%;
    }
    .partner-card .divider::before,
    .partner-card .divider::after {
      content: '';
      flex: 1;
      height: 1px;
      background: rgba(255,255,255,.15);
    }
    .partner-logo-wrap {
      background: var(--white);
      border-radius: 10px;
      padding: 12px 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      width: 180px;
      min-height: 72px;
    }
    .partner-logo-wrap img {
      max-height: 48px;
      width: auto;
      object-fit: contain;
    }
    /* UB logo fallback */
    .ub-logo-fallback {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 4px;
    }
    .ub-crest {
      width: 48px;
      height: 48px;
      background: var(--ub-red);
      border-radius: 8px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-weight: 800;
      font-size: 1.2rem;
      font-family: 'Playfair Display', serif;
    }
    .ub-name {
      font-size: .65rem;
      color: var(--navy);
      font-weight: 600;
      text-align: center;
      line-height: 1.3;
    }
    /* HCT logo fallback */
    .hct-logo-fallback {
      display: flex;
      align-items: center;
      gap: 10px;
    }
    .hct-mark {
      background: var(--teal);
      color: var(--white);
      font-weight: 800;
      font-size: 1rem;
      padding: 8px 10px;
      border-radius: 6px;
      letter-spacing: .05em;
    }
    .hct-name {
      font-size: .7rem;
      color: var(--navy);
      font-weight: 600;
      line-height: 1.3;
    }
    .x-badge {
      width: 32px;
      height: 32px;
      background: linear-gradient(135deg, var(--teal), var(--teal-dark));
      color: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      font-size: .85rem;
      flex-shrink: 0;
    }

    /* ─── Section spacing ────────────────────────────────────────── */
    .section { padding: 80px 0; }
    .section-alt { background: var(--off-white); }
    .section-dark { background: var(--navy); }
    .section-teal { background: var(--teal-light); }

    /* ─── About Section ──────────────────────────────────────────── */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 60px;
      align-items: start;
      margin-top: 48px;
    }
    .about-visual {
      position: relative;
    }
    .about-visual-main {
      background: linear-gradient(135deg, var(--teal-light), var(--teal-mid));
      border-radius: var(--radius-lg);
      padding: 48px 40px;
      display: flex;
      flex-direction: column;
      gap: 24px;
    }
    .program-pill {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: var(--white);
      border: 1px solid var(--teal-mid);
      padding: 8px 16px;
      border-radius: 100px;
      font-size: .85rem;
      font-weight: 600;
      color: var(--teal-dark);
    }
    .program-pill svg { flex-shrink: 0; }
    .floating-card {
      position: absolute;
      background: var(--white);
      border-radius: var(--radius);
      padding: 16px 20px;
      box-shadow: var(--shadow-lg);
      display: flex;
      align-items: center;
      gap: 12px;
    }
    .floating-card.card-1 { bottom: -20px; right: -20px; }
    .floating-card.card-2 { top: 24px; left: -32px; }
    .fc-icon {
      width: 40px; height: 40px; border-radius: 8px;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.2rem; flex-shrink: 0;
    }
    .fc-icon.teal { background: var(--teal-light); }
    .fc-icon.red { background: #FFF0F0; }
    .fc-text .fc-label { font-size: .72rem; color: var(--gray-400); }
    .fc-text .fc-value { font-size: .9rem; font-weight: 700; color: var(--navy); }
    .info-list { display: flex; flex-direction: column; gap: 16px; }
    .info-item {
      display: flex;
      gap: 16px;
      align-items: flex-start;
      padding: 16px;
      background: var(--white);
      border-radius: var(--radius);
      border: 1px solid var(--gray-200);
    }
    .info-icon {
      width: 42px; height: 42px;
      background: var(--teal-light);
      border-radius: 10px;
      display: flex; align-items: center; justify-content: center;
      flex-shrink: 0;
      font-size: 1.1rem;
    }
    .info-title { font-weight: 600; font-size: .9rem; color: var(--navy); }
    .info-desc { font-size: .83rem; color: var(--gray-600); margin-top: 2px; }

    /* ─── Curriculum ─────────────────────────────────────────────── */
    .curriculum-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
      margin-top: 48px;
    }
    .curriculum-card {
      background: var(--white);
      border: 1px solid var(--gray-200);
      border-radius: var(--radius);
      overflow: hidden;
      transition: transform .2s, box-shadow .2s;
    }
    .curriculum-card:hover { transform: translateY(-4px); box-shadow: var(--shadow-md); }
    .curriculum-card-header {
      padding: 20px 20px 16px;
      border-bottom: 1px solid var(--gray-200);
    }
    .phase-badge {
      font-size: .7rem;
      font-weight: 700;
      letter-spacing: .1em;
      text-transform: uppercase;
      color: var(--teal-dark);
      background: var(--teal-light);
      padding: 4px 10px;
      border-radius: 100px;
      display: inline-block;
      margin-bottom: 10px;
    }
    .curriculum-card h3 {
      font-size: 1rem;
      font-weight: 700;
      color: var(--navy);
      line-height: 1.3;
    }
    .curriculum-card-body { padding: 16px 20px; }
    .module-list { list-style: none; display: flex; flex-direction: column; gap: 10px; }
    .module-list li {
      display: flex;
      gap: 10px;
      font-size: .83rem;
      color: var(--gray-600);
      align-items: flex-start;
    }
    .module-list li::before {
      content: '›';
      color: var(--teal);
      font-weight: 700;
      flex-shrink: 0;
      margin-top: 1px;
    }

    /* ─── Why This Program ───────────────────────────────────────── */
    .why-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 20px;
      margin-top: 48px;
    }
    .why-card {
      background: rgba(255,255,255,.07);
      border: 1px solid rgba(255,255,255,.1);
      border-radius: var(--radius);
      padding: 28px;
      transition: background .2s;
    }
    .why-card:hover { background: rgba(255,255,255,.11); }
    .why-icon {
      font-size: 2rem;
      margin-bottom: 14px;
    }
    .why-card h3 {
      font-size: 1rem;
      font-weight: 700;
      color: var(--white);
      margin-bottom: 8px;
    }
    .why-card p { font-size: .85rem; color: rgba(255,255,255,.65); line-height: 1.6; }

    /* ─── Partnership Logos Feature ──────────────────────────────── */
    .partners-showcase {
      display: grid;
      grid-template-columns: 1fr auto 1fr;
      gap: 32px;
      align-items: center;
      background: var(--white);
      border: 1px solid var(--gray-200);
      border-radius: var(--radius-lg);
      padding: 40px 48px;
      margin-top: 48px;
      box-shadow: var(--shadow-sm);
    }
    .partner-info { display: flex; flex-direction: column; gap: 12px; }
    .partner-info:last-child { align-items: flex-end; text-align: right; }
    .partner-logo-box {
      height: 72px;
      display: flex;
      align-items: center;
    }
    .partner-logo-box img { max-height: 60px; width: auto; object-fit: contain; }
    .partner-desc { font-size: .85rem; color: var(--gray-600); max-width: 280px; line-height: 1.6; }
    .partner-detail { font-size: .78rem; color: var(--gray-400); }
    .partner-detail strong { color: var(--gray-600); }
    .x-connector {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 8px;
    }
    .x-ring {
      width: 64px; height: 64px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--teal), var(--teal-dark));
      display: flex; align-items: center; justify-content: center;
      color: white; font-size: 1.5rem; font-weight: 800;
      box-shadow: 0 4px 16px rgba(0,180,200,.3);
    }
    .x-label { font-size: .7rem; color: var(--gray-400); font-weight: 600; letter-spacing: .08em; text-transform: uppercase; }

    /* ─── Requirements ───────────────────────────────────────────── */
    .req-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 28px;
      margin-top: 48px;
    }
    .req-block {
      background: var(--white);
      border: 1px solid var(--gray-200);
      border-radius: var(--radius);
      padding: 28px;
    }
    .req-block h3 {
      font-weight: 700;
      color: var(--navy);
      font-size: .95rem;
      margin-bottom: 16px;
      display: flex;
      align-items: center;
      gap: 10px;
    }
    .req-block h3 .req-num {
      width: 28px; height: 28px; border-radius: 50%;
      background: var(--teal-light);
      color: var(--teal-dark);
      font-size: .78rem; font-weight: 700;
      display: flex; align-items: center; justify-content: center;
      flex-shrink: 0;
    }
    .req-list { list-style: none; display: flex; flex-direction: column; gap: 10px; }
    .req-list li {
      display: flex;
      gap: 10px;
      font-size: .85rem;
      color: var(--gray-600);
      align-items: flex-start;
    }
    .req-list li .check {
      color: var(--teal-dark);
      font-weight: 700;
      flex-shrink: 0;
      margin-top: 1px;
    }

    /* ─── Timeline ───────────────────────────────────────────────── */
    .timeline {
      display: flex;
      gap: 0;
      margin-top: 48px;
      position: relative;
    }
    .timeline::before {
      content: '';
      position: absolute;
      top: 32px;
      left: 0; right: 0;
      height: 2px;
      background: var(--gray-200);
      z-index: 0;
    }
    .timeline-step {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      position: relative;
      z-index: 1;
    }
    .tl-dot {
      width: 64px; height: 64px; border-radius: 50%;
      background: var(--white);
      border: 3px solid var(--gray-200);
      display: flex; align-items: center; justify-content: center;
      font-size: 1.4rem;
      margin-bottom: 16px;
      transition: border-color .2s, background .2s;
    }
    .timeline-step.active .tl-dot {
      background: var(--teal-light);
      border-color: var(--teal);
    }
    .tl-title { font-weight: 700; font-size: .88rem; color: var(--navy); margin-bottom: 4px; }
    .tl-date { font-size: .78rem; color: var(--teal-dark); font-weight: 600; margin-bottom: 6px; }
    .tl-desc { font-size: .78rem; color: var(--gray-400); max-width: 140px; }

    /* ─── Survey / Form ──────────────────────────────────────────── */
    .survey-section {
      background: linear-gradient(135deg, var(--navy-deep) 0%, var(--navy) 100%);
      position: relative;
      overflow: hidden;
    }
    .survey-section::before {
      content: '';
      position: absolute;
      left: -100px; top: -100px;
      width: 500px; height: 500px;
      background: radial-gradient(circle, rgba(0,180,200,.1) 0%, transparent 70%);
    }
    .survey-inner {
      position: relative;
      z-index: 1;
      display: grid;
      grid-template-columns: 1fr 1.2fr;
      gap: 60px;
      align-items: start;
    }
    .survey-info { padding-top: 16px; }
    .survey-info h2 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(1.6rem, 3vw, 2.2rem);
      color: var(--white);
      line-height: 1.2;
      margin-bottom: 16px;
    }
    .survey-info p { color: rgba(255,255,255,.7); font-size: .95rem; line-height: 1.7; margin-bottom: 28px; }
    .benefit-list { display: flex; flex-direction: column; gap: 12px; }
    .benefit-item {
      display: flex;
      align-items: center;
      gap: 12px;
      font-size: .88rem;
      color: rgba(255,255,255,.8);
    }
    .benefit-item .bi-icon {
      width: 32px; height: 32px;
      background: rgba(0,180,200,.2);
      border-radius: 8px;
      display: flex; align-items: center; justify-content: center;
      font-size: .9rem; flex-shrink: 0;
    }
    .form-card {
      background: var(--white);
      border-radius: var(--radius-lg);
      padding: 36px 32px;
      box-shadow: var(--shadow-lg);
    }
    .form-card h3 {
      font-size: 1.15rem;
      font-weight: 700;
      color: var(--navy);
      margin-bottom: 4px;
    }
    .form-card .form-sub {
      font-size: .83rem;
      color: var(--gray-400);
      margin-bottom: 24px;
    }
    .form-group { margin-bottom: 18px; }
    .form-group label {
      display: block;
      font-size: .82rem;
      font-weight: 600;
      color: var(--gray-600);
      margin-bottom: 6px;
    }
    .form-group label .req { color: var(--ub-red); margin-left: 2px; }
    .form-control {
      width: 100%;
      padding: 11px 14px;
      border: 1.5px solid var(--gray-200);
      border-radius: 8px;
      font-size: .88rem;
      font-family: inherit;
      color: var(--gray-800);
      background: var(--white);
      transition: border-color .15s, box-shadow .15s;
      outline: none;
      appearance: none;
    }
    .form-control:focus {
      border-color: var(--teal);
      box-shadow: 0 0 0 3px rgba(0,180,200,.15);
    }
    select.form-control {
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='8' viewBox='0 0 12 8'%3E%3Cpath d='M1 1l5 5 5-5' stroke='%239CA3AF' stroke-width='1.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: no-repeat;
      background-position: right 14px center;
      padding-right: 36px;
    }
    .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
    .radio-group { display: flex; flex-direction: column; gap: 8px; }
    .radio-item {
      display: flex;
      align-items: center;
      gap: 10px;
      padding: 10px 12px;
      border: 1.5px solid var(--gray-200);
      border-radius: 8px;
      cursor: pointer;
      transition: border-color .15s, background .15s;
      font-size: .85rem;
      color: var(--gray-600);
    }
    .radio-item:hover { border-color: var(--teal); background: var(--teal-light); }
    .radio-item input[type="radio"] { accent-color: var(--teal); }
    .checkbox-group { display: flex; flex-direction: column; gap: 8px; }
    .checkbox-item {
      display: flex;
      align-items: flex-start;
      gap: 10px;
      font-size: .83rem;
      color: var(--gray-600);
    }
    .checkbox-item input[type="checkbox"] { accent-color: var(--teal); margin-top: 2px; flex-shrink: 0; }
    .form-note { font-size: .76rem; color: var(--gray-400); margin-top: 8px; line-height: 1.5; }
    .submit-btn {
      width: 100%;
      padding: 15px;
      background: linear-gradient(135deg, var(--teal), var(--teal-dark));
      color: var(--white);
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      font-weight: 700;
      cursor: pointer;
      font-family: inherit;
      transition: opacity .2s, transform .2s;
      margin-top: 8px;
    }
    .submit-btn:hover { opacity: .9; transform: translateY(-1px); box-shadow: 0 6px 20px rgba(0,180,200,.35); }
    .form-footer {
      margin-top: 16px;
      text-align: center;
      font-size: .76rem;
      color: var(--gray-400);
    }
    .form-footer a { color: var(--teal-dark); text-decoration: underline; }

    /* ─── FAQ ────────────────────────────────────────────────────── */
    .faq-list { display: flex; flex-direction: column; gap: 12px; margin-top: 48px; max-width: 800px; }
    .faq-item {
      border: 1px solid var(--gray-200);
      border-radius: var(--radius);
      overflow: hidden;
    }
    .faq-q {
      width: 100%;
      background: var(--white);
      border: none;
      padding: 18px 24px;
      text-align: left;
      font-size: .92rem;
      font-weight: 600;
      color: var(--navy);
      cursor: pointer;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 16px;
      font-family: inherit;
      transition: background .15s;
    }
    .faq-q:hover { background: var(--gray-100); }
    .faq-q .arrow { color: var(--teal); font-size: 1.2rem; transition: transform .2s; }
    .faq-q[aria-expanded="true"] .arrow { transform: rotate(180deg); }
    .faq-a {
      max-height: 0;
      overflow: hidden;
      transition: max-height .3s ease;
      background: var(--off-white);
    }
    .faq-a.open { max-height: 300px; }
    .faq-a-inner {
      padding: 0 24px 18px;
      font-size: .88rem;
      color: var(--gray-600);
      line-height: 1.7;
    }

    /* ─── Footer ─────────────────────────────────────────────────── */
    .site-footer {
      background: var(--navy-deep);
      color: rgba(255,255,255,.55);
      padding: 48px 0 28px;
    }
    .footer-inner {
      display: grid;
      grid-template-columns: 2fr 1fr 1fr;
      gap: 48px;
      padding-bottom: 36px;
      border-bottom: 1px solid rgba(255,255,255,.08);
      margin-bottom: 24px;
    }
    .footer-brand p { font-size: .83rem; line-height: 1.7; margin-top: 14px; max-width: 300px; }
    .footer-logo { margin-bottom: 4px; }
    .footer-logo img { height: 40px; width: auto; filter: brightness(0) invert(1); opacity: .9; }
    .footer-logo .logo-fallback-footer {
      display: flex; align-items: center; gap: 10px;
    }
    .footer-logo .fmk {
      background: var(--teal);
      color: white; font-weight: 800;
      padding: 6px 10px; border-radius: 6px; font-size: 1rem;
    }
    .footer-logo .ftx { color: white; font-weight: 600; font-size: .9rem; }
    .footer-col h4 { font-size: .82rem; font-weight: 700; letter-spacing: .08em; text-transform: uppercase; color: rgba(255,255,255,.8); margin-bottom: 14px; }
    .footer-col ul { list-style: none; display: flex; flex-direction: column; gap: 8px; }
    .footer-col li a { font-size: .83rem; color: rgba(255,255,255,.5); transition: color .15s; }
    .footer-col li a:hover { color: var(--teal); }
    .footer-bottom {
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: .78rem;
    }
    .footer-bottom a { color: var(--teal); }

    /* ─── Success State ───────────────────────────────────────────── */
    .success-overlay {
      display: none;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 40px;
      gap: 16px;
    }
    .success-overlay .check-circle {
      width: 64px; height: 64px; border-radius: 50%;
      background: #E8FFF4;
      border: 2px solid #34D399;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.8rem;
      margin: 0 auto;
    }
    .success-overlay h3 { color: var(--navy); font-size: 1.15rem; }
    .success-overlay p { color: var(--gray-600); font-size: .88rem; line-height: 1.6; }

    /* ─── Responsive ─────────────────────────────────────────────── */
    @media (max-width: 900px) {
      .hero-inner { grid-template-columns: 1fr; }
      .partner-card { display: none; }
      .about-grid { grid-template-columns: 1fr; }
      .floating-card.card-2 { display: none; }
      .floating-card.card-1 { position: static; margin-top: 16px; }
      .curriculum-grid { grid-template-columns: 1fr; }
      .why-grid { grid-template-columns: 1fr; }
      .partners-showcase { grid-template-columns: 1fr; justify-items: center; text-align: center; }
      .partner-info:last-child { align-items: center; text-align: center; }
      .req-grid { grid-template-columns: 1fr; }
      .survey-inner { grid-template-columns: 1fr; }
      .form-row { grid-template-columns: 1fr; }
      .footer-inner { grid-template-columns: 1fr; gap: 28px; }
      .footer-bottom { flex-direction: column; gap: 8px; text-align: center; }
      .hero-stats { gap: 20px; }
      .site-nav { display: none; }
      .timeline { flex-direction: column; gap: 20px; align-items: flex-start; padding-left: 32px; }
      .timeline::before { width: 2px; height: auto; top: 0; bottom: 0; left: 32px; right: auto; }
      .timeline-step { flex-direction: row; align-items: flex-start; text-align: left; }
      .tl-dot { margin-bottom: 0; margin-right: 16px; flex-shrink: 0; }
    }
  </style>
</head>
<body>

  <!-- Top Bar -->
  <div class="top-bar">
    <strong>New Partnership Announcement</strong> — HCT Philippines × University of Barcelona &nbsp;|&nbsp; MSN Critical Care for Elderly Patients &nbsp;|&nbsp; Applications open 2025
  </div>

  <!-- Site Header -->
  <header class="site-header">
    <div class="container">
      <div class="header-inner">
        <!-- HCT Logo -->
        <a href="https://www.hct.ph" class="header-logo">
          <img
            src="https://www.hct.ph/cdn/shop/files/HCT_Full_Identity_Colored_White_Transparent_a2ccca9d-6e80-4983-8bfc-c705f8a9c6fd.png"
            alt="HCT — Healthcare and Technology"
            onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
          />
          <div class="logo-fallback" style="display:none;">
            <div class="logo-mark">HCT</div>
            <div class="logo-text">Healthcare & Technology<span>Philippines</span></div>
          </div>
        </a>

        <!-- Navigation -->
        <nav class="site-nav" aria-label="Main navigation">
          <a href="#">Home</a>
          <a href="#">About Us</a>
          <a href="#">Our Programs</a>
          <a href="#" class="active">International Partnerships</a>
          <a href="#">Media</a>
          <a href="#">Contact</a>
        </nav>

        <!-- CTA -->
        <div class="header-cta">
          <a href="#interest-form" class="btn btn-primary" style="padding:10px 20px;font-size:.85rem;">Express Interest</a>
        </div>
      </div>
    </div>
  </header>

  <!-- Breadcrumb -->
  <nav class="breadcrumb" aria-label="Breadcrumb">
    <div class="container">
      <ol>
        <li><a href="#">Home</a></li>
        <li><a href="#">International Partnerships</a></li>
        <li>MSN Critical Care — HCT × UB</li>
      </ol>
    </div>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <div class="container">
      <div class="hero-inner">
        <div class="hero-content">
          <div class="hero-badge">
            <span class="dot"></span>
            International Partnership · Now Accepting Interest
          </div>
          <h1>
            Master of Science<br/>in Nursing:<br/>
            <em>Critical Care for<br/>Elderly Patients</em>
          </h1>
          <p class="hero-subtitle">
            A groundbreaking graduate program jointly offered by <strong style="color:#fff;">HCT Philippines</strong>
            and the <strong style="color:#fff;">University of Barcelona</strong> — merging Filipino clinical expertise
            with world-class European academic rigor to transform geriatric critical care.
          </p>
          <div class="hero-actions">
            <a href="#interest-form" class="btn btn-primary">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M9 12l2 2 4-4"/><circle cx="12" cy="12" r="10"/></svg>
              Express Your Interest
            </a>
            <a href="#program-overview" class="btn btn-outline">Learn More</a>
          </div>
          <div class="hero-stats">
            <div class="stat">
              <div class="stat-number">2 yrs</div>
              <div class="stat-label">Program Duration</div>
            </div>
            <div class="stat">
              <div class="stat-number">100%</div>
              <div class="stat-label">Internationally Recognized</div>
            </div>
            <div class="stat">
              <div class="stat-number">30</div>
              <div class="stat-label">Slots Available</div>
            </div>
            <div class="stat">
              <div class="stat-number">EU + PH</div>
              <div class="stat-label">Dual Accreditation</div>
            </div>
          </div>
        </div>

        <!-- Partner logos card -->
        <div class="partner-card">
          <!-- HCT Logo -->
          <div class="partner-logo-wrap">
            <img
              src="https://www.hct.ph/cdn/shop/files/HCT_Full_Identity_Colored_White_Transparent_a2ccca9d-6e80-4983-8bfc-c705f8a9c6fd.png"
              alt="HCT Philippines"
              onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
              style="filter: none;"
            />
            <div class="hct-logo-fallback" style="display:none;">
              <div class="hct-mark">HCT</div>
              <div class="hct-name">Healthcare &amp;<br/>Technology</div>
            </div>
          </div>

          <div class="divider">PARTNERS WITH</div>

          <!-- UB Logo -->
          <div class="partner-logo-wrap">
            <img
              src="https://web.ub.edu/image/image_gallery?uuid=a8f3a789-0000-0000-0000-000000000001"
              alt="University of Barcelona"
              onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
            />
            <div class="ub-logo-fallback" style="display:flex;">
              <div class="ub-crest">UB</div>
              <div class="ub-name">University<br/>of Barcelona</div>
            </div>
          </div>

          <div style="text-align:center;font-size:.78rem;color:rgba(255,255,255,.45);line-height:1.5;">
            Jointly offering the first<br/>EU–PH graduate nursing degree<br/>in geriatric critical care
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- About the Partnership -->
  <section class="section">
    <div class="container">
      <div class="about-grid">
        <div class="about-visual">
          <div class="about-visual-main">
            <div class="program-pill">
              <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="#008FA0" stroke-width="2.5"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
              Graduate Program · Level 7 EQF
            </div>
            <div style="display:flex;flex-direction:column;gap:12px;">
              <div style="background:var(--white);border-radius:10px;padding:16px 20px;">
                <div style="font-size:.72rem;color:var(--gray-400);font-weight:600;text-transform:uppercase;letter-spacing:.08em;margin-bottom:4px;">Program</div>
                <div style="font-size:.95rem;font-weight:700;color:var(--navy);">MSN — Critical Care for Elderly Patients</div>
              </div>
              <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;">
                <div style="background:var(--white);border-radius:10px;padding:14px 16px;">
                  <div style="font-size:.72rem;color:var(--gray-400);font-weight:600;text-transform:uppercase;letter-spacing:.08em;margin-bottom:4px;">Format</div>
                  <div style="font-size:.88rem;font-weight:700;color:var(--navy);">Blended Online + Residency</div>
                </div>
                <div style="background:var(--white);border-radius:10px;padding:14px 16px;">
                  <div style="font-size:.72rem;color:var(--gray-400);font-weight:600;text-transform:uppercase;letter-spacing:.08em;margin-bottom:4px;">Language</div>
                  <div style="font-size:.88rem;font-weight:700;color:var(--navy);">English / Spanish</div>
                </div>
              </div>
              <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;">
                <div style="background:var(--white);border-radius:10px;padding:14px 16px;">
                  <div style="font-size:.72rem;color:var(--gray-400);font-weight:600;text-transform:uppercase;letter-spacing:.08em;margin-bottom:4px;">Credits</div>
                  <div style="font-size:.88rem;font-weight:700;color:var(--navy);">60 ECTS</div>
                </div>
                <div style="background:var(--white);border-radius:10px;padding:14px 16px;">
                  <div style="font-size:.72rem;color:var(--gray-400);font-weight:600;text-transform:uppercase;letter-spacing:.08em;margin-bottom:4px;">Start Date</div>
                  <div style="font-size:.88rem;font-weight:700;color:var(--navy);">September 2025</div>
                </div>
              </div>
            </div>
          </div>
          <div class="floating-card card-1">
            <div class="fc-icon red">🏛️</div>
            <div class="fc-text">
              <div class="fc-label">Established 1450</div>
              <div class="fc-value">University of Barcelona</div>
            </div>
          </div>
          <div class="floating-card card-2">
            <div class="fc-icon teal">🏥</div>
            <div class="fc-text">
              <div class="fc-label">Philippine Leader in</div>
              <div class="fc-value">Nursing Simulation Ed.</div>
            </div>
          </div>
        </div>

        <div>
          <span class="section-label">About This Partnership</span>
          <h2 class="section-title">Where Filipino Heart Meets European Excellence</h2>
          <p class="section-intro">
            This historic collaboration bridges HCT's innovative simulation-based nursing education
            with the University of Barcelona's 575-year legacy of academic excellence — creating
            a program purpose-built for the growing global challenge of caring for critically ill elderly patients.
          </p>
          <div class="info-list" style="margin-top:28px;">
            <div class="info-item">
              <div class="info-icon">🌍</div>
              <div>
                <div class="info-title">Globally Recognized Credential</div>
                <div class="info-desc">Graduates receive an MSN degree accredited by both PRC (Philippines) and AQU Catalunya (Europe), opening doors to careers on every continent.</div>
              </div>
            </div>
            <div class="info-item">
              <div class="info-icon">🧪</div>
              <div>
                <div class="info-title">Simulation-First Learning</div>
                <div class="info-desc">HCT's VR and simulation labs deliver hands-on critical care training — allowing you to practice in high-fidelity environments before touching a real patient.</div>
              </div>
            </div>
            <div class="info-item">
              <div class="info-icon">👴</div>
              <div>
                <div class="info-title">Specialized in Geriatric Critical Care</div>
                <div class="info-desc">Designed around the fastest-growing patient demographic worldwide. Master the clinical and ethical complexity of elderly care in ICU, CCU, and step-down settings.</div>
              </div>
            </div>
            <div class="info-item">
              <div class="info-icon">✈️</div>
              <div>
                <div class="info-title">Barcelona Immersion Week</div>
                <div class="info-desc">One intensive residency week at UB's Faculty of Medicine and Health Sciences — clinical rounds, research labs, and cultural exchange included.</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Partner Logos Showcase -->
  <section class="section section-teal" style="padding:48px 0;">
    <div class="container">
      <div style="text-align:center;margin-bottom:8px;">
        <span class="section-label">In Partnership With</span>
      </div>
      <div class="partners-showcase">
        <!-- HCT -->
        <div class="partner-info">
          <div class="partner-logo-box">
            <img
              src="https://www.hct.ph/cdn/shop/files/HCT_Full_Identity_Colored_White_Transparent_a2ccca9d-6e80-4983-8bfc-c705f8a9c6fd.png"
              alt="HCT Philippines"
              style="filter: invert(1) sepia(1) saturate(3) hue-rotate(170deg);"
              onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
            />
            <div style="display:none;align-items:center;gap:10px;">
              <div style="background:var(--teal);color:white;font-weight:800;padding:10px 14px;border-radius:8px;font-size:1.2rem;">HCT</div>
              <div style="font-weight:700;color:var(--navy);font-size:1rem;line-height:1.3;">Healthcare &amp;<br/>Technology</div>
            </div>
          </div>
          <p class="partner-desc">
            HCT Philippines leads simulation-based nursing education in Southeast Asia,
            combining AHA-certified programs with cutting-edge VR technology.
          </p>
          <div class="partner-detail"><strong>Location:</strong> Philippines &nbsp;|&nbsp; <strong>Focus:</strong> Healthcare Education & Technology</div>
        </div>

        <!-- X Connector -->
        <div class="x-connector">
          <div class="x-ring">×</div>
          <div class="x-label">Partnership</div>
        </div>

        <!-- UB -->
        <div class="partner-info">
          <div class="partner-logo-box">
            <img
              src="https://web.ub.edu/documents/2197285/0/logo-UB.png"
              alt="University of Barcelona"
              onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';"
            />
            <div style="display:flex;align-items:center;gap:12px;">
              <div style="background:var(--ub-red);color:white;font-weight:800;padding:10px 14px;border-radius:8px;font-size:1.2rem;font-family:'Playfair Display',serif;">UB</div>
              <div style="font-weight:700;color:var(--navy);font-size:1rem;line-height:1.3;">University<br/>of Barcelona</div>
            </div>
          </div>
          <p class="partner-desc">
            Founded in 1450, UB is Spain's leading research university and ranks among
            Europe's top institutions in Health Sciences and Clinical Nursing Research.
          </p>
          <div class="partner-detail"><strong>Location:</strong> Barcelona, Spain &nbsp;|&nbsp; <strong>Focus:</strong> Research, Health Sciences, Nursing</div>
        </div>
      </div>
    </div>
  </section>

  <!-- Program Overview / Curriculum -->
  <section class="section section-alt" id="program-overview">
    <div class="container">
      <div style="text-align:center;">
        <span class="section-label">Program Structure</span>
        <h2 class="section-title" style="text-align:center;">A Rigorous, Clinically-Focused Curriculum</h2>
        <p class="section-intro" style="margin: 16px auto 0;text-align:center;">
          60 ECTS over 4 semesters — blending evidence-based nursing science, hands-on simulation,
          and specialized geriatric clinical practice.
        </p>
      </div>
      <div class="curriculum-grid">
        <div class="curriculum-card">
          <div class="curriculum-card-header">
            <div class="phase-badge">Year 1 · Semester 1</div>
            <h3>Foundations of Geriatric Critical Care</h3>
          </div>
          <div class="curriculum-card-body">
            <ul class="module-list">
              <li>Advanced Gerontological Nursing Science</li>
              <li>Pathophysiology of Aging &amp; Chronic Disease</li>
              <li>Critical Care Pharmacology for Elderly Populations</li>
              <li>Evidence-Based Practice &amp; Nursing Research Methods</li>
              <li>Simulation Lab I: Assessment Skills in the Aging Patient</li>
            </ul>
          </div>
        </div>
        <div class="curriculum-card">
          <div class="curriculum-card-header">
            <div class="phase-badge">Year 1 · Semester 2</div>
            <h3>Advanced Critical Care Practice</h3>
          </div>
          <div class="curriculum-card-body">
            <ul class="module-list">
              <li>ICU &amp; CCU Management: Elderly-Specific Protocols</li>
              <li>Mechanical Ventilation &amp; Respiratory Failure</li>
              <li>Hemodynamic Monitoring &amp; Cardiovascular Emergencies</li>
              <li>Neurological Emergencies in Older Adults</li>
              <li>Simulation Lab II: High-Fidelity ICU Scenarios (VR)</li>
            </ul>
          </div>
        </div>
        <div class="curriculum-card">
          <div class="curriculum-card-header">
            <div class="phase-badge">Year 2 · Semester 3</div>
            <h3>Ethics, Leadership &amp; Systems</h3>
          </div>
          <div class="curriculum-card-body">
            <ul class="module-list">
              <li>Palliative Care Integration in Critical Settings</li>
              <li>Ethics of End-of-Life Decision Making</li>
              <li>Nursing Leadership &amp; Healthcare Quality Systems</li>
              <li>Interprofessional Collaboration in Geriatric Teams</li>
              <li>Barcelona Immersion Residency Week (UB Campus)</li>
            </ul>
          </div>
        </div>
        <div class="curriculum-card">
          <div class="curriculum-card-header">
            <div class="phase-badge">Year 2 · Semester 4</div>
            <h3>Research &amp; Capstone</h3>
          </div>
          <div class="curriculum-card-body">
            <ul class="module-list">
              <li>Clinical Practicum (300 hours in accredited hospitals)</li>
              <li>Research Design &amp; Data Analysis in Nursing</li>
              <li>Global Perspectives on Geriatric Healthcare Systems</li>
              <li>Master's Thesis / Applied Research Project</li>
              <li>Professional Portfolio &amp; Board Examination Prep</li>
            </ul>
          </div>
        </div>
        <div class="curriculum-card" style="grid-column: span 2; background: linear-gradient(135deg, var(--teal-light), #fff);">
          <div class="curriculum-card-header" style="border-bottom-color: var(--teal-mid);">
            <div class="phase-badge" style="background:var(--teal);color:white;">Throughout the Program</div>
            <h3>Cross-Cutting Threads in Every Semester</h3>
          </div>
          <div class="curriculum-card-body" style="display:grid;grid-template-columns:1fr 1fr;gap:0 24px;">
            <ul class="module-list">
              <li>Digital Health &amp; Technology in Critical Care</li>
              <li>Cultural Competence in Elderly Nursing Care</li>
              <li>Spanish Language Modules (A1–A2 Track)</li>
            </ul>
            <ul class="module-list">
              <li>Continuing Professional Development (PRC-CPD Credits)</li>
              <li>Mentorship by UB &amp; HCT Faculty Clinicians</li>
              <li>International Nursing Licensure Preparation</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Why This Program -->
  <section class="section section-dark">
    <div class="container">
      <div style="text-align:center;">
        <span class="section-label light">Why Choose This Program</span>
        <h2 class="section-title light" style="text-align:center;">Built for the Future of Nursing</h2>
        <p class="section-intro light" style="margin:16px auto 0;text-align:center;">
          The global elderly population will double by 2050. Nurses who specialize in
          geriatric critical care will be among the most sought-after clinicians on earth.
        </p>
      </div>
      <div class="why-grid">
        <div class="why-card">
          <div class="why-icon">🎓</div>
          <h3>Dual International Degree</h3>
          <p>Graduate with an MSN recognized by both Philippine Regulatory Commission and the Spanish Agència per a la Qualitat del Sistema Universitari de Catalunya (AQU) — credentials that open doors globally.</p>
        </div>
        <div class="why-card">
          <div class="why-icon">🖥️</div>
          <h3>HCT's Virtual Reality Simulation</h3>
          <p>Learn using the same cutting-edge VR simulation technology used by world-class nursing programs — practice critical care interventions in photo-realistic ICU environments without patient risk.</p>
        </div>
        <div class="why-card">
          <div class="why-icon">🌐</div>
          <h3>Global Career Mobility</h3>
          <p>Your combined EU + PH credential gives you a competitive edge for positions in Europe, the Middle East, North America, and across Asia-Pacific — wherever Filipino nurses are in demand.</p>
        </div>
        <div class="why-card">
          <div class="why-icon">🤝</div>
          <h3>Expert Filipino & European Faculty</h3>
          <p>Learn from HCT's experienced Philippine clinical instructors alongside UB's world-ranked researchers — a faculty team uniquely positioned to train the next generation of geriatric ICU specialists.</p>
        </div>
        <div class="why-card">
          <div class="why-icon">🏥</div>
          <h3>Hospital Practicum Network</h3>
          <p>300+ hours of supervised clinical practice in HCT's partner hospitals across the Philippines, with elective placements available in Barcelona through UB's clinical network.</p>
        </div>
        <div class="why-card">
          <div class="why-icon">💡</div>
          <h3>Flexible Blended Format</h3>
          <p>Online coursework allows working nurses to continue practicing while studying. Synchronous and asynchronous sessions are designed around the schedules of busy healthcare professionals.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Eligibility & Requirements -->
  <section class="section">
    <div class="container">
      <span class="section-label">Admission Requirements</span>
      <h2 class="section-title">Who Should Apply</h2>
      <p class="section-intro">This program is designed for registered nurses ready to advance their careers in critical care. Below are the standard admission requirements.</p>
      <div class="req-grid">
        <div class="req-block">
          <h3><span class="req-num">1</span> Academic Qualifications</h3>
          <ul class="req-list">
            <li><span class="check">✓</span> Bachelor of Science in Nursing (BSN) from an accredited institution</li>
            <li><span class="check">✓</span> Minimum GPA of 2.0 (Philippine system) or equivalent</li>
            <li><span class="check">✓</span> Official transcripts and diploma in English or with certified translation</li>
            <li><span class="check">✓</span> Two academic or professional letters of recommendation</li>
          </ul>
        </div>
        <div class="req-block">
          <h3><span class="req-num">2</span> Professional Qualifications</h3>
          <ul class="req-list">
            <li><span class="check">✓</span> Active PRC Nursing License (or equivalent license from your country)</li>
            <li><span class="check">✓</span> Minimum 1 year of post-licensure clinical nursing experience</li>
            <li><span class="check">✓</span> Current or recent experience in critical care, ICU, CCU, or ER is preferred</li>
            <li><span class="check">✓</span> Current AHA BLS/ACLS certification (or willingness to obtain before intake)</li>
          </ul>
        </div>
        <div class="req-block">
          <h3><span class="req-num">3</span> Language Requirements</h3>
          <ul class="req-list">
            <li><span class="check">✓</span> English proficiency: IELTS 6.0 / TOEFL iBT 79 or equivalent</li>
            <li><span class="check">✓</span> Spanish language modules are included in the curriculum (no prior knowledge required)</li>
            <li><span class="check">✓</span> Filipino graduates who completed BSN in English may be exempt from English proficiency test</li>
          </ul>
        </div>
        <div class="req-block">
          <h3><span class="req-num">4</span> Application Documents</h3>
          <ul class="req-list">
            <li><span class="check">✓</span> Completed interest survey &amp; application form</li>
            <li><span class="check">✓</span> Statement of Purpose (500–800 words)</li>
            <li><span class="check">✓</span> Updated curriculum vitae / resume</li>
            <li><span class="check">✓</span> Photocopy of valid government-issued ID and nursing license</li>
            <li><span class="check">✓</span> 2×2 photo (recent, professional attire)</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Application Timeline -->
  <section class="section section-alt">
    <div class="container">
      <div style="text-align:center;">
        <span class="section-label">Key Dates</span>
        <h2 class="section-title" style="text-align:center;">Application Timeline</h2>
      </div>
      <div class="timeline">
        <div class="timeline-step active">
          <div class="tl-dot">📋</div>
          <div>
            <div class="tl-title">Interest Survey Opens</div>
            <div class="tl-date">Now — Jun 30, 2025</div>
            <div class="tl-desc">Fill out the interest survey below to receive the full prospectus</div>
          </div>
        </div>
        <div class="timeline-step">
          <div class="tl-dot">📝</div>
          <div>
            <div class="tl-title">Applications Open</div>
            <div class="tl-date">July 1, 2025</div>
            <div class="tl-desc">Formal applications accepted; shortlisted candidates notified</div>
          </div>
        </div>
        <div class="timeline-step">
          <div class="tl-dot">🎤</div>
          <div>
            <div class="tl-title">Interviews &amp; Assessment</div>
            <div class="tl-date">July 15–31, 2025</div>
            <div class="tl-desc">Shortlisted candidates invited for online interview with faculty panel</div>
          </div>
        </div>
        <div class="timeline-step">
          <div class="tl-dot">📬</div>
          <div>
            <div class="tl-title">Admission Decisions</div>
            <div class="tl-date">August 15, 2025</div>
            <div class="tl-desc">Offer letters and enrollment instructions issued to accepted students</div>
          </div>
        </div>
        <div class="timeline-step">
          <div class="tl-dot">🎓</div>
          <div>
            <div class="tl-title">Program Begins</div>
            <div class="tl-date">September 2025</div>
            <div class="tl-desc">Orientation week and first semester commence</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Interest Survey & Form -->
  <section class="section survey-section" id="interest-form">
    <div class="container">
      <div class="survey-inner">
        <div class="survey-info">
          <span class="section-label light">Take the First Step</span>
          <h2>Tell Us You're Interested</h2>
          <p>
            Fill out the short survey below — it takes less than 3 minutes.
            We'll send you the full program prospectus, scholarship information,
            and notify you the moment applications open.
          </p>
          <p>No commitment required. Just your curiosity.</p>
          <div class="benefit-list">
            <div class="benefit-item">
              <div class="bi-icon">📘</div>
              Receive the full MSN program prospectus by email
            </div>
            <div class="benefit-item">
              <div class="bi-icon">💰</div>
              Be the first to learn about scholarship and financial aid options
            </div>
            <div class="benefit-item">
              <div class="bi-icon">📅</div>
              Get early access when applications open in July 2025
            </div>
            <div class="benefit-item">
              <div class="bi-icon">🎙️</div>
              Invitation to our exclusive online information webinar (free)
            </div>
            <div class="benefit-item">
              <div class="bi-icon">🔔</div>
              Priority notification for any upcoming intake or open events
            </div>
          </div>
        </div>

        <!-- FORM -->
        <div class="form-card" id="form-container">
          <h3>Interest Survey</h3>
          <p class="form-sub">MSN in Critical Care for Elderly Patients — HCT × University of Barcelona</p>

          <form id="survey-form" novalidate>

            <div class="form-row">
              <div class="form-group">
                <label>First Name <span class="req">*</span></label>
                <input type="text" class="form-control" name="first_name" placeholder="e.g. Maria" required />
              </div>
              <div class="form-group">
                <label>Last Name <span class="req">*</span></label>
                <input type="text" class="form-control" name="last_name" placeholder="e.g. Santos" required />
              </div>
            </div>

            <div class="form-group">
              <label>Email Address <span class="req">*</span></label>
              <input type="email" class="form-control" name="email" placeholder="you@email.com" required />
            </div>

            <div class="form-row">
              <div class="form-group">
                <label>Mobile / WhatsApp Number</label>
                <input type="tel" class="form-control" name="phone" placeholder="+63 9XX XXX XXXX" />
              </div>
              <div class="form-group">
                <label>Country of Residence <span class="req">*</span></label>
                <select class="form-control" name="country" required>
                  <option value="">Select country…</option>
                  <option value="PH">Philippines</option>
                  <option value="SA">Saudi Arabia</option>
                  <option value="AE">United Arab Emirates</option>
                  <option value="QA">Qatar</option>
                  <option value="KW">Kuwait</option>
                  <option value="UK">United Kingdom</option>
                  <option value="US">United States</option>
                  <option value="AU">Australia</option>
                  <option value="ES">Spain</option>
                  <option value="SG">Singapore</option>
                  <option value="OTHER">Other</option>
                </select>
              </div>
            </div>

            <div class="form-group">
              <label>Years of Nursing Experience <span class="req">*</span></label>
              <select class="form-control" name="experience" required>
                <option value="">Select range…</option>
                <option value="0-1">Less than 1 year</option>
                <option value="1-3">1–3 years</option>
                <option value="3-5">3–5 years</option>
                <option value="5-10">5–10 years</option>
                <option value="10+">10+ years</option>
              </select>
            </div>

            <div class="form-group">
              <label>Current Area of Practice</label>
              <select class="form-control" name="specialty">
                <option value="">Select specialty…</option>
                <option>Critical Care / ICU</option>
                <option>Emergency / Trauma</option>
                <option>Medical-Surgical</option>
                <option>Geriatrics / Long-term Care</option>
                <option>Pediatrics</option>
                <option>Operating Room</option>
                <option>Community / Public Health</option>
                <option>Nursing Education / Academia</option>
                <option>Other</option>
              </select>
            </div>

            <div class="form-group">
              <label>What motivates you most to pursue this program? <span class="req">*</span></label>
              <div class="radio-group">
                <label class="radio-item">
                  <input type="radio" name="motivation" value="career" required />
                  Advance my career and earning potential
                </label>
                <label class="radio-item">
                  <input type="radio" name="motivation" value="specialization" />
                  Specialize in geriatric &amp; critical care nursing
                </label>
                <label class="radio-item">
                  <input type="radio" name="motivation" value="international" />
                  Work abroad with an internationally recognized degree
                </label>
                <label class="radio-item">
                  <input type="radio" name="motivation" value="research" />
                  Pursue research and academic nursing roles
                </label>
              </div>
            </div>

            <div class="form-group">
              <label>When would you ideally like to start?</label>
              <select class="form-control" name="start_preference">
                <option value="">Select timeframe…</option>
                <option value="sept2025">September 2025 (First Intake)</option>
                <option value="2026">2026 Intake</option>
                <option value="unsure">Not sure yet, just exploring</option>
              </select>
            </div>

            <div class="form-group">
              <label>How did you hear about this program?</label>
              <select class="form-control" name="referral">
                <option value="">Select source…</option>
                <option>HCT Website</option>
                <option>Facebook / Social Media</option>
                <option>Colleague or Friend</option>
                <option>Email Newsletter</option>
                <option>LinkedIn</option>
                <option>Online Search (Google, etc.)</option>
                <option>HCT Event or Webinar</option>
                <option>Other</option>
              </select>
            </div>

            <div class="form-group">
              <div class="checkbox-group">
                <label class="checkbox-item">
                  <input type="checkbox" name="consent_email" required />
                  I agree to receive program information and updates from HCT Philippines by email. <span class="req">*</span>
                </label>
                <label class="checkbox-item">
                  <input type="checkbox" name="consent_privacy" required />
                  I have read and accept the <a href="#" style="color:var(--teal-dark);text-decoration:underline;">Privacy Policy</a>. My data will be used only to process my interest in this program. <span class="req">*</span>
                </label>
              </div>
            </div>

            <button type="submit" class="submit-btn">
              Submit My Interest &rarr;
            </button>

            <p class="form-footer">
              Your information is secure and will never be shared with third parties.<br/>
              Questions? Email <a href="mailto:partnerships@hct.ph">partnerships@hct.ph</a>
            </p>
          </form>

          <!-- Success State (hidden by default) -->
          <div class="success-overlay" id="success-overlay">
            <div class="check-circle">✅</div>
            <h3>Thank You!</h3>
            <p>
              We've received your interest. Watch your inbox for the full MSN prospectus
              and details about our upcoming information webinar.<br/><br/>
              <strong>Questions?</strong> Email us at
              <a href="mailto:partnerships@hct.ph" style="color:var(--teal-dark);">partnerships@hct.ph</a>
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- FAQ -->
  <section class="section">
    <div class="container">
      <span class="section-label">Frequently Asked Questions</span>
      <h2 class="section-title">Got Questions? We Have Answers.</h2>
      <div class="faq-list">

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false">
            Is this a fully online program?
            <span class="arrow">▾</span>
          </button>
          <div class="faq-a">
            <div class="faq-a-inner">
              The program is primarily delivered online in a blended format — allowing you to study from anywhere. Coursework is done through our e-learning platform, with live synchronous sessions each week. There is one required on-campus residency week in Barcelona at the University of Barcelona campus in Year 2, Semester 3. Simulation lab components are conducted at HCT's facility in the Philippines or through VR headsets for overseas students.
            </div>
          </div>
        </div>

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false">
            Will this degree be recognized in the Philippines and abroad?
            <span class="arrow">▾</span>
          </button>
          <div class="faq-a">
            <div class="faq-a-inner">
              Yes. The MSN is jointly awarded by HCT (Philippines, pending CHED recognition) and the University of Barcelona (accredited by AQU Catalunya, recognized throughout the European Higher Education Area). Graduates will have credentials recognized across Asia, Europe, the Middle East, and internationally — making this ideal for nurses who plan to work globally.
            </div>
          </div>
        </div>

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false">
            Do I need prior experience in geriatrics or critical care?
            <span class="arrow">▾</span>
          </button>
          <div class="faq-a">
            <div class="faq-a-inner">
              Not at all. While experience in critical care or geriatrics is an advantage, the curriculum is designed to build these competencies from the ground up alongside advanced concepts. Many admitted students come from medical-surgical, emergency, or general nursing backgrounds. What matters most is your commitment to excellence and passion for serving elderly patients.
            </div>
          </div>
        </div>

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false">
            Are there scholarships or financial assistance available?
            <span class="arrow">▾</span>
          </button>
          <div class="faq-a">
            <div class="faq-a-inner">
              Yes. HCT and UB are jointly developing a scholarship fund for the first cohort, with merit-based grants and installment payment plans available. Details will be shared with all registered interest applicants before formal applications open. Submitting your interest survey now ensures you are the first to receive scholarship announcements.
            </div>
          </div>
        </div>

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false">
            Can I work full-time while enrolled?
            <span class="arrow">▾</span>
          </button>
          <div class="faq-a">
            <div class="faq-a-inner">
              Yes. The program is specifically designed for working nurses. Online sessions are scheduled to accommodate different time zones and shift patterns. Coursework is a mix of synchronous (live video) and asynchronous (self-paced) learning. We recommend approximately 15–20 hours per week of study time, which most working nurses find manageable alongside full-time employment.
            </div>
          </div>
        </div>

        <div class="faq-item">
          <button class="faq-q" aria-expanded="false">
            What happens after I submit the interest survey?
            <span class="arrow">▾</span>
          </button>
          <div class="faq-a">
            <div class="faq-a-inner">
              Within 48 hours, you will receive the full program prospectus by email, including detailed curriculum, faculty bios, tuition fees, and financial aid information. You'll also receive an invitation to our free online information webinar hosted by HCT and UB faculty. Formal applications open July 1, 2025 — survey respondents receive early access before the public announcement.
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="site-footer">
    <div class="container">
      <div class="footer-inner">
        <div class="footer-brand">
          <div class="footer-logo">
            <img
              src="https://www.hct.ph/cdn/shop/files/HCT_white_logo.png?v=1708760124"
              alt="HCT Philippines"
              onerror="this.style.display='none';this.nextElementSibling.style.display='flex';"
            />
            <div class="logo-fallback-footer" style="display:none;">
              <div class="fmk">HCT</div>
              <div class="ftx">Healthcare &amp; Technology</div>
            </div>
          </div>
          <p>
            HCT Philippines is a leader in healthcare and nursing education,
            combining AHA-accredited programs with advanced simulation technology.
            This International Partnerships page is part of HCT's commitment to
            bringing world-class graduate education to Filipino nurses.
          </p>
          <div style="margin-top:14px;display:flex;gap:12px;">
            <a href="#" style="color:rgba(255,255,255,.4);font-size:.8rem;transition:color .15s;" onmouseover="this.style.color='#00B4C8'" onmouseout="this.style.color='rgba(255,255,255,.4)'">Facebook</a>
            <a href="#" style="color:rgba(255,255,255,.4);font-size:.8rem;transition:color .15s;" onmouseover="this.style.color='#00B4C8'" onmouseout="this.style.color='rgba(255,255,255,.4)'">Instagram</a>
            <a href="#" style="color:rgba(255,255,255,.4);font-size:.8rem;transition:color .15s;" onmouseover="this.style.color='#00B4C8'" onmouseout="this.style.color='rgba(255,255,255,.4)'">LinkedIn</a>
            <a href="#" style="color:rgba(255,255,255,.4);font-size:.8rem;transition:color .15s;" onmouseover="this.style.color='#00B4C8'" onmouseout="this.style.color='rgba(255,255,255,.4)'">YouTube</a>
          </div>
        </div>
        <div class="footer-col">
          <h4>International Partnerships</h4>
          <ul>
            <li><a href="#">All International Programs</a></li>
            <li><a href="#" style="color:var(--teal);">MSN Critical Care — UB Partnership</a></li>
            <li><a href="#">Partner Universities</a></li>
            <li><a href="#">Global Alumni Network</a></li>
            <li><a href="#">Study Abroad Opportunities</a></li>
          </ul>
        </div>
        <div class="footer-col">
          <h4>Support</h4>
          <ul>
            <li><a href="#">Contact Admissions</a></li>
            <li><a href="#">Scholarship Information</a></li>
            <li><a href="#">Program FAQs</a></li>
            <li><a href="#">Privacy Policy</a></li>
            <li><a href="mailto:partnerships@hct.ph">partnerships@hct.ph</a></li>
          </ul>
        </div>
      </div>
      <div class="footer-bottom">
        <div>© 2025 HCT Philippines — Healthcare and Technology. All rights reserved.</div>
        <div>In partnership with <a href="https://web.ub.edu/en/">University of Barcelona</a></div>
      </div>
    </div>
  </footer>

  <!-- JavaScript -->
  <script>
    // FAQ accordion
    document.querySelectorAll('.faq-q').forEach(btn => {
      btn.addEventListener('click', () => {
        const expanded = btn.getAttribute('aria-expanded') === 'true';
        document.querySelectorAll('.faq-q').forEach(b => {
          b.setAttribute('aria-expanded', 'false');
          b.nextElementSibling.classList.remove('open');
        });
        if (!expanded) {
          btn.setAttribute('aria-expanded', 'true');
          btn.nextElementSibling.classList.add('open');
        }
      });
    });

    // Form submission
    document.getElementById('survey-form').addEventListener('submit', function(e) {
      e.preventDefault();

      const required = this.querySelectorAll('[required]');
      let valid = true;
      required.forEach(field => {
        field.style.borderColor = '';
        if (field.type === 'radio') {
          const name = field.name;
          const checked = this.querySelector(`[name="${name}"]:checked`);
          if (!checked) {
            valid = false;
            this.querySelectorAll(`[name="${name}"]`).forEach(r => {
              r.closest('.radio-item').style.borderColor = '#C1272D';
            });
          }
        } else if (field.type === 'checkbox') {
          if (!field.checked) {
            valid = false;
            field.style.outline = '2px solid #C1272D';
          }
        } else if (!field.value.trim()) {
          valid = false;
          field.style.borderColor = '#C1272D';
          field.addEventListener('input', () => field.style.borderColor = '', { once: true });
        }
      });

      if (!valid) {
        const firstError = this.querySelector('[style*="C1272D"]');
        if (firstError) firstError.scrollIntoView({ behavior: 'smooth', block: 'center' });
        return;
      }

      // Show success
      this.style.display = 'none';
      const overlay = document.getElementById('success-overlay');
      overlay.style.display = 'flex';
    });

    // Smooth scroll for anchor links
    document.querySelectorAll('a[href^="#"]').forEach(a => {
      a.addEventListener('click', e => {
        const target = document.querySelector(a.getAttribute('href'));
        if (target) { e.preventDefault(); target.scrollIntoView({ behavior: 'smooth', block: 'start' }); }
      });
    });
  </script>
</body>
</html>
