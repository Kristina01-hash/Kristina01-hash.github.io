<!-- Google Fonts for modern typography -->

<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Inter:wght@400;600&display=swap" rel="stylesheet">

<!-- Hero Section -->

<section class="hero-section">
  <div class="hero-content">
    <img src="/assets/images/mobius_blog_spinning.png" alt="Mobius Blog Spinner" class="mobius-spin" style="width: 120px; margin: 0 auto 20px auto; display: block;" />
    <h1>Kristina's Blog</h1>
    <p class="hero-subtitle">You can find thoughts, humor, reflections, and notes about everything in a very sarcastic and spicy manner—no sugarcoating. You never expected this side of me. Enjoy the blog!</p>
  </div>
</section>
<!--<img src="/assets/images/mobius_blog.png" alt="Mobius Blog Banner" style="width: 120px; float: right; margin: 20px;" />-->

<!-- Preserved Blinking Möbius SVG -->

<svg width="120" height="120" viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg" style="display: block; margin: 30px auto;">
  <title>Möbius: Engineered Logic, Sprinkled with Irony</title>
  <defs>
    <radialGradient id="mobiusGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#99ffcc" />
      <stop offset="100%" stop-color="#1f1f2e" />
    </radialGradient>
  </defs>
  <g>
    <ellipse cx="50" cy="50" rx="35" ry="20" fill="url(#mobiusGlow)" stroke="#ff66a6" stroke-width="2">
      <animateTransform attributeName="transform" attributeType="XML" type="rotate" from="0 50 50" to="360 50 50" dur="12s" repeatCount="indefinite"/>
    </ellipse>
    <circle cx="65" cy="45" r="4" fill="#ff66a6">
      <animate attributeName="r" values="4;1;4" dur="3s" repeatCount="indefinite"/>
    </circle>
  </g>
</svg>

<!-- Most Recent Posts -->

<section class="recent-posts callout" aria-labelledby="recent-posts-title">
  <h2 id="recent-posts-title">Most Recent Posts</h2>
  <ol>
    <li>
      <span class="post-icon" aria-hidden="true">🎪</span>
      <a class="post-link" href="https://kristina01-hash.github.io/clown-network/chronicles/20260815_Shopee%20airpods%20investigation%20blog.html"> The Shopee AirPods Pro 3 Investigation
</a>
      <span class="badge new">NEW</span>
      <p class="excerpt"> How a Gray Market Device, Broken Return Policy, and Systemic Incompetence Exposed the Reality of Southeast Asian E-Commerce. 
    <li>
      <span class="post-icon" aria-hidden="true">🎪</span>
      <a class="post-link" href="https://kristina01-hash.github.io/clown-network/chronicles/20260809_airpods_blog_post.html"> Personal Essay: I Went Looking for AirPods Pro 3
</a>
      <span class="badge new">NEW</span>
      <p class="excerpt"> The day I tried to buy AirPods Pro 3 and accidentally conducted a national infrastructure audit. 
    <li>
      <span class="post-icon" aria-hidden="true">📚</span>
      <a class="post-link" href="https://kristina01-hash.github.io/clown-network/chronicles/2026-07-28_clustering-you-need-to-know.html"> Teaching a Computer to See in Shades of Gray
</a>
      <span class="badge new">NEW</span>
      <p class="excerpt"> Finally, I'm writing back about academic stuff! 😉 Here's an example of when maths meets its application in medical image segmentation: In review.  </p>
    </li> 


<!-- Floating Emojis (improved animation) -->

<div class="float-emoji" style="left: 10%; animation-delay: 0s;">👽</div>
<div class="float-emoji" style="left: 25%; animation-delay: 2s;">👽</div>
<div class="float-emoji" style="left: 40%; animation-delay: 4s;">👽</div>
<div class="float-emoji" style="left: 60%; animation-delay: 6s;">👽</div>
<div class="float-emoji" style="left: 80%; animation-delay: 8s;">👽</div>

<!-- Preserved Background Music Player -->

<audio id="background-music" loop>
  <source src="/assets/audio/clown-circus.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

