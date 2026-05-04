---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.typewriter-wrapper {
  font-size: 1.2em;
  font-weight: 600;
  color: var(--global-link-color);
  margin-bottom: 1.2em;
  min-height: 1.6em;
}
#typewriter-cursor {
  display: inline-block;
  width: 2px;
  background-color: var(--global-link-color);
  animation: blink 0.7s step-end infinite;
  margin-left: 2px;
  vertical-align: text-bottom;
  height: 1.1em;
}
@keyframes blink { 50% { opacity: 0; } }


.stats-bar {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin: 1.5em 0;
}
.stat-item {
  flex: 1;
  min-width: 140px;
  background-color: var(--global-bg-color);
  border: 1px solid var(--global-border-color);
  border-radius: 8px;
  padding: 14px 18px;
  text-align: center;
}
.stat-number {
  display: block;
  font-size: 1.8em;
  font-weight: 700;
  color: var(--global-link-color);
  line-height: 1.1;
}
.stat-label {
  display: block;
  font-size: 0.78em;
  color: var(--global-text-color-light);
  margin-top: 4px;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.currently-at {
  display: inline-flex;
  align-items: center;
  gap: 10px;
  background-color: rgba(14, 161, 197, 0.12);
  border: 1px solid rgba(14, 161, 197, 0.4);
  border-radius: 8px;
  padding: 10px 16px;
  margin-bottom: 1.2em;
  font-size: 0.95em;
}
.currently-at .dot {
  width: 9px;
  height: 9px;
  border-radius: 50%;
  background-color: #2ecc71;
  flex-shrink: 0;
  box-shadow: 0 0 6px #2ecc71;
  animation: pulse 2s ease-in-out infinite;
}
@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.4; }
}
</style>

<div class="typewriter-wrapper">
  <span id="typewriter-text"></span><span id="typewriter-cursor"></span>
</div>

<script>
(function() {
  const titles = [
    "Software Engineer",
    "Oracle Developer",
    "Computer Vision Researcher",
    "Parallel Computing Enthusiast",
    "Full-Stack Developer"
  ];
  let titleIndex = 0, charIndex = 0, deleting = false;
  const el = document.getElementById('typewriter-text');

  function type() {
    const current = titles[titleIndex];
    if (deleting) {
      el.textContent = current.substring(0, --charIndex);
      if (charIndex === 0) { deleting = false; titleIndex = (titleIndex + 1) % titles.length; setTimeout(type, 400); return; }
      setTimeout(type, 50);
    } else {
      el.textContent = current.substring(0, ++charIndex);
      if (charIndex === current.length) { deleting = true; setTimeout(type, 1800); return; }
      setTimeout(type, 90);
    }
  }
  setTimeout(type, 500);
})();
</script>

<div class="currently-at">
  <span class="dot"></span>
  <span>Currently working as <strong>Oracle Developer</strong> at <strong>Diyar United Company</strong> — Kuwait City, Kuwait</span>
</div>

<a href="/files/Ahmad_Alkadi_Resume.pdf" class="btn btn--info" download><i class="fas fa-download"></i>&nbsp; Download Resume</a>

<div class="stats-bar">
  <div class="stat-item">
    <span class="stat-number">80+</span>
    <span class="stat-label">REST APIs Optimized</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">50+</span>
    <span class="stat-label">JAX-RS Endpoints</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">40%</span>
    <span class="stat-label">Lower RMS Error</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">3.88</span>
    <span class="stat-label">M.S. GPA</span>
  </div>
  <div class="stat-item">
    <span class="stat-number">100+</span>
    <span class="stat-label">Images Benchmarked</span>
  </div>
</div>

---

I'm a Software Engineer and M.S. Computer Science graduate with hands-on experience in full-stack development, system programming, and database integration. I currently work as an Oracle Developer at Diyar United Company in Kuwait, where I build and maintain REST APIs, manage Oracle EBS schemas, and develop integrations between mobile applications and Oracle HR systems using Java and PL/SQL.

My background spans a wide range of technical domains — from computer vision research (UAV image stitching with OpenCV and SIFT) to game development (2D Unity platformer in C#), parallel GPU programming with CUDA, and enterprise-level data pipelines. I'm comfortable working across the stack and stepping into whatever role a project needs.

I hold an M.S. in Computer Science (GPA: 3.88) from California Polytechnic State University Pomona, and a B.S. in Computer Science with Honors (GPA: 3.6) from California State University Dominguez Hills. I'm passionate about building reliable, impactful systems and continuously pushing what I can do with technology.

---

## GitHub Activity

<div style="margin-bottom: 1em;">
  <img src="https://ghchart.rshah.org/2ecc71/AhmadAlkadi" alt="Ahmad's GitHub Contribution Chart" style="width:100%; border-radius:6px;" />
</div>

<a href="https://github.com/AhmadAlkadi" class="btn btn--inverse" target="_blank"><i class="fab fa-github"></i>&nbsp; View GitHub Profile</a>
