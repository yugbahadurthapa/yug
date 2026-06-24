<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta
    name="description"
    content="Local Business India helps Indian local businesses grow with websites, AI tools, and digital systems that drive real results."
  />
  <meta name="theme-color" content="#0f172a" />
  <title>Local Business India | Websites, AI, and Digital Growth for Local Businesses</title>

  <style>
    :root {
      --bg: #f8fafc;
      --surface: #ffffff;
      --surface-muted: #f1f5f9;
      --text: #0f172a;
      --text-soft: #475569;
      --primary: #2563eb;
      --primary-dark: #1d4ed8;
      --accent: #0f766e;
      --border: #e2e8f0;
      --shadow: 0 10px 30px rgba(15, 23, 42, 0.08);
      --radius-lg: 20px;
      --radius-md: 14px;
      --radius-sm: 10px;
      --max-width: 1180px;
      --nav-height: 76px;
      --transition: 180ms ease;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: linear-gradient(180deg, #f8fafc 0%, #eef4ff 100%);
      color: var(--text);
      line-height: 1.6;
    }

    img {
      max-width: 100%;
      display: block;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    button,
    input,
    textarea {
      font: inherit;
    }

    .container {
      width: min(100% - 2rem, var(--max-width));
      margin: 0 auto;
    }

    .section {
      padding: 88px 0;
    }

    .section-header {
      max-width: 720px;
      margin-bottom: 40px;
    }

    .eyebrow {
      display: inline-block;
      font-size: 0.85rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--primary);
      margin-bottom: 12px;
    }

    .section-header h2 {
      font-size: clamp(2rem, 4vw, 3rem);
      line-height: 1.12;
      margin-bottom: 14px;
    }

    .section-header p {
      color: var(--text-soft);
      font-size: 1.05rem;
    }

    .card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius-md);
      box-shadow: var(--shadow);
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 0.5rem;
      border: none;
      border-radius: 999px;
      padding: 0.95rem 1.35rem;
      font-weight: 700;
      cursor: pointer;
      transition: transform var(--transition), background var(--transition), color var(--transition), box-shadow var(--transition);
    }

    .btn:hover {
      transform: translateY(-1px);
    }

    .btn-primary {
      background: var(--primary);
      color: #ffffff;
      box-shadow: 0 12px 24px rgba(37, 99, 235, 0.22);
    }

    .btn-primary:hover {
      background: var(--primary-dark);
    }

    .btn-secondary {
      background: #ffffff;
      color: var(--text);
      border: 1px solid var(--border);
    }

    .btn-secondary:hover {
      background: var(--surface-muted);
    }

    .chip-row {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
      margin-top: 1.5rem;
    }

    .chip {
      padding: 0.7rem 0.9rem;
      border-radius: 999px;
      background: rgba(255, 255, 255, 0.8);
      border: 1px solid rgba(226, 232, 240, 0.9);
      color: var(--text-soft);
      font-size: 0.95rem;
      backdrop-filter: blur(10px);
    }

    header.site-header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(248, 250, 252, 0.82);
      backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(226, 232, 240, 0.85);
    }

    .nav {
      min-height: var(--nav-height);
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 0.85rem;
      font-weight: 800;
      font-size: 1.05rem;
    }

    .brand-mark {
      width: 42px;
      height: 42px;
      border-radius: 12px;
      display: grid;
      place-items: center;
      background: linear-gradient(135deg, var(--primary), var(--accent));
      color: #ffffff;
      font-weight: 800;
      box-shadow: 0 10px 20px rgba(15, 118, 110, 0.18);
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 1.1rem;
      list-style: none;
    }

    .nav-links a {
      color: var(--text-soft);
      font-weight: 600;
      transition: color var(--transition);
    }

    .nav-links a:hover,
    .nav-links a:focus {
      color: var(--text);
    }

    .menu-toggle {
      display: none;
      background: transparent;
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 0.55rem 0.7rem;
      cursor: pointer;
    }

    .hero {
      padding: 72px 0 48px;
      position: relative;
      overflow: hidden;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.2fr 0.95fr;
      gap: 2rem;
      align-items: center;
    }

    .hero-copy h1 {
      font-size: clamp(2.5rem, 6vw, 4.75rem);
      line-height: 0.98;
      letter-spacing: -0.03em;
      margin-bottom: 18px;
    }

    .hero-copy p {
      font-size: 1.08rem;
      color: var(--text-soft);
      max-width: 640px;
      margin-bottom: 26px;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.9rem;
    }

    .hero-panel {
      padding: 1.1rem;
      background: linear-gradient(180deg, rgba(255,255,255,0.95), rgba(255,255,255,0.88));
      border: 1px solid rgba(226, 232, 240, 0.9);
      border-radius: 24px;
      box-shadow: var(--shadow);
    }

    .dashboard {
      display: grid;
      gap: 1rem;
    }

    .dashboard-top {
      padding: 1.25rem;
      border-radius: 18px;
      background: linear-gradient(135deg, #0f172a, #1e293b);
      color: #ffffff;
    }

    .dashboard-top h3 {
      font-size: 1.1rem;
      margin-bottom: 0.4rem;
    }

    .dashboard-top p {
      color: rgba(255,255,255,0.8);
      font-size: 0.95rem;
      margin-bottom: 1rem;
    }

    .metric-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 0.75rem;
    }

    .metric {
      padding: 0.9rem;
      border-radius: 14px;
      background: rgba(255,255,255,0.08);
      border: 1px solid rgba(255,255,255,0.1);
    }

    .metric strong {
      display: block;
      font-size: 1.15rem;
      margin-bottom: 0.2rem;
    }

    .metric span {
      font-size: 0.85rem;
      color: rgba(255,255,255,0.75);
    }

    .dashboard-bottom {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1rem;
    }

    .mini-card {
      padding: 1.1rem;
      border-radius: 16px;
      background: #ffffff;
      border: 1px solid var(--border);
    }

    .mini-card h4 {
      margin-bottom: 0.45rem;
      font-size: 1rem;
    }

    .mini-card p {
      color: var(--text-soft);
      font-size: 0.94rem;
    }

    .stats-row {
      margin-top: 48px;
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 1rem;
    }

    .stat-card {
      padding: 1.25rem;
      border-radius: 18px;
      background: rgba(255,255,255,0.8);
      border: 1px solid var(--border);
      box-shadow: var(--shadow);
    }

    .stat-card strong {
      display: block;
      font-size: 1.55rem;
      margin-bottom: 0.3rem;
    }

    .stat-card span {
      color: var(--text-soft);
      font-size: 0.95rem;
    }

    .grid-3 {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 1.2rem;
    }

    .grid-2 {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 1.25rem;
    }

    .feature-card,
    .service-card,
    .learn-card,
    .about-card,
    .contact-card {
      padding: 1.5rem;
    }

    .icon-box {
      width: 52px;
      height: 52px;
      border-radius: 14px;
      display: grid;
      place-items: center;
      background: linear-gradient(135deg, rgba(37, 99, 235, 0.14), rgba(15, 118, 110, 0.14));
      color: var(--primary);
      margin-bottom: 1rem;
      font-weight: 800;
    }

    .feature-card h3,
    .service-card h3,
    .learn-card h3,
    .about-card h3,
    .contact-card h3 {
      font-size: 1.15rem;
      margin-bottom: 0.55rem;
    }

    .feature-card p,
    .service-card p,
    .learn-card p,
    .about-card p,
    .contact-card p {
      color: var(--text-soft);
    }

    .learn-layout {
      display: grid;
      grid-template-columns: 1fr 0.92fr;
      gap: 1.5rem;
      align-items: start;
    }

    .learn-list {
      display: grid;
      gap: 1rem;
    }

    .learn-highlight {
      padding: 1.7rem;
      background: linear-gradient(180deg, #ffffff, #f8fbff);
    }

    .learn-highlight ul {
      list-style: none;
      display: grid;
      gap: 0.9rem;
      margin-top: 1rem;
    }

    .learn-highlight li {
      padding: 0.95rem 1rem;
      border-radius: 14px;
      background: var(--surface-muted);
      color: var(--text-soft);
      border: 1px solid var(--border);
    }

    .service-card {
      position: relative;
      overflow: hidden;
    }

    .service-tag {
      display: inline-block;
      margin-bottom: 0.8rem;
      padding: 0.4rem 0.7rem;
      border-radius: 999px;
      background: #eff6ff;
      color: var(--primary-dark);
      font-size: 0.82rem;
      font-weight: 700;
    }

    .use-case {
      margin-top: 1rem;
      padding: 1rem;
      border-radius: 14px;
      background: var(--surface-muted);
      border: 1px solid var(--border);
      font-size: 0.94rem;
      color: var(--text-soft);
    }

    .about-layout {
      display: grid;
      grid-template-columns: 1.05fr 0.95fr;
      gap: 1.5rem;
      align-items: stretch;
    }

    .credibility-list {
      list-style: none;
      display: grid;
      gap: 0.9rem;
      margin-top: 1rem;
    }

    .credibility-list li {
      padding: 0.95rem 1rem;
      border-left: 4px solid var(--primary);
      background: #ffffff;
      border-radius: 12px;
      color: var(--text-soft);
      border-top: 1px solid var(--border);
      border-right: 1px solid var(--border);
      border-bottom: 1px solid var(--border);
    }

    .timeline {
      display: grid;
      gap: 1rem;
    }

    .timeline-step {
      padding: 1.25rem;
      border-radius: 16px;
      border: 1px solid var(--border);
      background: #ffffff;
    }

    .timeline-step strong {
      display: block;
      margin-bottom: 0.4rem;
      font-size: 1rem;
    }

    .timeline-step p {
      color: var(--text-soft);
      font-size: 0.95rem;
    }

    .contact-layout {
      display: grid;
      grid-template-columns: 0.9fr 1.1fr;
      gap: 1.5rem;
    }

    .contact-panel {
      padding: 1.5rem;
      background: linear-gradient(135deg, #0f172a, #1e3a8a);
      color: #ffffff;
      border-radius: 20px;
      box-shadow: var(--shadow);
    }

    .contact-panel p {
      color: rgba(255,255,255,0.8);
    }

    .contact-points {
      list-style: none;
      display: grid;
      gap: 0.9rem;
      margin-top: 1.25rem;
    }

    .contact-points li {
      padding: 0.9rem 1rem;
      border-radius: 14px;
      background: rgba(255,255,255,0.08);
      border: 1px solid rgba(255,255,255,0.1);
    }

    form.contact-form {
      padding: 1.5rem;
    }

    .form-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1rem;
      margin-bottom: 1rem;
    }

    .form-group {
      display: grid;
      gap: 0.45rem;
      margin-bottom: 1rem;
    }

    label {
      font-weight: 600;
      font-size: 0.95rem;
    }

    input,
    textarea {
      width: 100%;
      border: 1px solid var(--border);
      background: #ffffff;
      border-radius: 12px;
      padding: 0.95rem 1rem;
      color: var(--text);
      transition: border-color var(--transition), box-shadow var(--transition);
    }

    input:focus,
    textarea:focus {
      outline: none;
      border-color: var(--primary);
      box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.12);
    }

    textarea {
      min-height: 150px;
      resize: vertical;
    }

    .full-width {
      grid-column: 1 / -1;
    }

    .cta-band {
      padding: 1.6rem;
      border-radius: 24px;
      background: linear-gradient(135deg, rgba(37, 99, 235, 0.08), rgba(15, 118, 110, 0.08));
      border: 1px solid var(--border);
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
      flex-wrap: wrap;
      margin-top: 2rem;
    }

    footer {
      padding: 28px 0 50px;
    }

    .footer-inner {
      display: flex;
      justify-content: space-between;
      gap: 1rem;
      align-items: center;
      flex-wrap: wrap;
      color: var(--text-soft);
      border-top: 1px solid var(--border);
      padding-top: 1.2rem;
    }

    .footer-nav {
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
    }

    .reveal {
      opacity: 0;
      transform: translateY(16px);
      transition: opacity 500ms ease, transform 500ms ease;
    }

    .reveal.visible {
      opacity: 1;
      transform: translateY(0);
    }

    @media (max-width: 1024px) {
      .hero-grid,
      .learn-layout,
      .about-layout,
      .contact-layout {
        grid-template-columns: 1fr;
      }

      .grid-3 {
        grid-template-columns: repeat(2, 1fr);
      }

      .stats-row {
        grid-template-columns: repeat(2, 1fr);
      }
    }

    @media (max-width: 760px) {
      .nav {
        flex-wrap: wrap;
        padding: 0.8rem 0;
      }

      .menu-toggle {
        display: inline-flex;
      }

      .nav-links {
        display: none;
        width: 100%;
        flex-direction: column;
        align-items: flex-start;
        padding: 0.4rem 0 0.9rem;
      }

      .nav-links.open {
        display: flex;
      }

      .hero {
        padding-top: 36px;
      }

      .hero-actions {
        flex-direction: column;
        align-items: stretch;
      }

      .metric-grid,
      .dashboard-bottom,
      .grid-3,
      .grid-2,
      .stats-row,
      .form-grid {
        grid-template-columns: 1fr;
      }

      .section {
        padding: 72px 0;
      }

      .hero-copy h1 {
        font-size: 2.4rem;
      }

      .cta-band {
        align-items: flex-start;
      }
    }
  </style>
