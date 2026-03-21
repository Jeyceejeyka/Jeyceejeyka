<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jaafar · Full-Stack Engineer</title>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
  <!-- Font Awesome 6 -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #ffffff;
      font-family: 'Inter', sans-serif;
      color: #1a2a3a;
      line-height: 1.5;
      padding: 2rem 1.5rem;
    }

    /* Main container - clean, no backgrounds */
    .profile-container {
      max-width: 1100px;
      margin: 0 auto;
    }

    /* Banner - preserve your image */
    .banner {
      width: 100%;
      height: 240px;
      overflow: hidden;
      border-radius: 24px;
      margin-bottom: 2rem;
    }
    .banner img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
      display: block;
    }

    /* Clean section dividers */
    .section {
      margin-bottom: 3rem;
    }

    .section-title {
      font-size: 1.5rem;
      font-weight: 600;
      letter-spacing: -0.02em;
      color: #11181c;
      margin-bottom: 1.5rem;
      padding-bottom: 0.5rem;
      border-bottom: 2px solid #e8edf2;
      display: inline-block;
    }

    /* About card - minimal, no background */
    .about-card {
      text-align: center;
      padding: 1rem 0 1.5rem 0;
    }
    .name {
      font-size: 2.8rem;
      font-weight: 700;
      letter-spacing: -0.02em;
      color: #0a1927;
      margin-bottom: 0.5rem;
    }
    .title {
      font-size: 1.1rem;
      font-weight: 500;
      color: #54708f;
      margin-bottom: 1.5rem;
    }
    .about-text {
      max-width: 700px;
      margin: 0 auto;
      font-size: 1rem;
      color: #2c3e42;
      line-height: 1.6;
    }
    .about-text p {
      margin-bottom: 0.75rem;
    }
    .highlight {
      font-weight: 600;
      color: #2c6e6e;
    }
    .signature {
      font-weight: 500;
      color: #5b8c8c;
      margin-top: 1rem;
    }

    /* Social links - minimal */
    .social-links {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin-top: 1rem;
    }
    .social-link {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.5rem 1.25rem;
      background: #f6f8fa;
      border-radius: 40px;
      text-decoration: none;
      font-size: 0.9rem;
      font-weight: 500;
      color: #2c5a6e;
      transition: all 0.2s ease;
      border: 1px solid #e2e8f0;
    }
    .social-link i {
      font-size: 1rem;
    }
    .social-link:hover {
      background: #edf2f7;
      border-color: #cbd5e1;
      transform: translateY(-1px);
    }

    /* Tech grid - clean badges */
    .tech-category {
      margin-bottom: 1.8rem;
    }
    .tech-category h3 {
      font-size: 1rem;
      font-weight: 600;
      color: #2c5a6e;
      margin-bottom: 0.75rem;
      letter-spacing: -0.2px;
    }
    .badge-group {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem;
    }
    .tech-badge {
      background: #f5f7f9;
      padding: 0.35rem 1rem;
      border-radius: 30px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #2c5a6e;
      border: 1px solid #e9edf2;
      transition: all 0.2s;
    }
    .tech-badge i {
      margin-right: 6px;
      font-size: 0.75rem;
      color: #5f8b9e;
    }
    .tech-badge:hover {
      background: #eef2f6;
      border-color: #d0dce6;
    }

    /* Stats grid - clean cards with subtle border */
    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.2rem;
      margin-bottom: 1.2rem;
    }
    .stat-item {
      border: 1px solid #eef2f6;
      border-radius: 20px;
      padding: 0.8rem;
      background: transparent;
      transition: all 0.2s;
    }
    .stat-item img {
      width: 100%;
      border-radius: 16px;
      display: block;
    }
    .double-stats {
      display: flex;
      flex-wrap: wrap;
      gap: 1.2rem;
      margin-top: 1.2rem;
    }
    .double-stats > * {
      flex: 1;
      min-width: 240px;
    }

    /* Projects - clean cards */
    .projects-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1.5rem;
      margin-top: 0.5rem;
    }
    .project-card {
      flex: 1 1 280px;
      border: 1px solid #eef2f6;
      border-radius: 20px;
      padding: 1.5rem;
      transition: all 0.25s;
      background: transparent;
    }
    .project-card:hover {
      border-color: #d4e0e8;
      transform: translateY(-3px);
    }
    .project-icon {
      font-size: 1.8rem;
      color: #5f8b9e;
      margin-bottom: 1rem;
    }
    .project-title {
      font-size: 1.2rem;
      font-weight: 600;
      margin-bottom: 0.5rem;
      color: #1f3b44;
    }
    .project-desc {
      font-size: 0.85rem;
      color: #5a6f7a;
      margin: 0.6rem 0;
      line-height: 1.45;
    }
    .project-stack {
      font-size: 0.7rem;
      font-weight: 500;
      background: #f5f7f9;
      display: inline-block;
      padding: 0.2rem 0.8rem;
      border-radius: 20px;
      color: #4c6f82;
      letter-spacing: -0.2px;
    }
    .project-link {
      margin-top: 1rem;
      display: inline-block;
      font-size: 0.8rem;
      font-weight: 500;
      color: #5f8b9e;
      text-decoration: none;
    }
    .project-link i {
      font-size: 0.7rem;
      margin-left: 4px;
    }

    /* Upcoming skills */
    .upcoming-badge {
      background: #f5f7f9;
      border: 1px solid #e9edf2;
      padding: 0.35rem 1rem;
      border-radius: 30px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #2c5a6e;
      display: inline-flex;
      align-items: center;
      gap: 8px;
    }

    /* Footer */
    .footer {
      text-align: center;
      margin-top: 3rem;
      padding-top: 1.5rem;
      border-top: 1px solid #eef2f6;
      font-size: 0.75rem;
      color: #8aa0ae;
    }
    .visit-count {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      background: #f8fafc;
      padding: 0.3rem 1rem;
      border-radius: 40px;
      font-size: 0.75rem;
      border: 1px solid #eef2f6;
    }

    hr {
      margin: 1.5rem 0;
      border: none;
      border-top: 1px solid #eef2f6;
    }

    @media (max-width: 680px) {
      body { padding: 1.2rem; }
      .name { font-size: 2rem; }
    }
  </style>
