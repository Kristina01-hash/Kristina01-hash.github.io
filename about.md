---
layout: default
title: About
---
<!-- Theme Toggle UI -->

<div class="theme-container">
  <label for="theme-select">Theme:</label>
  <select id="theme-select" onchange="setTheme(this.value)">
    <option value="auto">Auto</option>
    <option value="light">Light</option>
    <option value="dark">Dark</option>
  </select>
  <span id="theme-status"></span>
</div>

<style>
body, .markdown-body {
  --bg: #fff;
  --fg: #222;
  --link: #007acc;
  --blockquote: #ff99cc;
  --accent: #6c5ce7;
  --muted: #888;
  --border: #e1e4e8;
  --section-spacing: 2rem;
  background: var(--bg);
  color: var(--fg);
  transition: background 0.2s, color 0.2s;
  line-height: 1.6;
}

body.dark-mode, .markdown-body.dark-mode {
  --bg: #181a1b;
  --fg: #eee;
  --link: #80bfff;
  --blockquote: #ffb3de;
  --accent: #a29bfe;
  --muted: #aaa;
  --border: #383838;
}

a { 
  color: var(--link); 
  text-decoration: none;
  border-bottom: 1px dotted;
  transition: all 0.2s ease;
}

a:hover {
  opacity: 0.8;
}

blockquote {
  color: var(--blockquote);
  border-left: 4px solid var(--blockquote);
  padding-left: 1rem;
  font-style: italic;
}

hr {
  border: 0;
  border-top: 1px solid var(--border);
  margin: var(--section-spacing) 0;
}

.theme-container {
  margin: 1.5em 0 2em 0; 
  display: flex; 
  align-items: center; 
  gap: 0.8em;
  padding: 0.8rem;
  background: rgba(0,0,0,0.03);
  border-radius: 6px;
}

body.dark-mode .theme-container {
  background: rgba(255,255,255,0.05);
}

.theme-container label {
  font-weight: bold;
}

.theme-container select {
  padding: 0.3em 0.8em;
  border-radius: 4px;
  border: 1px solid var(--border);
  background: var(--bg);
  color: var(--fg);
}

#theme-status {
  font-size: 0.9em;
  color: var(--muted);
}

.profile-container {
  display: flex;
  align-items: center;
  gap: 2rem;
  margin-bottom: var(--section-spacing);
}

.profile-image {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid var(--accent);
}

.profile-info h1 {
  margin-top: 0;
  margin-bottom: 0.5rem;
}

.profile-title {
  color: var(--muted);
  font-size: 1.1rem;
  margin-bottom: 1rem;
}

.badge-container {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  margin: var(--section-spacing) 0;
}

.badge {
  background: var(--accent);
  color: white;
  padding: 0.4rem 1rem;
  border-radius: 20px;
  font-size: 0.9rem;
  display: inline-block;
}

.card-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin: var(--section-spacing) 0;
}

.card {
  border: 1px solid var(--border);
  border-radius: 8px;
  padding: 1.5rem;
  transition: all 0.2s ease;
}

.card:hover {
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  transform: translateY(-3px);
}

body.dark-mode .card:hover {
  box-shadow: 0 5px 15px rgba(0,0,0,0.3);
}

.card h3 {
  margin-top: 0;
  color: var(--accent);
}

.highlight-box {
  background: rgba(108, 92, 231, 0.1);
  border-left: 4px solid var(--accent);
  padding: 1.5rem;
  margin: var(--section-spacing) 0;
  border-radius: 0 8px 8px 0;
}

body.dark-mode .highlight-box {
  background: rgba(162, 155, 254, 0.1);
}

.social-links {
  display: flex;
  gap: 1rem;
  margin-top: 1rem;
}

.social-link {
  color: var(--accent);
  border: none;
  font-weight: bold;
}

.cta-button {
  display: inline-block;
  background: var(--accent);
  color: white;
  padding: 0.8rem 1.5rem;
  border-radius: 4px;
  font-weight: bold;
  border: none;
  margin-top: 1rem;
  transition: all 0.2s ease;
}

.cta-button:hover {
  opacity: 0.9;
  transform: translateY(-2px);
}

.publication-list {
  margin: 2rem 0;
}

.publication-item {
  display: flex;
  margin-bottom: 1.5rem;
  padding-bottom: 1.5rem;
  border-bottom: 1px solid var(--border);
}

.pub-year {
  font-weight: bold;
  min-width: 60px;
  color: var(--accent);
  font-size: 1.1rem;
  padding-top: 0.2rem;
}

.pub-details {
  flex: 1;
}

.pub-title {
  font-weight: bold;
  margin: 0 0 0.3rem 0;
}

.pub-authors {
  margin: 0 0 0.3rem 0;
}

.pub-journal {
  margin: 0 0 0.5rem 0;
}

.pub-links {
  display: flex;
  gap: 10px;
}

.pub-links a {
  display: inline-flex;
  align-items: center;
  padding: 4px 12px;
  border-radius: 4px;
  font-size: 0.8rem;
  font-weight: bold;
  border: none;
  text-transform: uppercase;
}

