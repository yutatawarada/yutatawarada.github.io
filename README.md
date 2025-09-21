<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Data Scientist — Portfolio</title>
<style>
:root{
  --blue-1:#3f51b5;   /* banner */
  --blue-2:#2f3fa8;   /* nav */
  --bg:#f6f7fb; --text:#222; --muted:#5f6368; --card:#fff;
  --max:980px; --pad-x:24px;
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial;
}
*{box-sizing:border-box} html,body{margin:0;background:var(--bg);color:var(--text);line-height:1.6}

/* layout */
.wrapper{max-width:var(--max);margin:0 auto;padding:0 var(--pad-x)}
.section{padding:28px 0}
.card{background:var(--card);border-radius:6px;box-shadow:0 1px 3px rgba(0,0,0,.08);padding:24px;margin:0 0 24px}
.card h2{margin:0 0 12px} .card h3{margin:16px 0 10px;color:#444} .muted{color:var(--muted)}

/* banner + nav */
.banner{background:var(--blue-1);color:#fff;padding:40px 0 16px}
.banner h1{margin:0;font-size:34px}
.banner p{margin:8px 0 0;opacity:.9}
.navbar{background:var(--blue-2);color:#fff}
.nav{display:flex;gap:28px;align-items:center;overflow-x:auto}
.nav a{color:#cfe0ff;text-decoration:none;font-weight:700;letter-spacing:.2px;padding:14px 0;border-bottom:3px solid transparent}
.nav a.active{color:#fff;border-color:#90a4ff}

/* home */
.hero{display:grid;grid-template-columns:1fr;gap:12px}
.hero h2{margin:0}
img.resp{max-width:100%;height:auto;border-radius:4px;box-shadow:0 1px 3px rgba(0,0,0,.08)}
ul,ol{margin:8px 0 0 20px}

/* responsive */
@media (min-width:760px){ .hero{grid-template-columns:1fr 360px} }

/* Hide github.com UI headers if someone views raw in repo (no effect on Pages) */
header.repohead,.gh-header,.application-main .pagehead{display:none!important}
</style>
</head>
<body>

<!-- Banner -->
<header class="banner">
  <div class="wrapper">
    <h1>Data Scientist</h1>
    <p class="muted">Python • SQL • AWS • Snowflake • MATLAB</p>
  </div>
</header>

<!-- Tabs -->
<nav class="navbar">
  <div class="wrapper">
    <div id="nav" class="nav">
      <a href="#home" data-route="home" class="active">HOME</a>
      <a href="#education" data-route="education">EDUCATION</a>
      <a href="#experience" data-route="experience">EXPERIENCE</a>
      <a href="#projects" data-route="projects">PROJECTS</a>
      <a href="#talks" data-route="talks">TALKS</a>
      <a href="#publications" data-route="publications">PUBLICATIONS</a>
    </div>
  </div>
</nav>

<!-- Pages -->
<main class="wrapper section">

  <!-- HOME -->
  <section id="page-home" class="page">
    <div class="card hero">
      <div>
        <h2>Hi — I’m a Data Scientist</h2>
        <p class="muted">I build production ML systems, improve data pipelines, and publish applied research.</p>
      </div>
    </div>
  </section>

  <!-- EDUCATION -->
  <section id="page-education" class="page" hidden>
    <div class="card">
      <h2>Education</h2>
      <ul>
        <li><strong>Ph.D., Physics</strong> — The University of Texas at Dallas <em>(May 2022)</em></li>
        <li><strong>M.S., Physics</strong> — The University of Texas at Dallas <em>(December 2019)</em></li>
        <li><strong>B.S., Physics</strong> — The University of Texas at Dallas <em>(May 2017)</em></li>
      </ul>
    </div>
  </section>

  <!-- EXPERIENCE -->
  <section id="page-experience" class="page" hidden>
    <div class="card">
      <h2>Toyota Financial Services — Data Scientist <span class="muted">(June 2022 – Present)</span></h2>
      <ul>
        <li>Uncovered and corrected missing step in production data pipeline which impacted over 70% of active accounts.</li>
        <li>Redeveloped loan originations model → ~50% performance lift; ~$1M potential losses avoided.</li>
      </ul>
    </div>
    <div class="card">
      <h2>Shawhin Talebi Ventures LLC — Data Science Consultant <span class="muted">(Dec 2020 – Present)</span></h2>
      <ul>
        <li>Data collection, processing, and analysis for study on 300+ biometrics in live-fire training performance.</li>
        <li>Unsupervised deep learning on longitudinal ICU data to discover sepsis sub-phenotypes.</li>
      </ul>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="page-projects" class="page" hidden>
    <div class="card">
      <h2>Data-Driven EEG Band Discovery with Decision Trees</h2>
      <p><a href="https://www.mdpi.com/1424-8220/22/8/3048" target="_blank" rel="noopener">Publication</a></p>
      <p>Objective strategy for discovering optimal EEG bands from power spectra using <strong>Python</strong>; identified bands that outperformed common boundaries by ~2×.</p>
      <img class="resp" src="/assets/img/eeg_band_discovery.jpeg" alt="EEG Band Discovery">
    </div>

    <div class="card">
      <h2>Decoding Physical & Cognitive Impacts of PM at Ultra-Fine Scales</h2>
      <p><a href="https://www.mdpi.com/1424-8220/22/11/4240" target="_blank" rel="noopener">Publication</a></p>
      <p>Trained 100+ ML models in <strong>MATLAB</strong> to estimate particulate matter from 300+ biometric variables (R²≈0.91); smaller particles estimated more accurately.</p>
      <img class="resp" src="/assets/img/bike_study.jpeg" alt="Bike Study">
    </div>
  </section>

  <!-- TALKS -->
  <section id="page-talks" class="page" hidden>
    <div class="card">
      <h2>Talks & Lectures</h2>
      <ul>
        <li>Causality: The new science of an old question — GSP Seminar, Fall 2021</li>
        <li>Guest Lecture: Dimensionality Reduction — PHYS 5336, Spring 2021</li>
        <li>Guest Lecture: Fourier and Wavelet Transforms — PHYS 5315, Fall 2020</li>
        <li>A Brief Introduction to Optimization — GSP Seminar, Fall 2019</li>
        <li>Weeks of Welcome Poster Competition — UTD, Fall 2019</li>
        <li>A Brief Introduction to Networks — GSP Seminar, Spring 2019</li>
      </ul>
      <p><a href="https://www.youtube.com/channel/UCa9gErQ9AE5jT2DZLjXBIdA" target="_blank" rel="noopener">Data Science YouTube</a></p>
    </div>
  </section>

  <!-- PUBLICATIONS -->
  <section id="page-publications" class="page" hidden>
    <div class="card">
      <h2>Publications</h2>
      <ol>
        <li>Talebi S., Lary D.J., Wijeratne L. O.H., Lary T. <em>Modeling Autonomic Pupillary Responses…</em> (2019). DOI: 10.26717/BJSTR.2019.20.003446</li>
        <li>Wijeratne, L.O.; Kiv, D.R.; Aker, A.R.; Talebi, S.; Lary, D.J. <em>Using Machine Learning for the Calibration of Airborne Particulate Sensors</em>. Sensors 2020, 20, 99.</li>
        <li>Lary, D.J. et al. <em>Autonomous Learning of New Environments…</em> Sensors 2021, 21, 2240. https://doi.org/10.3390/s21062240</li>
        <li>Zhang, Y.; Wijeratne, L.O.H.; Talebi, S.; Lary, D.J. <em>Machine Learning for Light Sensor Calibration</em>. Sensors 2021, 21, 6259.</li>
        <li>Talebi, S. et al. <em>Data-Driven EEG Band Discovery with Decision Trees</em>. Preprints 2022, 2022030145.</li>
        <li>Fernando, B.A. et al. <em>Unsupervised Blink Detection Using Eye Aspect Ratio Values</em>. Preprints 2022, 2022030200.</li>
        <li>Talebi, S. et al. <em>Decoding Physical and Cognitive Impacts of PM Concentrations…</em> Research Square, 2022.</li>
        <li>Lary, D.J. et al. <em>Machine Learning, Big Data, and Spatial Tools…</em> Springer, 2022.</li>
        <li>Wijerante, L.O.H. et al. <em>Advancement in Airborne Particulate Estimation Using Machine Learning</em>. Springer, 2022.</li>
      </ol>
      <p><a href="https://medium.com/@shawhin" target="_blank" rel="noopener">Data Science Blog</a></p>
    </div>
  </section>

</main>

<script>
/* tiny SPA router using hashes */
const routes = ["home","education","experience","projects","talks","publications"];
function show(route){
  document.querySelectorAll('.nav a').forEach(a=>{
    a.classList.toggle('active', a.dataset.route===route);
  });
  routes.forEach(r=>{
    const sec = document.getElementById('page-'+r);
    if(sec) sec.hidden = (r!==route);
  });
  window.scrollTo({top:0, behavior:"instant"});
}
function currentRoute(){
  const h = location.hash.replace('#','').toLowerCase();
  return routes.includes(h) ? h : 'home';
}
addEventListener('hashchange', ()=>show(currentRoute()));
addEventListener('DOMContentLoaded', ()=>show(currentRoute()));
</script>
</body>
</html>