</head>
<body>
  <header class="site-header">
    <div class="container nav">
      <a class="brand" href="#home" aria-label="Local Business India home">
        <span class="brand-mark">LBI</span>
        <span>Local Business India</span>
      </a>

      <button class="menu-toggle" id="menuToggle" aria-expanded="false" aria-controls="navLinks" aria-label="Toggle navigation">
        Menu
      </button>

      <ul class="nav-links" id="navLinks">
        <li><a href="#home">Home</a></li>
        <li><a href="#learn">Learn</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
        <li><a class="btn btn-primary" href="#contact">Book a Free Consultation</a></li>
      </ul>
    </div>
  </header>

  <main>
    <!-- Home -->
    <section class="hero" id="home">
      <div class="container">
        <div class="hero-grid">
          <div class="hero-copy reveal">
            <span class="eyebrow">Digital growth for Indian local businesses</span>
            <h1>Grow your local business with a better website, smarter tools, and practical AI.</h1>
            <p>
              Local Business India helps shops, clinics, service providers, restaurants, and growing brands build a stronger digital presence.
              We create modern websites, simplify customer communication, and introduce AI in a way that is useful, affordable, and easy to understand.
            </p>

            <div class="hero-actions">
              <a class="btn btn-primary" href="#contact">Start Your Growth Plan</a>
              <a class="btn btn-secondary" href="#services">Explore Services</a>
            </div>

            <div class="chip-row" aria-label="Key focus areas">
              <span class="chip">Websites that build trust</span>
              <span class="chip">AI that saves time</span>
              <span class="chip">Growth systems for local reach</span>
            </div>
          </div>

          <div class="hero-panel reveal" aria-label="Business growth dashboard preview">
            <div class="dashboard">
              <div class="dashboard-top">
                <h3>Business Growth Snapshot</h3>
                <p>Simple digital systems can improve visibility, response time, and lead quality.</p>
                <div class="metric-grid">
                  <div class="metric">
                    <strong>24/7</strong>
                    <span>Website presence</span>
                  </div>
                  <div class="metric">
                    <strong>3x</strong>
                    <span>Faster responses</span>
                  </div>
                  <div class="metric">
                    <strong>+Local</strong>
                    <span>Better discovery</span>
                  </div>
                </div>
              </div>

              <div class="dashboard-bottom">
                <div class="mini-card">
                  <h4>Website Foundations</h4>
                  <p>Fast, mobile-friendly pages that help customers understand your business and take action.</p>
                </div>
                <div class="mini-card">
                  <h4>AI Assistance</h4>
                  <p>Automate common questions, follow-ups, and content tasks without making things complicated.</p>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="stats-row reveal">
          <div class="stat-card">
            <strong>Fast Launch</strong>
            <span>Clear process from planning to delivery</span>
          </div>
          <div class="stat-card">
            <strong>Local Focus</strong>
            <span>Built for Indian service and retail businesses</span>
          </div>
          <div class="stat-card">
            <strong>Practical AI</strong>
            <span>Useful automation, not hype</span>
          </div>
          <div class="stat-card">
            <strong>Scalable Setup</strong>
            <span>Ready for future tools and features</span>
          </div>
        </div>
      </div>
    </section>

    <!-- Home supporting section -->
    <section class="section">
      <div class="container">
        <div class="section-header reveal">
          <span class="eyebrow">Why businesses choose us</span>
          <h2>Built to solve real business problems, not just create a nice-looking website.</h2>
          <p>
            Many local businesses need more than design. They need clarity, customer trust, and systems that make daily work easier.
            That is where our approach stands out.
          </p>
        </div>

        <div class="grid-3">
          <article class="feature-card card reveal">
            <div class="icon-box">01</div>
            <h3>Clear value proposition</h3>
            <p>
              We help visitors quickly understand what you do, who you serve, and why they should contact you.
            </p>
          </article>

          <article class="feature-card card reveal">
            <div class="icon-box">02</div>
            <h3>Designed for action</h3>
            <p>
              Every page is planned to move users toward a clear next step such as calling, booking, or sending an enquiry.
            </p>
          </article>

          <article class="feature-card card reveal">
            <div class="icon-box">03</div>
            <h3>Ready for growth</h3>
            <p>
              The structure supports future additions like blogs, booking systems, WhatsApp integration, lead forms, and AI assistants.
            </p>
          </article>
        </div>
      </div>
    </section>

    <!-- Learn -->
    <section class="section" id="learn">
      <div class="container">
        <div class="section-header reveal">
          <span class="eyebrow">Learn</span>
          <h2>Simple education for business owners who want to grow with confidence.</h2>
          <p>
            Technology should feel practical, not confusing. Our learning section explains how websites, AI, and digital tools can create real business value.
          </p>
        </div>

        <div class="learn-layout">
          <div class="learn-list">
            <article class="learn-card card reveal">
              <div class="icon-box">AI</div>
              <h3>What AI can actually do for a local business</h3>
              <p>
                AI can help answer common questions, write first drafts of messages, organize leads, and reduce repetitive work.
                It does not replace your business knowledge. It supports it.
              </p>
            </article>

            <article class="learn-card card reveal">
              <div class="icon-box">Web</div>
              <h3>Why a professional website still matters</h3>
              <p>
                Social media helps people discover you, but a website gives credibility, control, and a central place for services, pricing, reviews, and enquiries.
              </p>
            </article>

            <article class="learn-card card reveal">
              <div class="icon-box">Grow</div>
              <h3>How digital growth works in the real world</h3>
              <p>
                Growth usually comes from small improvements done well: better visibility, easier contact, quicker replies, and clear information that builds trust.
              </p>
            </article>
          </div>

          <aside class="learn-highlight card reveal">
            <h3>Beginner-friendly digital roadmap</h3>
            <p style="color: var(--text-soft); margin-top: 0.6rem;">
              For many businesses, the best path is to start simple and improve step by step.
            </p>

            <ul>
              <li><strong>Step 1:</strong> Create a clear website with mobile-friendly pages and strong contact options.</li>
              <li><strong>Step 2:</strong> Improve visibility with local SEO, customer trust signals, and useful content.</li>
              <li><strong>Step 3:</strong> Add AI and automation where they save time or improve service quality.</li>
              <li><strong>Step 4:</strong> Track what works and grow using data, not guesswork.</li>
            </ul>
          </aside>
        </div>

        <div class="cta-band reveal">
          <div>
            <h3 style="margin-bottom: 0.4rem;">Knowledge is part of the service.</h3>
            <p style="color: var(--text-soft);">
              We explain things in plain language so business owners can make confident digital decisions.
            </p>
          </div>
          <a class="btn btn-primary" href="#contact">Talk to Our Team</a>
        </div>
      </div>
    </section>

    <!-- Services -->
    <section class="section" id="services">
      <div class="container">
        <div class="section-header reveal">
          <span class="eyebrow">Services</span>
          <h2>Practical services designed for visibility, trust, and business efficiency.</h2>
          <p>
            We focus on tools and systems that local businesses can actually use. Every service is tied to a real outcome, not just a technical feature.
          </p>
        </div>

        <div class="grid-2">
          <article class="service-card card reveal">
            <span class="service-tag">Website Design and Development</span>
            <h3>Modern business websites that turn visitors into customers</h3>
            <p>
              We build clean, fast, mobile-friendly websites with clear messaging, strong calls to action, and a structure that is easy to expand over time.
            </p>
            <div class="use-case">
              <strong>Use case:</strong> A dental clinic can showcase treatments, doctor profiles, timings, FAQs, and appointment enquiries in one trusted place.
            </div>
          </article>

          <article class="service-card card reveal">
            <span class="service-tag">AI for Daily Operations</span>
            <h3>Smart support tools that reduce repetitive work</h3>
            <p>
              We help businesses use AI for enquiry handling, content drafts, simple customer support flows, and internal process support.
            </p>
            <div class="use-case">
              <strong>Use case:</strong> A coaching center can automate common responses about fees, batches, and admissions while the team focuses on serious leads.
            </div>
          </article>

          <article class="service-card card reveal">
            <span class="service-tag">Digital Growth Systems</span>
            <h3>Stronger online presence with local-first strategy</h3>
            <p>
              We improve how your business appears online through better content structure, local discovery, trust-building pages, and lead-focused design.
            </p>
            <div class="use-case">
              <strong>Use case:</strong> A home services brand can attract better leads by clearly showing service areas, pricing guidance, and customer proof.
            </div>
          </article>

          <article class="service-card card reveal">
            <span class="service-tag">Consulting and Setup</span>
            <h3>Clear digital planning for founders and small teams</h3>
            <p>
              Not every business needs a complex system. We help identify the right starting point and build a roadmap that matches your stage and budget.
            </p>
            <div class="use-case">
              <strong>Use case:</strong> A retail store expanding online can start with a business website first, then add catalog, payments, and automation later.
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- About -->
    <section class="section" id="about">
      <div class="container">
        <div class="section-header reveal">
          <span class="eyebrow">About</span>
          <h2>We believe local businesses deserve high-quality digital infrastructure.</h2>
          <p>
            Local Business India exists to help Indian businesses compete in a digital-first world with better websites, smarter systems, and practical guidance.
          </p>
        </div>

        <div class="about-layout">
          <div class="about-card card reveal">
            <h3>Mission</h3>
            <p>
              To make modern digital tools accessible, useful, and results-focused for local businesses across India.
            </p>

            <h3 style="margin-top: 1.5rem;">Vision</h3>
            <p>
              To become a trusted growth partner for local businesses that want to build credibility, improve operations, and grow sustainably through technology.
            </p>

            <h3 style="margin-top: 1.5rem;">Why we are credible</h3>
            <ul class="credibility-list">
              <li><strong>Business-first thinking:</strong> We start with goals, customer needs, and operational challenges before choosing tools.</li>
              <li><strong>Scalable structure:</strong> Our websites and systems are built so new features can be added without starting over.</li>
              <li><strong>Clear communication:</strong> We explain technical ideas in simple, practical language that business owners can act on.</li>
            </ul>
          </div>

          <div class="timeline reveal">
            <div class="timeline-step card">
              <strong>1. Understand the business</strong>
              <p>We learn what you sell, how customers find you, and where digital friction is slowing growth.</p>
            </div>

            <div class="timeline-step card">
              <strong>2. Build a strong foundation</strong>
              <p>We create the core website and content structure needed for trust, clarity, and lead generation.</p>
            </div>

            <div class="timeline-step card">
              <strong>3. Improve customer experience</strong>
              <p>We simplify how customers contact you, ask questions, and move toward a purchase or booking.</p>
            </div>

            <div class="timeline-step card">
              <strong>4. Add smart growth layers</strong>
              <p>We introduce AI, automation, content systems, and future-ready enhancements when the business is ready.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact -->
    <section class="section" id="contact">
      <div class="container">
        <div class="section-header reveal">
          <span class="eyebrow">Contact</span>
          <h2>Start with a simple conversation about your business goals.</h2>
          <p>
            Whether you need a professional website, digital advice, or a practical AI plan, we can help you identify the best next step.
          </p>
        </div>

        <div class="contact-layout">
          <div class="contact-panel reveal">
            <h3 style="font-size: 1.4rem; margin-bottom: 0.6rem;">Let's build something useful.</h3>
            <p>
              We work best with business owners who want clarity, quality, and long-term digital value.
            </p>

            <ul class="contact-points">
              <li><strong>Email:</strong> hello@localbusinessindia.com</li>
              <li><strong>Phone:</strong> +91 98765 43210</li>
              <li><strong>Focus:</strong> Websites, AI adoption, local digital growth</li>
            </ul>
          </div>

          <form class="contact-form card reveal" onsubmit="handleSubmit(event)">
            <div class="form-grid">
              <div class="form-group">
                <label for="name">Full Name</label>
                <input id="name" name="name" type="text" placeholder="Your name" required />
              </div>

              <div class="form-group">
                <label for="business">Business Name</label>
                <input id="business" name="business" type="text" placeholder="Your business name" required />
              </div>
            </div>

            <div class="form-grid">
              <div class="form-group">
                <label for="email">Email Address</label>
                <input id="email" name="email" type="email" placeholder="you@example.com" required />
              </div>

              <div class="form-group">
                <label for="phone">Phone Number</label>
                <input id="phone" name="phone" type="tel" placeholder="+91" />
              </div>
            </div>

            <div class="form-group">
              <label for="message">What do you need help with?</label>
              <textarea id="message" name="message" placeholder="Tell us about your business, goals, or current challenges." required></textarea>
            </div>

            <button class="btn btn-primary" type="submit">Send Enquiry</button>
            <p id="formMessage" style="margin-top: 1rem; color: var(--text-soft);"></p>
          </form>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container footer-inner">
      <p><strong>Local Business India</strong> - Websites, AI, and digital growth for ambitious local businesses.</p>
      <nav class="footer-nav" aria-label="Footer navigation">
        <a href="#home">Home</a>
        <a href="#learn">Learn</a>
        <a href="#services">Services</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </footer>

  <script>
    const menuToggle = document.getElementById("menuToggle");
    const navLinks = document.getElementById("navLinks");

    menuToggle.addEventListener("click", () => {
      const isOpen = navLinks.classList.toggle("open");
      menuToggle.setAttribute("aria-expanded", String(isOpen));
    });

    document.querySelectorAll('.nav-links a').forEach(link => {
      link.addEventListener('click', () => {
        navLinks.classList.remove('open');
        menuToggle.setAttribute('aria-expanded', 'false');
      });
    });

    function handleSubmit(event) {
      event.preventDefault();
      const formMessage = document.getElementById("formMessage");
      formMessage.textContent = "Thank you. Your enquiry has been captured. This demo form can be connected to email, CRM, or backend services.";
      event.target.reset();
    }

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add("visible");
        }
      });
    }, { threshold: 0.12 });

    document.querySelectorAll(".reveal").forEach(el => observer.observe(el));
  </script>
</body>
</html>