<div class="music-controls">
  <button aria-label="Play background music" onclick="document.getElementById('background-music').play()">▶️ Play Marching Music</button>
  <button aria-label="Pause background music" onclick="document.getElementById('background-music').pause()">⏸️ Pause</button>
</div>

<script>
  // Preserved audio autoplay logic
  const audio = document.getElementById('background-music');
  const isMobile = /iPhone|iPad|iPod|Android/i.test(navigator.userAgent);
  if (!isMobile) {
    audio.autoplay = true;
    audio.load();
  } else {
    audio.pause();
  }
</script>

<main>
<section class="intro-section">
  <h2>Welcome to the Blog</h2>
  <p>Here you can find information about many different topics, presented in a sarcastic and satirical style. This is stronger than the person who taught you to scream 😉. This page shows that people are involved, but they also speak up in a way you never would have thought possible 😎.</p>
</section>

<section class="work-philosophy">
  <h2>Value-Driven Work: Delivering Impact Beyond Hours</h2>
  <p>In today's evolving workplace, success is measured by outcomes, not time spent at a desk. I focus on creating tangible value through purposeful work and strategic thinking.</p>
  <blockquote>"It's not about being seen working—it's about delivering something worth seeing."</blockquote>
  <p>I don't subscribe to outdated models of productivity rooted in clock-ins, noise, and endless meetings. I believe in intentional, outcome-driven work guided by deep focus and systems thinking.</p>
  <div class="highlight">You'll get real work done if you treat it like a hobby. Is there anything else besides that? That's a bullshit!</div>
  <p>If you're someone who values sharp thinking over surface performance, results over rituals, and depth over noise—we're probably aligned.</p>
  <div class="audio-player">
    <p class="audio-title">Hear my thoughts on modern work culture:</p>
    <audio controls>
      <source src="/assets/audio/modern_work_culture.mp3" type="audio/mp3">
      Your browser does not support the audio element.
    </audio>
  </div>
  <h3>Core Principles</h3>
  <div class="principles-grid">
    <div class="principle-card">
      <div class="principle-icon"><i class="fas fa-bullseye" aria-hidden="true"></i></div>
      <h4>Outcome-Focused</h4>
      <p>I measure success by tangible results and impact, not by hours logged or tasks completed.</p>
    </div>
    <div class="principle-card">
      <div class="principle-icon"><i class="fas fa-brain" aria-hidden="true"></i></div>
      <h4>Deep Focus</h4>
      <p>Quality work requires uninterrupted concentration and deliberate thinking without constant distractions.</p>
    </div>
    <div class="principle-card">
      <div class="principle-icon"><i class="fas fa-handshake" aria-hidden="true"></i></div>
      <h4>Try and See</h4>
      <p>I believe in experimenting and iterating quickly to find effective solutions rather than over-planning.</p>
    </div>
    <div class="principle-card">
      <div class="principle-icon"><i class="fas fa-lightbulb" aria-hidden="true"></i></div>
      <h4>Continuous Learning</h4>
      <p>I am committed to lifelong learning and regularly updating my skills to stay ahead in my field.</p>
    </div>
    <div class="principle-card">
      <div class="principle-icon"><i class="fas fa-sitemap" aria-hidden="true"></i></div>
      <h4>Systems Approach</h4>
      <p>I build scalable systems and frameworks rather than one-off solutions to create lasting value.</p>
    </div>
    <div class="principle-card">
      <div class="principle-icon"><i class="fas fa-lightbulb" aria-hidden="true"></i></div>
      <h4>Continuous Innovation</h4>
      <p>Staying ahead requires constant learning, adaptation, and willingness to challenge the status quo.</p>
    </div>
  </div>
</section>
</main>

---

## Featured Archive

Do you need a stronger way to express your emotions than words?
Check out the full **Clown Network Chronicles**, which is like an online library with information on all kinds of topics.

<div style="margin: 2em 0; text-align: center;">
  <a href="/clown-network/chronicles/" class="cta-button">
    <span class="clown-icon">🎪</span> Visit the Clown Network Chronicles →
  </a>
</div>

---