</head>
<body>
<div class="profile-container">

  <!-- Banner Section - your original image preserved -->
  <div class="banner">
    <img src="git-banner2.png" alt="Header Banner" onerror="this.onerror=null; this.src='https://placehold.co/1200x300/f8fafc/8ba0ae?text=Jaafar+·+Full+Stack'">
  </div>

  <!-- About Section - clean, no background -->
  <div class="section">
    <div class="about-card">
      <h1 class="name">Jaafar Abdiwahid</h1>
      <div class="title">Full-Stack Software Engineer · Creative Developer</div>
      <div class="about-text">
        <p>👋 Hi, I'm <span class="highlight">Jaafar</span>, a passionate Full-Stack Engineer building scalable, user-focused applications with clean code and thoughtful design.</p>
        <p>Skilled in <span class="highlight">JavaScript, React, Next.js</span>, and <span class="highlight">Python ecosystems</span> — I deliver efficient backend systems and intuitive frontend experiences.</p>
        <p class="signature">✨ Let's build something extraordinary together.</p>
      </div>
    </div>
  </div>

  <!-- Social Links -->
  <div class="section">
    <div class="social-links">
      <a href="https://www.linkedin.com/in/jaafar-abdiwahid/" target="_blank" class="social-link"><i class="fab fa-linkedin-in"></i> LinkedIn</a>
      <a href="mailto:jeyceejeyka635@gmail.com" class="social-link"><i class="fas fa-envelope"></i> Email</a>
      <a href="https://full-stack-portfolio-jade.vercel.app/" target="_blank" class="social-link"><i class="fas fa-globe"></i> Portfolio</a>
      <a href="https://github.com/Jeyceejeyka" target="_blank" class="social-link"><i class="fab fa-github"></i> GitHub</a>
    </div>
  </div>

  <!-- Tech Stack Section - minimal badges -->
  <div class="section">
    <h2 class="section-title">Tech Stack</h2>
    
    <div class="tech-category">
      <h3>Frontend</h3>
      <div class="badge-group">
        <span class="tech-badge"><i class="fab fa-react"></i> React</span>
        <span class="tech-badge"><i class="fab fa-js"></i> Next.js</span>
        <span class="tech-badge"><i class="fas fa-layer-group"></i> Redux</span>
        <span class="tech-badge"><i class="fas fa-code-branch"></i> Redux-Saga</span>
        <span class="tech-badge"><i class="fab fa-js"></i> JavaScript (ES6+)</span>
        <span class="tech-badge"><i class="fas fa-code"></i> jQuery</span>
        <span class="tech-badge"><i class="fab fa-html5"></i> HTML5/CSS3</span>
        <span class="tech-badge"><i class="fab fa-sass"></i> SASS</span>
        <span class="tech-badge"><i class="fab fa-bootstrap"></i> Bootstrap</span>
        <span class="tech-badge"><i class="fas fa-wind"></i> TailwindCSS</span>
        <span class="tech-badge"><i class="fas fa-chart-line"></i> Chart.js</span>
      </div>
    </div>

    <div class="tech-category">
      <h3>Backend & Databases</h3>
      <div class="badge-group">
        <span class="tech-badge"><i class="fas fa-flask"></i> Flask</span>
        <span class="tech-badge"><i class="fab fa-python"></i> Python</span>
        <span class="tech-badge"><i class="fas fa-database"></i> PostgreSQL</span>
        <span class="tech-badge"><i class="fas fa-database"></i> SQLAlchemy</span>
        <span class="tech-badge"><i class="fas fa-database"></i> SQLite</span>
        <span class="tech-badge"><i class="fas fa-key"></i> JWT</span>
        <span class="tech-badge"><i class="fas fa-cloud-upload-alt"></i> REST API</span>
        <span class="tech-badge"><i class="fas fa-exchange-alt"></i> Axios</span>
      </div>
    </div>

    <div class="tech-category">
      <h3>DevOps & Tools</h3>
      <div class="badge-group">
        <span class="tech-badge"><i class="fab fa-docker"></i> Docker</span>
        <span class="tech-badge"><i class="fas fa-sync-alt"></i> CI/CD</span>
        <span class="tech-badge"><i class="fab fa-git-alt"></i> Git/GitHub</span>
        <span class="tech-badge"><i class="fas fa-flask"></i> Postman</span>
        <span class="tech-badge"><i class="fas fa-code"></i> VS Code</span>
      </div>
    </div>

    <div class="tech-category">
      <h3>📚 Upcoming Skills</h3>
      <div class="badge-group">
        <span class="upcoming-badge"><i class="fas fa-brain"></i> Machine Learning</span>
        <span class="upcoming-badge"><i class="fas fa-chart-network"></i> TensorFlow</span>
      </div>
    </div>
  </div>

  <!-- GitHub Analytics - clean, transparent cards -->
  <div class="section">
    <h2 class="section-title">GitHub Analytics</h2>
    <div class="stats-grid">
      <div class="stat-item">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Jeyceejeyka&theme=default" alt="profile details">
      </div>
      <div class="stat-item">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Jeyceejeyka&theme=default" alt="repos per language">
      </div>
      <div class="stat-item">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Jeyceejeyka&theme=default" alt="most commit language">
      </div>
      <div class="stat-item">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Jeyceejeyka&theme=default" alt="stats">
      </div>
      <div class="stat-item">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Jeyceejeyka&theme=default&utcOffset=0" alt="productive time">
      </div>
    </div>

    <div class="double-stats">
      <div class="stat-item">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=Jeyceejeyka&theme=default&hide_border=true&background=FFFFFF&stroke=E2E8F0&ring=5f8b9e&fire=CC9966" alt="streak stats">
      </div>
      <div class="stat-item">
        <img src="https://github-readme-activity-graph.vercel.app/graph?username=Jeyceejeyka&theme=minimal&bg_color=ffffff&color=3b6e8b&line=5f8b9e&point=8aaec2&area=true&hide_border=true" alt="activity graph">
      </div>
    </div>

    <div class="double-stats">
      <div class="stat-item">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jeyceejeyka&layout=compact&theme=default&hide_border=true&bg_color=ffffff&title_color=2c5a6e&text_color=4a6f82" alt="top languages">
      </div>
      <div class="stat-item">
        <img src="https://github-profile-trophy.vercel.app/?username=Jeyceejeyka&theme=flat&no-frame=true&no-bg=true&margin-w=8&row=2&column=4&title_color=5f8b9e" alt="trophy case">
      </div>
    </div>
  </div>

  <!-- Featured Projects -->
  <div class="section">
    <h2 class="section-title">Featured Projects</h2>
    <div class="projects-grid">
      <div class="project-card">
        <div class="project-icon"><i class="fas fa-shopping-cart"></i></div>
        <div class="project-title">Elysian Market</div>
        <div class="project-desc">Full-stack e-commerce platform with user auth, cart system, and order tracking.</div>
        <span class="project-stack">React · Flask · PostgreSQL</span>
        <div><a href="https://github.com/Jeyceejeyka/project1" class="project-link">View project <i class="fas fa-arrow-right"></i></a></div>
      </div>
      <div class="project-card">
        <div class="project-icon"><i class="fas fa-comments"></i></div>
        <div class="project-title">Chroma Chat</div>
        <div class="project-desc">Real-time chat application with rooms, typing indicators, and WebSocket connection.</div>
        <span class="project-stack">Next.js · Socket.io · Tailwind</span>
        <div><a href="https://github.com/Jeyceejeyka/project2" class="project-link">View project <i class="fas fa-arrow-right"></i></a></div>
      </div>
      <div class="project-card">
        <div class="project-icon"><i class="fas fa-chart-simple"></i></div>
        <div class="project-title">Insightify</div>
        <div class="project-desc">Interactive data visualization dashboard for analytics and business metrics.</div>
        <span class="project-stack">React · Chart.js · Python</span>
        <div><a href="https://github.com/Jeyceejeyka/project3" class="project-link">View project <i class="fas fa-arrow-right"></i></a></div>
      </div>
    </div>
  </div>

  <!-- Footer with visit counter -->
  <div class="footer">
    <div class="visit-count">
      <i class="fas fa-eye"></i>
      <img src="https://visitcount.itsvg.in/api?id=Jeyceejeyka&icon=0&color=1" alt="visit counter" style="height: 18px; vertical-align: middle;">
      <span>profile views</span>
    </div>
    <div style="margin-top: 1rem;">✧ built with clarity & purpose ✧</div>
  </div>

</div>
</body>
</html>
