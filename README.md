<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Draxx Editor | Retention Architect & Short-Form Specialist</title>
  <meta name="description" content="High-retention short-form video editing for international founders, podcasters, and performance brands. 70%+ average view duration frameworks.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-base: #07080c;
      --bg-surface: #0e111a;
      --bg-elevated: #161b26;
      --border-subtle: #1f2637;
      --border-glow: #2d374e;
      --accent-emerald: #10b981;
      --accent-emerald-dim: rgba(16, 185, 129, 0.15);
      --accent-cyan: #06b6d4;
      --accent-cyan-dim: rgba(6, 182, 212, 0.15);
      --text-main: #f9fafb;
      --text-muted: #9ca3af;
      --text-dim: #6b7280;
      --font-sans: 'Plus Jakarta Sans', -apple-system, BlinkMacSystemFont, sans-serif;
      --font-mono: 'JetBrains Mono', monospace;
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
      background-color: var(--bg-base);
      color: var(--text-main);
      font-family: var(--font-sans);
      line-height: 1.6;
      overflow-x: hidden;
      background-image: 
        radial-gradient(circle at 15% 20%, rgba(16, 185, 129, 0.08) 0%, transparent 40%),
        radial-gradient(circle at 85% 65%, rgba(6, 182, 212, 0.08) 0%, transparent 40%);
      background-attachment: fixed;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      max-width: 1140px;
      margin: 0 auto;
      padding: 0 1.5rem;
    }

    /* Navigation */
    nav {
      position: sticky;
      top: 0;
      z-index: 100;
      backdrop-filter: blur(16px);
      background: rgba(7, 8, 12, 0.85);
      border-bottom: 1px solid var(--border-subtle);
      padding: 1rem 0;
    }

    .nav-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 0.75rem;
      font-weight: 800;
      font-size: 1.15rem;
      letter-spacing: -0.02em;
    }

    .brand-badge {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 34px;
      height: 34px;
      background: linear-gradient(135deg, var(--accent-emerald), var(--accent-cyan));
      color: #000;
      border-radius: 8px;
      font-weight: 900;
      font-size: 0.9rem;
    }

    .nav-links {
      display: flex;
      gap: 2rem;
      align-items: center;
      font-size: 0.9rem;
      font-weight: 500;
      color: var(--text-muted);
    }

    .nav-links a:hover {
      color: var(--text-main);
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 0.5rem;
      padding: 0.75rem 1.4rem;
      border-radius: 8px;
      font-size: 0.9rem;
      font-weight: 700;
      cursor: pointer;
      transition: all 0.2s ease;
      border: none;
    }

    .btn-primary {
      background: var(--accent-emerald);
      color: #05140d;
      box-shadow: 0 0 24px rgba(16, 185, 129, 0.25);
    }

    .btn-primary:hover {
      background: #0ea372;
      transform: translateY(-1px);
    }

    .btn-secondary {
      background: var(--bg-surface);
      color: var(--text-main);
      border: 1px solid var(--border-subtle);
    }

    .btn-secondary:hover {
      background: var(--bg-elevated);
      border-color: var(--border-glow);
    }

    /* Hero Section */
    .hero {
      padding: 5rem 0 4rem;
      text-align: center;
    }

    .pill-tag {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.35rem 0.9rem;
      background: var(--accent-emerald-dim);
      border: 1px solid rgba(16, 185, 129, 0.3);
      border-radius: 999px;
      font-family: var(--font-mono);
      font-size: 0.75rem;
      color: var(--accent-emerald);
      margin-bottom: 1.5rem;
      font-weight: 600;
      letter-spacing: 0.05em;
      text-transform: uppercase;
    }

    .pill-dot {
      width: 7px;
      height: 7px;
      background: var(--accent-emerald);
      border-radius: 50%;
      box-shadow: 0 0 8px var(--accent-emerald);
    }

    .hero h1 {
      font-size: clamp(2.3rem, 5vw, 3.8rem);
      font-weight: 800;
      line-height: 1.15;
      letter-spacing: -0.03em;
      max-width: 840px;
      margin: 0 auto 1.25rem;
    }

    .hero h1 .highlight {
      background: linear-gradient(135deg, var(--accent-emerald), var(--accent-cyan));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .hero p {
      font-size: 1.125rem;
      color: var(--text-muted);
      max-width: 640px;
      margin: 0 auto 2rem;
    }

    .hero-actions {
      display: flex;
      justify-content: center;
      gap: 1rem;
      flex-wrap: wrap;
    }

    /* Telemetry Stats Bar */
    .telemetry-bar {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
      padding: 2rem;
      background: var(--bg-surface);
      border: 1px solid var(--border-subtle);
      border-radius: 14px;
      margin-bottom: 5rem;
    }

    .telemetry-item {
      text-align: center;
    }

    .telemetry-item .value {
      font-size: 2rem;
      font-weight: 800;
      color: var(--text-main);
      font-family: var(--font-mono);
      display: block;
    }

    .telemetry-item .label {
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      color: var(--text-dim);
      font-weight: 600;
    }

    /* Section Headers */
    .section-header {
      margin-bottom: 2.5rem;
      display: flex;
      justify-content: space-between;
      align-items: flex-end;
      flex-wrap: wrap;
      gap: 1rem;
    }

    .section-header h2 {
      font-size: 2rem;
      font-weight: 800;
      letter-spacing: -0.02em;
    }

    .section-header p {
      color: var(--text-muted);
      font-size: 0.95rem;
      margin-top: 0.25rem;
    }

    /* Portfolio Cards Grid */
    .portfolio-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1.5rem;
      margin-bottom: 4rem;
    }

    .video-card {
      background: var(--bg-surface);
      border: 1px solid var(--border-subtle);
      border-radius: 12px;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      transition: all 0.25s ease;
    }

    .video-card:hover {
      border-color: var(--border-glow);
      transform: translateY(-3px);
      box-shadow: 0 12px 32px rgba(0, 0, 0, 0.4);
    }

    .video-preview {
      position: relative;
      background: #000;
      aspect-ratio: 9/16;
      display: flex;
      align-items: center;
      justify-content: center;
      border-bottom: 1px solid var(--border-subtle);
      overflow: hidden;
    }

    .video-preview-inner {
      text-align: center;
      padding: 1.5rem;
      width: 100%;
    }

    .video-preview .badge-tag {
      position: absolute;
      top: 1rem;
      left: 1rem;
      padding: 0.25rem 0.6rem;
      background: rgba(0, 0, 0, 0.8);
      border: 1px solid var(--border-subtle);
      border-radius: 6px;
      font-family: var(--font-mono);
      font-size: 0.7rem;
      font-weight: 600;
      color: var(--accent-cyan);
    }

    .video-card-body {
      padding: 1.25rem;
      flex-grow: 1;
      display: flex;
      flex-direction: column;
    }

    .video-card-body h3 {
      font-size: 1.1rem;
      font-weight: 700;
      margin-bottom: 0.5rem;
    }

    .video-card-body p {
      color: var(--text-muted);
      font-size: 0.85rem;
      line-height: 1.5;
      margin-bottom: 1rem;
      flex-grow: 1;
    }

    .specs-list {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
      gap: 0.4rem;
      margin-bottom: 1.25rem;
    }

    .specs-list li {
      font-family: var(--font-mono);
      font-size: 0.7rem;
      padding: 0.2rem 0.5rem;
      background: var(--bg-elevated);
      border: 1px solid var(--border-subtle);
      border-radius: 4px;
      color: var(--text-dim);
    }

    /* Drive Master Box */
    .drive-banner {
      background: linear-gradient(135deg, rgba(16, 185, 129, 0.08), rgba(6, 182, 212, 0.08));
      border: 1px solid rgba(16, 185, 129, 0.3);
      border-radius: 12px;
      padding: 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 1.5rem;
      margin-bottom: 5rem;
    }

    .drive-banner h3 {
      font-size: 1.25rem;
      font-weight: 800;
      margin-bottom: 0.25rem;
    }

    .drive-banner p {
      color: var(--text-muted);
      font-size: 0.9rem;
    }

    /* Retention Curve Graphic */
    .retention-section {
      background: var(--bg-surface);
      border: 1px solid var(--border-subtle);
      border-radius: 14px;
      padding: 2.5rem 2rem;
      margin-bottom: 5rem;
    }

    .chart-container {
      margin-top: 2rem;
      background: #050608;
      border: 1px solid var(--border-subtle);
      border-radius: 10px;
      padding: 1.5rem;
    }

    .chart-legend {
      display: flex;
      gap: 2rem;
      margin-bottom: 1rem;
      font-size: 0.8rem;
      font-family: var(--font-mono);
    }

    .legend-item {
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .legend-color {
      width: 12px;
      height: 3px;
      border-radius: 2px;
    }

    /* Pricing Section */
    .pricing-section {
      margin-bottom: 5rem;
    }

    .currency-switcher {
      display: inline-flex;
      background: var(--bg-surface);
      border: 1px solid var(--border-subtle);
      padding: 4px;
      border-radius: 8px;
      gap: 4px;
    }

    .currency-btn {
      padding: 0.4rem 0.9rem;
      border-radius: 6px;
      font-family: var(--font-mono);
      font-size: 0.8rem;
      font-weight: 700;
      cursor: pointer;
      background: transparent;
      border: none;
      color: var(--text-dim);
      transition: all 0.2s;
    }

    .currency-btn.active {
      background: var(--bg-elevated);
      color: var(--text-main);
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.3);
    }

    .pricing-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.5rem;
      margin-top: 2rem;
    }

    .pricing-card {
      background: var(--bg-surface);
      border: 1px solid var(--border-subtle);
      border-radius: 14px;
      padding: 2rem;
      display: flex;
      flex-direction: column;
      position: relative;
    }

    .pricing-card.featured {
      border-color: var(--accent-emerald);
      background: linear-gradient(180deg, rgba(16, 185, 129, 0.04), var(--bg-surface));
    }

    .featured-tag {
      position: absolute;
      top: -12px;
      right: 2rem;
      background: var(--accent-emerald);
      color: #03140c;
      font-family: var(--font-mono);
      font-size: 0.7rem;
      font-weight: 800;
      padding: 0.25rem 0.6rem;
      border-radius: 4px;
      text-transform: uppercase;
    }

    .pricing-card h3 {
      font-size: 1.3rem;
      font-weight: 800;
      margin-bottom: 0.5rem;
    }

    .pricing-card .price {
      font-size: 2.4rem;
      font-weight: 800;
      font-family: var(--font-mono);
      margin: 1rem 0;
      color: var(--text-main);
    }

    .pricing-card .price span {
      font-size: 0.9rem;
      color: var(--text-dim);
      font-weight: 500;
    }

    .pricing-features {
      list-style: none;
      margin: 1.5rem 0 2rem;
      flex-grow: 1;
    }

    .pricing-features li {
      display: flex;
      align-items: flex-start;
      gap: 0.75rem;
      font-size: 0.9rem;
      color: var(--text-muted);
      margin-bottom: 0.75rem;
    }

    .pricing-features li svg {
      flex-shrink: 0;
      margin-top: 3px;
      color: var(--accent-emerald);
    }

    /* Modal */
    .modal-backdrop {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(0, 0, 0, 0.85);
      backdrop-filter: blur(8px);
      z-index: 1000;
      align-items: center;
      justify-content: center;
      padding: 1.5rem;
    }

    .modal-backdrop.active {
      display: flex;
    }

    .modal-window {
      background: var(--bg-surface);
      border: 1px solid var(--border-glow);
      border-radius: 14px;
      max-width: 520px;
      width: 100%;
      padding: 2rem;
      position: relative;
    }

    .modal-close {
      position: absolute;
      top: 1.25rem;
      right: 1.25rem;
      background: transparent;
      border: none;
      color: var(--text-muted);
      font-size: 1.4rem;
      cursor: pointer;
    }

    .form-group {
      margin-bottom: 1.25rem;
    }

    .form-group label {
      display: block;
      font-size: 0.85rem;
      font-weight: 600;
      color: var(--text-muted);
      margin-bottom: 0.4rem;
    }

    .form-group input, .form-group textarea {
      width: 100%;
      background: var(--bg-base);
      border: 1px solid var(--border-subtle);
      border-radius: 6px;
      padding: 0.75rem;
      color: #fff;
      font-family: inherit;
      font-size: 0.9rem;
    }

    .form-group input:focus, .form-group textarea:focus {
      outline: none;
      border-color: var(--accent-emerald);
    }

    /* Footer */
    footer {
      border-top: 1px solid var(--border-subtle);
      padding: 3rem 0;
      color: var(--text-dim);
      font-size: 0.85rem;
      text-align: center;
    }

    .toast {
      position: fixed;
      bottom: 2rem;
      right: 2rem;
      background: var(--accent-emerald);
      color: #03140c;
      padding: 0.75rem 1.4rem;
      border-radius: 8px;
      font-weight: 700;
      font-size: 0.85rem;
      display: none;
      z-index: 2000;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.4);
    }

    @media (max-width: 768px) {
      .nav-links { display: none; }
      .hero h1 { font-size: 2.2rem; }
      .drive-banner { flex-direction: column; text-align: center; }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <div class="container nav-inner">
      <div class="brand">
        <span class="brand-badge">DX</span>
        <span>DRAXX EDITOR</span>
      </div>
      <div class="nav-links">
        <a href="#portfolio">Portfolio Assets</a>
        <a href="#framework">Retention Engine</a>
        <a href="#pricing">Retainers</a>
      </div>
      <button class="btn btn-primary" onclick="openModal()">Request Trial Cut</button>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <div class="container">
      <div class="pill-tag">
        <span class="pill-dot"></span>
        Zero Fluff • 70%+ Retention Framework
      </div>
      <h1>High-Retention Short Form For <span class="highlight">Founders & Brands</span></h1>
      <p>Pacing psychology, visual storytelling metaphors, and studio audio ducking built to stop the scroll and drive commercial outcomes.</p>
      <div class="hero-actions">
        <a href="#portfolio" class="btn btn-primary">Review Work Samples</a>
        <button class="btn btn-secondary" onclick="copyDriveLink()">Copy Drive Link</button>
      </div>
    </div>
  </section>

  <main class="container">
    <!-- Telemetry Stats -->
    <div class="telemetry-bar">
      <div class="telemetry-item">
        <span class="value">&lt; 0.18s</span>
        <span class="label">Dead-Air Pacing Floor</span>
      </div>
      <div class="telemetry-item">
        <span class="value">72%+</span>
        <span class="label">Avg Hook Completion</span>
      </div>
      <div class="telemetry-item">
        <span class="value">-24 dB</span>
        <span class="label">Dynamic BGM Ducking</span>
      </div>
      <div class="telemetry-item">
        <span class="value">24–48h</span>
        <span class="label">Async Turnaround</span>
      </div>
    </div>

    <!-- Portfolio Section -->
    <section id="portfolio">
      <div class="section-header">
        <div>
          <h2>Locked Portfolio Assets</h2>
          <p>Four distinct commercial editing archetypes. No generic auto-captions.</p>
        </div>
        <button class="btn btn-secondary" onclick="copyDriveLink()">Copy All 4 Samples Link</button>
      </div>

      <div class="portfolio-grid">
        <!-- Asset 1 -->
        <div class="video-card">
          <div class="video-preview">
            <span class="badge-tag">STORYTELLING</span>
            <div class="video-preview-inner">
              <p style="font-size: 0.75rem; color: var(--accent-cyan); font-family: var(--font-mono); margin-bottom: 0.4rem;">CHRIS WILLIAMSON</p>
              <h4 style="font-size: 1rem; font-weight: 800;">"If Life Was A Movie"</h4>
              <p style="font-size: 0.75rem; color: var(--text-dim); margin-top: 0.4rem;">Depth & Cutout Layer</p>
            </div>
          </div>
          <div class="video-card-body">
            <h3>Visual Narrative Metaphor</h3>
            <p>Text-behind-subject 2.5D layer with rapid metaphorical cuts: broken polaroids, corporate badges, and horror audio risers.</p>
            <ul class="specs-list">
              <li>Text-Behind-Subject</li>
              <li>Atmospheric SFX</li>
              <li>Curiosity Loop</li>
            </ul>
            <button class="btn btn-secondary" style="width: 100%; font-size: 0.8rem;" onclick="openDrive()">Inspect in Drive</button>
          </div>
        </div>

        <!-- Asset 2 -->
        <div class="video-card">
          <div class="video-preview">
            <span class="badge-tag">KINETIC PACING</span>
            <div class="video-preview-inner">
              <p style="font-size: 0.75rem; color: var(--accent-emerald); font-family: var(--font-mono); margin-bottom: 0.4rem;">ALEX HORMOZI</p>
              <h4 style="font-size: 1rem; font-weight: 800;">"6 Mo vs 10 Years"</h4>
              <p style="font-size: 0.75rem; color: var(--text-dim); margin-top: 0.4rem;">Split Pacing Engine</p>
            </div>
          </div>
          <div class="video-card-body">
            <h3>Founder Business Breakdown</h3>
            <p>High-contrast typographic framework. Sequential B-roll contrast replacing generic animations with real-world execution metrics.</p>
            <ul class="specs-list">
              <li>Kinetic Typography</li>
              <li>High-Contrast Cuts</li>
              <li>Sound Design</li>
            </ul>
            <button class="btn btn-secondary" style="width: 100%; font-size: 0.8rem;" onclick="openDrive()">Inspect in Drive</button>
          </div>
        </div>

        <!-- Asset 3 -->
        <div class="video-card">
          <div class="video-preview">
            <span class="badge-tag">PODCAST MASTER</span>
            <div class="video-preview-inner">
              <p style="font-size: 0.75rem; color: var(--accent-cyan); font-family: var(--font-mono); margin-bottom: 0.4rem;">RANVEER / SUFIYAN</p>
              <h4 style="font-size: 1rem; font-weight: 800;">"We Are All Ghosts"</h4>
              <p style="font-size: 0.75rem; color: var(--text-dim); margin-top: 0.4rem;">Shock Pacing Cut</p>
            </div>
          </div>
          <div class="video-card-body">
            <h3>Conversational Hook Pacing</h3>
            <p>Instant shock-value pattern interrupt hook, rapid micro-zooms on speech cadence, and spectral audio transition cues.</p>
            <ul class="specs-list">
              <li>Pattern Interrupt</li>
              <li>Sub-Bass Drops</li>
              <li>Zero Dead-Air</li>
            </ul>
            <button class="btn btn-secondary" style="width: 100%; font-size: 0.8rem;" onclick="openDrive()">Inspect in Drive</button>
          </div>
        </div>

        <!-- Asset 4 -->
        <div class="video-card">
          <div class="video-preview">
            <span class="badge-tag">PERFORMANCE UGC</span>
            <div class="video-preview-inner">
              <p style="font-size: 0.75rem; color: var(--accent-emerald); font-family: var(--font-mono); margin-bottom: 0.4rem;">DIRECT RESPONSE</p>
              <h4 style="font-size: 1rem; font-weight: 800;">"Winter Window Tint"</h4>
              <p style="font-size: 0.75rem; color: var(--text-dim); margin-top: 0.4rem;">Commercial Ad Cut</p>
            </div>
          </div>
          <div class="video-card-body">
            <h3>High-Converting Ad Format</h3>
            <p>Aggressive 13-second commercial edit locked to beat-drop rhythm, UV protection badge animations, and direct-response CTA overlays.</p>
            <ul class="specs-list">
              <li>Beat-Drop Sync</li>
              <li>UGC Direct-Response</li>
              <li>Clean Audio Vocal</li>
            </ul>
            <button class="btn btn-secondary" style="width: 100%; font-size: 0.8rem;" onclick="openDrive()">Inspect in Drive</button>
          </div>
        </div>
      </div>

      <!-- Drive Master Link Banner -->
      <div class="drive-banner">
        <div>
          <h3>Direct Access: Verified Raw Master Files</h3>
          <p>Clean Google Drive folder set to Public View. No download or registration required.</p>
        </div>
        <div style="display: flex; gap: 0.75rem; flex-wrap: wrap;">
          <button class="btn btn-primary" onclick="openDrive()">Open Drive Folder</button>
          <button class="btn btn-secondary" onclick="copyPitch()">Copy Pitch Script</button>
        </div>
      </div>
    </section>

    <!-- Retention Section -->
    <section id="framework" class="retention-section">
      <div class="section-header">
        <div>
          <h2>The Retention Framework</h2>
          <p>Why standard edits drop viewers at 3 seconds, and how our pacing holds past the 70% mark.</p>
        </div>
      </div>
      <div class="chart-container">
        <div class="chart-legend">
          <div class="legend-item">
            <div class="legend-color" style="background: var(--accent-emerald);"></div>
            <span>Draxx Retention Engine (72% Avg)</span>
          </div>
          <div class="legend-item">
            <div class="legend-color" style="background: #ef4444;"></div>
            <span>Standard Amateur Reel (22% Avg)</span>
          </div>
        </div>
        <!-- SVG Graphic Representation -->
        <svg viewBox="0 0 800 240" style="width: 100%; height: auto; overflow: visible;">
          <defs>
            <linearGradient id="emeraldGrad" x1="0%" y1="0%" x2="0%" y2="100%">
              <stop offset="0%" stop-color="#10b981" stop-opacity="0.3"/>
              <stop offset="100%" stop-color="#10b981" stop-opacity="0.0"/>
            </linearGradient>
          </defs>
          <!-- Grid Lines -->
          <line x1="50" y1="20" x2="780" y2="20" stroke="#1f2637" stroke-dasharray="4"/>
          <line x1="50" y1="80" x2="780" y2="80" stroke="#1f2637" stroke-dasharray="4"/>
          <line x1="50" y1="140" x2="780" y2="140" stroke="#1f2637" stroke-dasharray="4"/>
          <line x1="50" y1="200" x2="780" y2="200" stroke="#1f2637"/>
          <!-- Axis Labels -->
          <text x="10" y="24" fill="#6b7280" font-family="monospace" font-size="11">100%</text>
          <text x="18" y="84" fill="#6b7280" font-family="monospace" font-size="11">75%</text>
          <text x="18" y="144" fill="#6b7280" font-family="monospace" font-size="11">50%</text>
          <text x="18" y="204" fill="#6b7280" font-family="monospace" font-size="11">0%</text>
          <!-- Amateur Curve (Red) -->
          <path d="M 50 20 Q 90 140 180 170 T 400 190 T 780 195" fill="none" stroke="#ef4444" stroke-width="2.5" stroke-dasharray="6"/>
          <!-- Draxx Retention Curve (Emerald) -->
          <path d="M 50 20 C 100 25, 140 50, 240 55 C 380 60, 520 65, 780 75" fill="none" stroke="#10b981" stroke-width="3"/>
          <path d="M 50 20 C 100 25, 140 50, 240 55 C 380 60, 520 65, 780 75 L 780 200 L 50 200 Z" fill="url(#emeraldGrad)"/>
          <!-- Key Points -->
          <circle cx="140" cy="50" r="5" fill="#10b981"/>
          <text x="145" y="42" fill="#10b981" font-family="monospace" font-weight="700" font-size="11">Hook Lock (0:02)</text>
          <circle cx="450" cy="62" r="5" fill="#10b981"/>
          <text x="455" y="54" fill="#06b6d4" font-family="monospace" font-weight="700" font-size="11">Metaphor Shift (0:12)</text>
        </svg>
      </div>
    </section>

    <!-- Pricing Section -->
    <section id="pricing" class="pricing-section">
      <div class="section-header">
        <div>
          <h2>Predictable Monthly Retainers</h2>
          <p>Flat rates. No per-cut invoice friction. Cancel anytime.</p>
        </div>
        <div class="currency-switcher">
          <button id="btn-usd" class="currency-btn active" onclick="setCurrency('USD')">USD ($)</button>
          <button id="btn-inr" class="currency-btn" onclick="setCurrency('INR')">INR (₹)</button>
        </div>
      </div>

      <div class="pricing-grid">
        <!-- Starter -->
        <div class="pricing-card">
          <h3>Starter Flow</h3>
          <p style="color: var(--text-dim); font-size: 0.85rem;">For founders testing short-form traction.</p>
          <div class="price" id="price-starter">$350 <span>/ month</span></div>
          <ul class="pricing-features">
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> 10 High-retention vertical edits / month</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> Aggressive dead-air trimming</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> Studio voice cleaning & ducking</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> 48-Hour delivery queue</li>
          </ul>
          <button class="btn btn-secondary" onclick="openModal('Starter Retainer')">Lock Starter Spot</button>
        </div>

        <!-- Growth (Featured) -->
        <div class="pricing-card featured">
          <span class="featured-tag">MOST POPULAR</span>
          <h3>Growth Partner</h3>
          <p style="color: var(--text-dim); font-size: 0.85rem;">The sweet spot for consistent weekly cadence.</p>
          <div class="price" id="price-growth" style="color: var(--accent-emerald);">$500 <span>/ month</span></div>
          <ul class="pricing-features">
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> <strong>20 High-retention vertical edits / month</strong></li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> Kinetic typography & custom B-roll</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> 2 Unique hook styles per video</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> Priority 24–48 hour turnaround</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> Async workflow (Slack/Twitter/Drive)</li>
          </ul>
          <button class="btn btn-primary" onclick="openModal('Growth Retainer')">Lock Growth Spot</button>
        </div>

        <!-- Scale -->
        <div class="pricing-card">
          <h3>Daily Dominance</h3>
          <p style="color: var(--text-dim); font-size: 0.85rem;">Complete daily short-form takeover.</p>
          <div class="price" id="price-scale">$850 <span>/ month</span></div>
          <ul class="pricing-features">
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> 30 High-retention edits / month (Daily post)</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> Complete sound design & metaphor layers</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> Dedicated 24h turnaround pipeline</li>
            <li><svg width="18" height="18" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M20 6L9 17l-5-5"/></svg> Direct async revisions channel</li>
          </ul>
          <button class="btn btn-secondary" onclick="openModal('Daily Dominance')">Lock Dominance Spot</button>
        </div>
      </div>
    </section>
  </main>

  <!-- Modal for Trial Requests -->
  <div class="modal-backdrop" id="trial-modal" onclick="closeModalOnBackdrop(event)">
    <div class="modal-window">
      <button class="modal-close" onclick="closeModal()">&times;</button>
      <h3 style="font-size: 1.4rem; font-weight: 800; margin-bottom: 0.5rem;">Claim Async Trial Cut</h3>
      <p style="color: var(--text-muted); font-size: 0.85rem; margin-bottom: 1.5rem;">I cut a 15–20s scroll-stopping hook from your raw footage for free so you can evaluate the pacing firsthand.</p>
      
      <form onsubmit="handleTrialSubmit(event)">
        <div class="form-group">
          <label>Your Name / Brand / X Handle</label>
          <input type="text" id="trial-name" placeholder="@yourhandle or Brand" required>
        </div>
        <div class="form-group">
          <label>Raw Footage Link (Drive / Dropbox / Loom)</label>
          <input type="url" id="trial-link" placeholder="https://drive.google.com/..." required>
        </div>
        <div class="form-group">
          <label>Selected Tier / Specific Goals</label>
          <textarea id="trial-notes" rows="3" placeholder="Targeting YouTube Shorts / IG Reels. Focus on high watch time..."></textarea>
        </div>
        <button type="submit" class="btn btn-primary" style="width: 100%;">Submit Raw Footage For Trial</button>
      </form>
    </div>
  </div>

  <!-- Toast Notification -->
  <div class="toast" id="toast">Link copied to clipboard!</div>

  <!-- Footer -->
  <footer>
    <div class="container">
      <p style="margin-bottom: 0.5rem; font-weight: 700; color: var(--text-main);">DRAXX EDITOR • SHORT-FORM RETENTION ARCHITECTURE</p>
      <p>Built for async execution with international creators and performance brands.</p>
    </div>
  </footer>

  <script>
    const DRIVE_LINK = "https://drive.google.com/drive/folders/1xnKoUrR6agjsNNT_u6f1_EEhOSMJ_nGL";

    const PITCH_SCRIPT = `Hey, saw your post regarding short-form video editing.
I specialize in high-retention vertical cuts—clean kinetic typography, narrative B-roll metaphors, and crisp sound design built specifically to stop the scroll.
Here are 4 fresh portfolio samples (Podcast, Talking-Head, and Commercial UGC):
🔗 ${DRIVE_LINK}
I'd love to edit a quick 15-20s test hook from your raw footage today so you can evaluate my pacing and turnaround speed. Let me know!`;

    function openDrive() {
      window.open(DRIVE_LINK, '_blank');
    }

    function copyDriveLink() {
      navigator.clipboard.writeText(DRIVE_LINK).then(() => {
        showToast("Drive portfolio link copied!");
      });
    }

    function copyPitch() {
      navigator.clipboard.writeText(PITCH_SCRIPT).then(() => {
        showToast("Outreach pitch script copied!");
      });
    }

    function showToast(text) {
      const toast = document.getElementById('toast');
      toast.innerText = text;
      toast.style.display = 'block';
      setTimeout(() => {
        toast.style.display = 'none';
      }, 2500);
    }

    // Currency Switcher Logic
    function setCurrency(curr) {
      const btnUsd = document.getElementById('btn-usd');
      const btnInr = document.getElementById('btn-inr');
      const pStarter = document.getElementById('price-starter');
      const pGrowth = document.getElementById('price-growth');
      const pScale = document.getElementById('price-scale');

      if (curr === 'USD') {
        btnUsd.classList.add('active');
        btnInr.classList.remove('active');
        pStarter.innerHTML = '$350 <span>/ month</span>';
        pGrowth.innerHTML = '$500 <span>/ month</span>';
        pScale.innerHTML = '$850 <span>/ month</span>';
      } else {
        btnInr.classList.add('active');
        btnUsd.classList.remove('active');
        pStarter.innerHTML = '₹29,500 <span>/ month</span>';
        pGrowth.innerHTML = '₹42,500 <span>/ month</span>';
        pScale.innerHTML = '₹72,000 <span>/ month</span>';
      }
    }

    // Modal Operations
    function openModal(planName) {
      if (planName) {
        document.getElementById('trial-notes').value = `Interested in: ${planName}`;
      }
      document.getElementById('trial-modal').classList.add('active');
    }

    function closeModal() {
      document.getElementById('trial-modal').classList.remove('active');
    }

    function closeModalOnBackdrop(e) {
      if (e.target.id === 'trial-modal') {
        closeModal();
      }
    }

    function handleTrialSubmit(e) {
      e.preventDefault();
      const name = document.getElementById('trial-name').value;
      const link = document.getElementById('trial-link').value;
      closeModal();
      showToast("Trial request received! Turnaround window: 24h.");
      window.location.href = `mailto:editor@draxx.media?subject=Trial Cut Request - ${encodeURIComponent(name)}&body=Raw Footage Link: ${encodeURIComponent(link)}`;
    }
  </script>
</body>
</html>