This blog has a variety of information, including data, sarcasm, and observations. If you like to speak frankly, meaning in a direct way, you'll enjoy this blog. If you're not comfortable with that, this platform isn't for you.

<!-- Dark Mode Toggle -->

<div class="dark-toggle">
  <button aria-label="Toggle dark mode" onclick="toggleDarkMode()">🌓 Toggle Dark Mode</button>
</div>

<script>
  function toggleDarkMode() {
    document.body.classList.toggle('dark-mode');
    localStorage.setItem('theme', document.body.classList.contains('dark-mode') ? 'dark' : 'light');
    // Ensure animations continue working in dark mode
    const mobiusSpin = document.querySelector('.mobius-spin');
    if (mobiusSpin) {
      mobiusSpin.style.animation = 'none';
      setTimeout(() => {
        mobiusSpin.style.animation = 'spin 5s linear infinite';
      }, 10);
    }
  }
  window.onload = () => {
    if (localStorage.getItem('theme') === 'dark') {
      document.body.classList.add('dark-mode');
    }
    // Add Font Awesome for icons if not already present
    if (!document.querySelector('link[href*="font-awesome"]')) {
      const link = document.createElement('link');
      link.rel = 'stylesheet';
      link.href = 'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css';
      document.head.appendChild(link);
    }
  }
</script>