.journal-link {
  background-color: var(--accent);
  color: white !important;
}

.code-link {
  background-color: #333;
  color: white !important;
}

body.dark-mode .code-link {
  background-color: #555;
}

.doi-link {
  background-color: #e67e22;
  color: white !important;
}
</style>

<script>
function setTheme(mode) {
  const root = document.body.classList;
  if (mode === 'dark') {
    root.add('dark-mode');
    localStorage.setItem('theme', 'dark');
    updateThemeStatus('Dark mode');
  } else if (mode === 'light') {
    root.remove('dark-mode');
    localStorage.setItem('theme', 'light');
    updateThemeStatus('Light mode');
  } else {
    localStorage.setItem('theme', 'auto');
    applyAutoTheme();
    updateThemeStatus('Auto (system)');
  }
}
function applyAutoTheme() {
  const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
  document.body.classList.toggle('dark-mode', prefersDark);
}
function updateThemeStatus(text) {
  var el = document.getElementById('theme-status');
  if (el) el.textContent = text;
}
(function() {
  const select = document.getElementById('theme-select');
  const saved = localStorage.getItem('theme') || 'auto';
  if (select) select.value = saved;
  if (saved === 'dark') {
    document.body.classList.add('dark-mode');
    updateThemeStatus('Dark mode');
  } else if (saved === 'light') {
    document.body.classList.remove('dark-mode');
    updateThemeStatus('Light mode');
  } else {
    applyAutoTheme();
    updateThemeStatus('Auto (system)');
  }
  window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', e => {
    if ((localStorage.getItem('theme') || 'auto') === 'auto') applyAutoTheme();
  });
})();
</script>

<div class="profile-container">
  <img src="https://Kristina01-hash.github.io/assets/images/IMG_0249.jpeg" alt="Kristina P. Sinaga" class="profile-image">
  <div class="profile-info">
    <h1>Kristina P. Sinaga</h1>
    <div class="profile-title">Ph.D. in Applied Mathematics, Chung Yuan Christian University (CYCU), Taiwan</div>
    <div class="social-links">
      <a href="https://github.com/Kristina01-hash" class="social-link">GitHub</a>
      <a href="www.linkedin.com/in/kristina-p-sinaga-0ba152309" class="social-link">LinkedIn</a>
      <a href="https://medium.com/@kristinapestaria.sinaga" class="social-link">Medium</a>
      <a href="https://scholar.google.com/citations?view_op=list_works&hl=it&hl=it&user=XoJ7EkoAAAAJ" class="social-link">Google Scholar</a>
    </div>
  </div>
</div> 

<blockquote class="quote">
  "A mind wired for patterns. A soul allergic to nonsense."
</blockquote>

## About Me

As an independent researcher, I specialize in applied mathematics, pattern recognition, machine learning, and federated learning. I facilitate the development of advancements at the intersection of academia and industry. I cultivated my expertise as a postdoctoral researcher at ISTI-CNR in Italy and the Department of Applied Mathematics at CYCU in Taiwan. I have a proven track record of developing innovative solutions that integrate theoretical research and practical applications, delivering tangible results in both fields. I speak my mind and mean what I say.

<div class="highlight-box">
  <h3>Research Interests</h3>
  <p>
   My research focuses on developing innovative algorithms for complex systems, with a particular emphasis on multi-view clustering, heat-kernel methods, and fuzzy clustering approaches in both centralized and decentralized environments. These methods are designed to deliver robust performance in unpredictable, real-world settings characterized by heterogeneous data sources. For instance, in domains such as autonomous systems and smart healthcare, where data can vary significantly in format and quality, my algorithms ensure reliable outcomes despite inherent uncertainties.
  </p>
</div>

## Specializations

<div class="badge-container">
  <span class="badge">Clustering Algorithms</span>
  <span class="badge">Supervised learning</span>
  <span class="badge">Deep learning</span>
  <span class="badge">Multi-view learning</span>
  <span class="badge">Fuzzy C-Means</span>
  <span class="badge">Heat-Kernel Methods</span>
  <span class="badge">Federated learning</span>
  <span class="badge">Edge AI</span>
</div>

I specialize in testing systems in unpredictable, real-world settings, where they are truly put to the test. My approach integrates theoretical rigor with hands-on experimentation to develop scalable, intelligent solutions that are durable and applicable in real-world settings. My research in the field of heat-kernel coefficients has resulted in the development of innovative clustering algorithms that demonstrate superior performance in comparison to conventional methods when dealing with heterogeneous data.

## Experience & Projects

