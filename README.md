
<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;1,400&family=DM+Mono:wght@400;500&family=DM+Sans:wght@300;400;500&display=swap');
  :root {
    --accent: #7B5EA7;
    --accent-light: #EDE9F6;
    --gold: #B08D57;
    --gold-light: #FBF5EA;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  .readme { max-width: 680px; margin: 0 auto; padding: 2rem 1rem 3rem; font-family: 'DM Sans', sans-serif; }

  /* ── HEADER ── */
  .header { margin-bottom: 2rem; }
  .dept-banner {
    display: flex; flex-direction: column;
    align-items: center; text-align: center;
    border: 0.5px solid var(--color-border-tertiary);
    border-radius: 10px;
    padding: 20px 24px 16px;
    margin-bottom: 18px;
    background: var(--color-background-secondary);
  }
  .dept-top {
    font-family: 'DM Mono', monospace;
    font-size: 10px; letter-spacing: 0.2em;
    color: var(--color-text-tertiary);
    text-transform: uppercase;
    margin-bottom: 8px;
  }
  .dept-name {
    font-family: 'Playfair Display', serif;
    font-size: 22px; font-weight: 600;
    color: var(--color-text-primary);
    letter-spacing: 0.01em;
    margin-bottom: 6px;
  }
  .dept-meta {
    font-family: 'DM Mono', monospace;
    font-size: 10px; letter-spacing: 0.12em;
    color: var(--color-text-tertiary);
    text-transform: uppercase;
  }
  .dept-divider {
    width: 40px; height: 1px;
    background: var(--accent);
    margin: 10px auto 10px;
    opacity: 0.5;
  }
  .member-line {
    font-family: 'DM Mono', monospace;
    font-size: 11px; color: var(--color-text-secondary);
  }
  .member-line span {
    color: var(--accent); font-weight: 500;
  }

  /* Name + badges below banner */
  .name-block { margin-bottom: 10px; }
  .big-name {
    font-family: 'Playfair Display', serif;
    font-size: 28px; font-weight: 600;
    color: var(--color-text-primary);
  }
  .badge-row { display: flex; gap: 6px; flex-wrap: wrap; margin-top: 10px; }
  .badge {
    font-family: 'DM Mono', monospace;
    font-size: 10px; padding: 3px 10px;
    border-radius: 2px; border: 0.5px solid;
  }
  .b-purple { background: var(--accent-light); color: var(--accent); border-color: var(--accent); }
  .b-gold   { background: var(--gold-light); color: var(--gold); border-color: var(--gold); }
  .b-gray   { background: var(--color-background-secondary); color: var(--color-text-secondary); border-color: var(--color-border-tertiary); }

  /* ── TAGLINE ── */
  .tagline {
    font-family: 'Playfair Display', serif;
    font-size: 14px; font-style: italic;
    color: var(--color-text-secondary);
    border-left: 2px solid var(--accent);
    padding: 10px 14px; margin-bottom: 2rem;
  }

  /* ── SECTIONS ── */
  .section { margin-bottom: 2.2rem; }
  .section-label {
    font-family: 'DM Mono', monospace;
    font-size: 10px; letter-spacing: 0.15em;
    color: var(--color-text-tertiary);
    text-transform: uppercase; margin-bottom: 12px;
  }

  /* Stats */
  .stats-grid { display: grid; grid-template-columns: repeat(4, minmax(0,1fr)); gap: 8px; }
  .stat-card { background: var(--color-background-secondary); border-radius: 6px; padding: 14px 10px; text-align: center; }
  .stat-val { font-family: 'Playfair Display', serif; font-size: 22px; font-weight: 600; color: var(--color-text-primary); }
  .stat-lbl { font-size: 11px; color: var(--color-text-tertiary); margin-top: 4px; }

  /* About */
  .about-text { font-size: 14px; line-height: 1.8; color: var(--color-text-secondary); }
  .about-text strong { color: var(--color-text-primary); font-weight: 500; }

  /* Pillars */
  .pillars { display: grid; grid-template-columns: repeat(2, minmax(0,1fr)); gap: 8px; }
  .pillar { border: 0.5px solid var(--color-border-tertiary); border-radius: 8px; padding: 14px; }
  .pillar-title { font-size: 13px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 4px; }
  .pillar-desc { font-size: 12px; color: var(--color-text-tertiary); line-height: 1.55; }

  /* Impact cards (no project names) */
  .impact-card { border: 0.5px solid var(--color-border-tertiary); border-radius: 8px; padding: 14px 16px; margin-bottom: 8px; }
  .impact-top { display: flex; justify-content: space-between; align-items: center; margin-bottom: 6px; }
  .impact-type { font-family: 'DM Mono', monospace; font-size: 10px; color: var(--accent); text-transform: uppercase; letter-spacing: 0.1em; }
  .impact-pill { background: #EAF3DE; color: #3B6D11; font-family: 'DM Mono', monospace; font-size: 10px; padding: 2px 8px; border-radius: 20px; }
  .impact-stack { font-family: 'DM Mono', monospace; font-size: 10px; color: var(--color-text-tertiary); margin-bottom: 6px; }
  .impact-desc { font-size: 12px; color: var(--color-text-secondary); line-height: 1.6; }

  /* Skills */
  .skill-section { margin-bottom: 14px; }
  .skill-dept { font-family: 'DM Mono', monospace; font-size: 10px; letter-spacing: 0.1em; color: var(--accent); text-transform: uppercase; margin-bottom: 8px; }
  .skill-chips { display: flex; flex-wrap: wrap; gap: 6px; }
  .chip { font-family: 'DM Mono', monospace; font-size: 11px; padding: 4px 10px; border-radius: 4px; background: var(--color-background-secondary); color: var(--color-text-secondary); border: 0.5px solid var(--color-border-tertiary); }
  .chip.primary { background: var(--accent-light); color: var(--accent); border-color: var(--accent); }

  /* Quest */
  .quest-block { background: var(--color-background-secondary); border-radius: 8px; padding: 14px 16px; border-left: 2px solid var(--accent); }
  .quest-item { display: flex; align-items: flex-start; gap: 10px; font-size: 13px; color: var(--color-text-secondary); margin-bottom: 8px; }
  .quest-item:last-child { margin-bottom: 0; }
  .quest-dot { width: 6px; height: 6px; border-radius: 50%; background: var(--accent); margin-top: 5px; flex-shrink: 0; }

  /* Connect */
  .connect-row { display: flex; gap: 8px; flex-wrap: wrap; }
  .connect-btn { font-family: 'DM Mono', monospace; font-size: 11px; padding: 8px 16px; border-radius: 4px; border: 0.5px solid var(--color-border-tertiary); color: var(--color-text-secondary); cursor: pointer; background: transparent; text-decoration: none; display: inline-block; }
  .connect-btn.primary { background: var(--accent); color: #fff; border-color: var(--accent); }

  /* Closing */
  .closing { text-align: center; margin-top: 2.5rem; padding-top: 1.5rem; border-top: 0.5px solid var(--color-border-tertiary); }
  .closing-quote { font-family: 'Playfair Display', serif; font-size: 13px; font-style: italic; color: var(--color-text-tertiary); }
</style>

<div class="readme">

  <!-- Header Banner -->
  <div class="header">
    <div class="dept-banner">
      <div class="dept-top">Est. 2018 &nbsp;·&nbsp; Jaipur, Rajasthan</div>
      <div class="dept-name">The Tortured Coders Department</div>
      <div class="dept-divider"></div>
      <div class="member-line">Member ID &nbsp;·&nbsp; <span>Trilok Chand Swami</span> &nbsp;·&nbsp; Software Engineer</div>
    </div>

    <div class="name-block">
      <div class="big-name">Trilok Chand Swami</div>
      <div class="badge-row">
        <span class="badge b-purple">Software Engineer</span>
        <span class="badge b-gold">.NET Specialist</span>
        <span class="badge b-gray">AZ-900 in Progress</span>
        <span class="badge b-gray">Open to Opportunities</span>
      </div>
    </div>
  </div>

  <!-- Tagline -->
  <p class="tagline">"Migrating legacy systems is not just engineering — it's archaeology, therapy, and warfare, all at once."</p>

  <!-- Stats -->
  <div class="section">
    <div class="section-label">By the numbers</div>
    <div class="stats-grid">
      <div class="stat-card"><div class="stat-val">2+</div><div class="stat-lbl">Yrs shipped</div></div>
      <div class="stat-card"><div class="stat-val">30+</div><div class="stat-lbl">APIs built</div></div>
      <div class="stat-card"><div class="stat-val">30%</div><div class="stat-lbl">Perf. gains</div></div>
      <div class="stat-card"><div class="stat-val">5K+</div><div class="stat-lbl">Users served</div></div>
    </div>
  </div>

  <!-- About -->
  <div class="section">
    <div class="section-label">Manuscript</div>
    <p class="about-text">
      Software engineer forged in enterprise systems and government platforms.
      I specialise in <strong>backend architecture with .NET Core</strong> — crafting clean APIs,
      optimising SQL for scale, and modernising the legacy codebases that hold industries together.
      By night: cloud blueprints, Docker containers, and the AZ-900 grind.<br><br>
      Clean code is not a luxury. It's a responsibility.
    </p>
  </div>

  <!-- Pillars -->
  <div class="section">
    <div class="section-label">Engineering pillars</div>
    <div class="pillars">
      <div class="pillar">
        <div class="pillar-title">⚡ Performance-first</div>
        <div class="pillar-desc">Query tuning, Dapper ORM, index strategy — if it's slow, I find out why.</div>
      </div>
      <div class="pillar">
        <div class="pillar-title">🏛️ Clean architecture</div>
        <div class="pillar-desc">RESTful design, API versioning, separation of concerns — from day one.</div>
      </div>
      <div class="pillar">
        <div class="pillar-title">🔒 Security mindset</div>
        <div class="pillar-desc">OAuth 2.0, vulnerability patching, secure third-party integrations.</div>
      </div>
      <div class="pillar">
        <div class="pillar-title">☁️ Cloud-ready</div>
        <div class="pillar-desc">Azure, Docker, CI/CD — building for production, not just localhost.</div>
      </div>
    </div>
  </div>

  <!-- Impact (no project names) -->
  <div class="section">
    <div class="section-label">Impact delivered</div>

    <div class="impact-card">
      <div class="impact-top">
        <span class="impact-type">Government Portal · Workflow Automation</span>
        <span class="impact-pill">−60% processing time</span>
      </div>
      <div class="impact-stack">.NET Core MVC · SQL Server · Angular · Role-Based Workflows</div>
      <div class="impact-desc">Transformed a non-functional static system into a dynamic, data-driven platform. Built role-based multi-level approval workflows and reduced end-to-end processing time by 60%.</div>
    </div>

    <div class="impact-card">
      <div class="impact-top">
        <span class="impact-type">State-Wide Data Platform · 5,000+ Entities</span>
        <span class="impact-pill">−70% manual paperwork</span>
      </div>
      <div class="impact-stack">.NET Core · Angular · SQL Server · RESTful APIs</div>
      <div class="impact-desc">Engineered APIs and database architecture for a large-scale state government system. Reduced manual paperwork by 70% and improved API response times by 30%.</div>
    </div>

    <div class="impact-card">
      <div class="impact-top">
        <span class="impact-type">HR Platform · Legacy Modernisation</span>
        <span class="impact-pill">+30% performance</span>
      </div>
      <div class="impact-stack">ASP.NET WebForms → .NET Core · FCM · HubSpot · Dapper ORM</div>
      <div class="impact-desc">Migrated legacy modules to .NET Core, integrated third-party HR tools, and delivered real-time push notifications to 5,000+ active employees.</div>
    </div>
  </div>

  <!-- Skills -->
  <div class="section">
    <div class="section-label">Tech stack</div>
    <div class="skill-section">
      <div class="skill-dept">Backend — mastery</div>
      <div class="skill-chips">
        <span class="chip primary">C#</span>
        <span class="chip primary">.NET Core</span>
        <span class="chip primary">ASP.NET Web API</span>
        <span class="chip primary">Dapper ORM</span>
        <span class="chip primary">SQL Server</span>
        <span class="chip">ADO.NET</span>
        <span class="chip">OAuth 2.0</span>
        <span class="chip">RESTful APIs</span>
      </div>
    </div>
    <div class="skill-section">
      <div class="skill-dept">Frontend — proficient</div>
      <div class="skill-chips">
        <span class="chip primary">Angular</span>
        <span class="chip primary">TypeScript</span>
        <span class="chip">JavaScript</span>
        <span class="chip">HTML5 / CSS3</span>
        <span class="chip">Bootstrap</span>
      </div>
    </div>
    <div class="skill-section">
      <div class="skill-dept">Cloud & tools — growing</div>
      <div class="skill-chips">
        <span class="chip">Azure · AZ-900</span>
        <span class="chip">Docker</span>
        <span class="chip">Git</span>
        <span class="chip">CI/CD</span>
        <span class="chip">Firebase FCM</span>
        <span class="chip">Postman</span>
      </div>
    </div>
  </div>

  <!-- Current Quest -->
  <div class="section">
    <div class="section-label">Current quest</div>
    <div class="quest-block">
      <div class="quest-item"><div class="quest-dot"></div><span><strong style="color:var(--color-text-primary)">AZ-900</strong> — Azure fundamentals certification in progress</span></div>
      <div class="quest-item"><div class="quest-dot"></div><span><strong style="color:var(--color-text-primary)">React.js</strong> — Expanding frontend beyond Angular</span></div>
      <div class="quest-item"><div class="quest-dot"></div><span><strong style="color:var(--color-text-primary)">Microservices</strong> — Distributed systems architecture patterns</span></div>
    </div>
  </div>

  <!-- Connect -->
  <div class="section">
    <div class="section-label">Department of collaboration</div>
    <div class="connect-row">
      <a class="connect-btn primary" href="https://linkedin.com/in/triilok10" target="_blank">LinkedIn ↗</a>
      <a class="connect-btn" href="mailto:ittiku3@gmail.com">ittiku3@gmail.com</a>
      <a class="connect-btn" href="tel:+918058436268">+91 80584 36268</a>
    </div>
  </div>

  <div class="closing">
    <div class="closing-quote">Clean code today. Cloud-native tomorrow.</div>
  </div>

</div>