<style>
  :root {
    --bg: #f6f4ff;
    --bg-accent: #fff4f8;
    --surface: #ffffff;
    --surface-alt: #f4f7ff;
    --text-color: #2e233b;
    --muted-text: #6e5f79;
    --primary-color: #b30059;
    --primary-strong: #8f0047;
    --primary-light: #ffe9f2;
    --secondary-color: #0f7a8a;
    --secondary-light: #e4f7fa;
    --accent-color: #f2a93b;
    --accent-soft: #fff1d7;
    --border-color: rgba(15, 122, 138, 0.18);
    --shadow-color: rgba(46, 35, 59, 0.12);
    --link-color: #0f7a8a;
  }

  html { scroll-behavior: smooth; }

  body {
    background: linear-gradient(135deg, var(--bg) 0%, var(--bg-accent) 45%, var(--surface-alt) 100%);
    background-size: cover;
    position: relative;
    overflow-x: hidden;
    font-family: 'Inter', 'Montserrat', Arial, sans-serif;
    color: var(--text-color);
    line-height: 1.7;
    font-size: 1.08em;
    margin: 0;
    transition: background 0.3s ease, color 0.3s ease;
  }

  a { color: var(--link-color); }

  .hero-section {
    background: linear-gradient(90deg, #ffe7f0 0%, #f6ebff 50%, #e7f8fb 100%);
    padding: 3.5em 0 2em 0;
    text-align: center;
    border-radius: 0 0 32px 32px;
    box-shadow: 0 2px 18px rgba(179, 0, 89, 0.08);
    margin-bottom: 2em;
  }

  .hero-content h1 {
    font-family: 'Montserrat', sans-serif;
    font-size: 2.8em;
    margin-bottom: 0.2em;
    color: var(--secondary-color);
    letter-spacing: 0.01em;
  }

  .hero-subtitle {
    font-style: italic;
    color: var(--secondary-color);
    font-size: 1.25em;
    margin-bottom: 0;
  }

  .intro-section {
    max-width: 700px;
    margin: 0 auto 2em auto;
    padding: 0 1em;
  }

  .work-philosophy {
    background-color: var(--surface);
    border-radius: 14px;
    padding: 2.2rem 2rem;
    margin: 2rem auto;
    box-shadow: 0 6px 20px var(--shadow-color);
    max-width: 800px;
    border: 1px solid var(--border-color);
  }

  .work-philosophy h2 {
    color: var(--primary-color);
    font-family: 'Montserrat', sans-serif;
    font-weight: 700;
    font-size: 2em;
    margin-bottom: 0.5em;
  }

  .work-philosophy blockquote {
    font-style: italic;
    border-left: 4px solid var(--primary-color);
    padding: 1rem 2rem;
    margin: 2rem 0;
    background-color: var(--primary-light);
    position: relative;
    font-size: 1.2rem;
    color: var(--primary-color);
    border-radius: 8px;
  }

  .highlight {
    background: linear-gradient(90deg, var(--primary-light) 0%, var(--accent-soft) 100%);
    padding: 1rem;
    display: block;
    margin: 1.5rem 0;
    border-left: 4px solid var(--accent-color);
    border-radius: 8px;
    font-size: 1.08em;
  }

  .principles-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
  }

  .principle-card {
    background-color: var(--surface);
    border-radius: 10px;
    padding: 1.5rem 1.2rem;
    box-shadow: 0 4px 12px var(--shadow-color);
    transition: transform 0.3s, box-shadow 0.3s;
    text-align: center;
    border: 1px solid var(--border-color);
  }

  .principle-card:hover {
    transform: translateY(-7px) scale(1.03);
    box-shadow: 0 8px 24px rgba(46, 35, 59, 0.16);
  }

  .principle-icon {
    font-size: 2.2rem;
    color: var(--secondary-color);
    margin-bottom: 1rem;
  }

  .cta-button {
    background: linear-gradient(90deg, var(--primary-color) 0%, var(--accent-color) 100%);
    color: white;
    padding: 0.9em 1.7em;
    border-radius: 999px;
    text-decoration: none;
    font-weight: bold;
    display: inline-block;
    box-shadow: 0 4px 10px rgba(179, 0, 89, 0.18);
    font-size: 1.15em;
    transition: transform 0.2s, box-shadow 0.2s;
    border: none;
    cursor: pointer;
  }

  .cta-button:hover {
    transform: scale(1.06);
    box-shadow: 0 8px 18px rgba(179, 0, 89, 0.24);
  }

  .cta-button .clown-icon {
    display: inline-block;
    transition: transform 0.6s;
  }

  .cta-button:hover .clown-icon {
    transform: rotate(360deg);
  }

  .float-emoji {
    position: absolute;
    animation: float 14s linear infinite, glitch 1.2s infinite;
    font-size: 2em;
    opacity: 0.32;
    pointer-events: none;
    z-index: 1;
  }

  @keyframes float {
    0% { transform: translateY(100vh) translateX(0); }
    100% { transform: translateY(-200vh) translateX(100px); }
  }

  @keyframes glitch {
    0% { text-shadow: 2px 2px #ff4d7d; }
    20% { text-shadow: -2px -2px #5dc9ff; }
    40% { text-shadow: 2px -2px #7ee6b3; }
    60% { text-shadow: -2px 2px #ffd166; }
    80% { text-shadow: 2px 2px #b388ff; }
    100% { text-shadow: -2px -2px #ff8c42; }
  }

  .music-controls {
    position: fixed;
    bottom: 16px;
    right: 16px;
    z-index: 9999;
    display: flex;
    gap: 6px;
  }

  .music-controls button {
    margin: 2px;
    padding: 0.5em 1em;
    font-size: 0.95em;
    color: white;
    border: none;
    border-radius: 999px;
    cursor: pointer;
    background-color: var(--primary-color);
    transition: transform 0.2s, opacity 0.2s;
  }

  .music-controls button:first-child { background-color: var(--secondary-color); }
  .music-controls button:hover { opacity: 0.93; transform: translateY(-1px); }

  .audio-player {
    margin: 2rem 0 1rem 0;
    padding: 1rem;
    background-color: rgba(255,255,255,0.18);
    border-radius: 8px;
    max-width: 500px;
    margin-left: auto;
    margin-right: auto;
    border: 1px solid var(--border-color);
  }

  .audio-player audio { width: 100%; }
  .audio-title { font-weight: bold; margin-bottom: 0.5rem; color: var(--primary-color); }

  .dark-toggle { text-align: center; margin-top: 3rem; }
  .dark-toggle button {
    background: linear-gradient(90deg, #2f2a3b 0%, #433951 100%);
    color: #f8f2ff;
    border: none;
    padding: 0.6rem 1.2rem;
    border-radius: 999px;
    cursor: pointer;
    font-size: 1.1em;
    transition: transform 0.2s, box-shadow 0.2s;
    box-shadow: 0 4px 10px rgba(0,0,0,0.16);
  }

  .dark-toggle button:hover { transform: translateY(-1px); box-shadow: 0 6px 14px rgba(0,0,0,0.2); }

  .dark-mode {
    background: linear-gradient(135deg, #1b1424 0%, #261c33 50%, #132b35 100%);
    color: #f8f2ff;
  }

  .dark-mode .work-philosophy {
    background-color: #2d2238;
    border-color: rgba(255, 211, 232, 0.14);
    box-shadow: 0 6px 20px rgba(0, 0, 0, 0.28);
  }

  .dark-mode .principle-card {
    background-color: #352742;
    color: #f8f2ff;
    border-color: rgba(255, 211, 232, 0.14);
  }

  .dark-mode .highlight {
    background-color: rgba(179, 0, 89, 0.18);
  }

  .dark-mode .cta-button {
    background: linear-gradient(90deg, #cf2f78 0%, #ff7cac 100%);
  }

  .dark-mode a { color: #ffd3e8; }
  .dark-mode .hero-section { background: linear-gradient(90deg, #2d2238 0%, #1d3140 100%); }
  .dark-mode .audio-player { background-color: rgba(255,255,255,0.08); }
  .dark-mode .music-controls button { background-color: var(--primary-color); }
  .dark-mode .music-controls button:first-child { background-color: var(--secondary-color); }
  .dark-mode .mobius-spin { filter: brightness(1.15) hue-rotate(20deg); }
  .dark-mode svg ellipse { stroke: #ffd3e8; }
  .dark-mode svg circle { fill: #ffd3e8; }

  @media (max-width: 700px) {
    .hero-content h1 { font-size: 2em; }
    .work-philosophy { padding: 1.2rem 0.5rem; }
    .principles-grid { grid-template-columns: 1fr; }
    .music-controls { right: 8px; bottom: 8px; }
  }

  @media (max-width: 500px) {
    .hero-section { padding: 2em 0 1em 0; }
    .audio-player { padding: 0.5rem; }
  }

  /* Mobius Spinner Animation */
  @keyframes spin {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }

  .mobius-spin {
    animation: spin 5s linear infinite;
    display: block;
    margin: 0 auto;
  }

  /* Recent posts callout */
  .recent-posts.callout {
    max-width: 700px;
    margin: 1.25rem auto;
    padding: 1rem 1.25rem;
    background: linear-gradient(90deg, #fff4f8 0%, #f7fbff 100%);
    border-left: 6px solid var(--primary-color);
    border-radius: 10px;
    box-shadow: 0 6px 18px rgba(46, 35, 59, 0.08);
  }

  .recent-posts h2 {
    margin-top: 0;
    color: var(--primary-color);
    font-family: 'Montserrat', sans-serif;
  }

  .recent-posts ol { list-style: none; padding-left: 0; margin: 0; }
  .recent-posts li { margin: 0.75rem 0; padding: 0.6rem 0; border-bottom: 1px dashed rgba(0,0,0,0.06); }
  .recent-posts .post-link { font-weight: 600; color: var(--primary-color); text-decoration: none; }
  .recent-posts .post-link:hover { text-decoration: underline; color: var(--primary-strong); }
  .recent-posts .excerpt { margin: 0.25rem 0 0 0; color: var(--muted-text); font-size: 0.95em; }

  .dark-mode .recent-posts.callout {
    background: linear-gradient(90deg, #32263d 0%, #1f2734 100%);
    border-left-color: #ffd3e8;
  }

  .dark-mode .recent-posts .excerpt { color: #d8cfe0; }
  .post-icon { margin-right: 0.5rem; font-size: 1.15rem; display: inline-block; vertical-align: middle; }
  .badge { display: inline-block; margin-left: 0.6rem; background: var(--primary-color); color: white; font-weight: 700; font-size: 0.7rem; padding: 0.18rem 0.45rem; border-radius: 999px; vertical-align: middle; }
  .badge.new { background: var(--accent-color); color: #2e233b; box-shadow: 0 2px 8px rgba(242, 169, 59, 0.18); }
  .dark-mode .badge { background: #ff99cc; color: #2a2a3a; }
</style>