<div class="card-container">
  <div class="card">
    <h3>Algorithm Design</h3>
    <p>
     The foundation of my work is the creation of scalable solutions that integrate theoretical rigor with practical utility. For the past decade, I have specialized in unsupervised learning, developing clustering algorithms that outperform traditional methods when handling diverse, multi-source data. This expertise provides a solid foundation for my current exploration into hybrid models that integrate unsupervised, supervised, and deep learning techniques. This transition signifies a paradigm shift, leveraging the strengths of deep learning to enhance efficiency and accuracy in complex data environments, such as real-time analytics in IoT systems or personalized recommendation engines.
    </p>
  </div>
  <div class="card">
    <h3>Robustness Research</h3>
    <p>
     A key aspect of this research involves adapting to modern computational tools. The transition from MATLAB to Python has been a substantial change in my workflow. It has given me greater flexibility and access to advanced libraries like TensorFlow and PyTorch. This shift is both straightforward and impactful. It begins with formulating core functions and progresses to leveraging Python's extensive ecosystem of libraries, streamlining algorithm development and deployment. Python's versatility allows for rapid prototyping in industry while maintaining the precision required for academic research. This research has broad implications. For academic institutions, it contributes to the advancement of theoretical understanding in the fields of clustering and learning paradigms. For industry, it offers practical, scalable solutions for data-driven decision-making in dynamic environments. For the general public, it paves the way for smarter, more reliable technologies that adapt to real-world complexities, from improved medical diagnostics to enhanced user experiences in digital platforms.
    </p>
  </div>
  <div class="card">
    <h3>NeuralGlow.ai</h3>
    <p>Founded a satirical AI lab blending humor, critique, and product design to challenge hype culture and reimagine intelligent systems.</p>
  </div>
</div>

## Recent Publications

<div style="text-align: center; margin-bottom: 2rem; padding: 1rem; background: rgba(255, 153, 204, 0.1); border-radius: 8px;">
  <p style="margin: 0; font-size: 1.1em;">
    <i class="fas fa-book"></i> Browse my <a href="https://kristinap09.github.io/publications.html" style="color: #ff99cc; font-weight: bold; border-bottom: 1px dotted;">complete publication list</a> with full citations and impact metrics
  </p>
</div>

<div class="publication-list">

<div class="publication-item">
    <span class="pub-year">2026</span>
    <div class="pub-details">
      <p class="pub-title"> Multi-View Clustering Goes Federated: A Survey</p>
      <p class="pub-authors">Sinaga, K.P.</p>
      <p class="pub-journal"><em>Qeios</em></p>
      <div class="pub-links">
        <a href="https://www.qeios.com/read/PC8X49" target="_blank" class="journal-link">Preprint</a>
      </div>
    </div>
    <span class="pub-year">2026</span>
    <div class="pub-details">
      <p class="pub-title">Personalized Federated Heat-Kernel Enhanced Multi-View Clustering via Advanced Tensor Decomposition Techniques (v4)</p>
      <p class="pub-authors">Sinaga, K.P.</p>
      <p class="pub-journal"><em>arXiv</em></p>
      <div class="pub-links">
        <a href="https://arxiv.org/abs/2509.16101" target="_blank" class="journal-link">Preprint</a>
      </div>
    </div>
  <span class="pub-year">2025</span>
    <div class="pub-details">
      <p class="pub-title">A Globally Collaborative Multi-View k-Means Clustering</p>
      <p class="pub-authors">Sinaga, K.P., Yang, M.S.</p>
      <p class="pub-journal"><em>MDPI Electronics</em></p>
      <div class="pub-links">
        <a href="https://arxiv.org/abs/2509.15844" target="_blank" class="journal-link">Journal</a>
        <a href="https://pypi.org/project/gcomvkm/" target="_blank" class="code-link">Code</a>
      </div>
    </div>
  <span class="pub-year">2025</span>
    <div class="pub-details">
      <p class="pub-title">FedHK-MVFC: Federated Heat Kernel Multi-View Clustering (v2)</p>
      <p class="pub-authors">Sinaga, K.P.</p>
      <p class="pub-journal"><em>arXiv</em></p>
      <div class="pub-links">
        <a href="https://arxiv.org/abs/2509.15844" target="_blank" class="journal-link">Preprint</a>
        <a href="https://ieee-dataport.org/documents/synthetic-multi-view-cardiovascular-dataset-federated-clustering" target="_blank" class="code-link">IEEE DataPort DOI</a>
        <a href="https://github.com/KristinaP09/FedHK-MVFC" target="_blank" class="code-link">Code</a>
      </div>
    </div>
   </div>

</div>

## Opportunities

<div class="highlight-box">
  <h3>Open to New Roles</h3>
  <p>I am seeking employment opportunities in the global job market, specifically in research-driven or applied roles within teams that value clarity, autonomy, and creative rigor. If you prioritize achieving tangible results and do not tolerate frivolous content, I invite you to initiate a dialogue.</p>
  <a href="mailto:kristinasinaga41@gmail.com" class="cta-button">Get in Touch</a>
</div>

## Contact

If you are interested in exploring collaboration or research opportunities, or if you simply wish to discuss intriguing problems in AI and mathematics, please do not hesitate to contact me.

- Email: kristinasinaga41@gmail.com
- Previous Affiliation: ISTI-CNR, Italy

---

<p style="text-align: center; color: var(--muted); font-size: 0.9em;">
© 2025 Kristina P. Sinaga | Last updated: July 2026
</p>
