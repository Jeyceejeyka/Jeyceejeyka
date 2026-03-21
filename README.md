<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jaafar · Full-Stack Engineer</title>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: transparent;
      font-family: 'Inter', sans-serif;
      color: #1a2c3e;
      line-height: 1.5;
      padding: 2rem 1.5rem;
    }

    /* Main container - no background, just transparent */
    .profile-container {
      max-width: 1200px;
      margin: 0 auto;
    }

    /* Banner Section */
    .banner-wrapper {
      width: 100%;
      height: 260px;
      overflow: hidden;
      border-radius: 28px;
      margin-bottom: 2rem;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.06);
    }
    .banner-wrapper img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
      display: block;
    }

    /* Clean card style - minimal, no background colors, just subtle borders */
    .clean-card {
      background: transparent;
      border: 1px solid #e9edf2;
      border-radius: 28px;
      padding: 2rem;
      margin-bottom: 2rem;
      transition: all 0.2s ease;
    }

    /* Section headers */
    .section-header {
      display: flex;
      align-items: center;
      gap: 0.75rem;
      margin-bottom: 1.75rem;
      border-bottom: 2px solid #eef2f6;
      padding-bottom: 0.75rem;
    }
    .section-header i {
      font-size: 1.6rem;
      color: #2c7da0;
    }
    .section-header h2 {
      font-size: 1.6rem;
      font-weight: 600;
      color: #1f4a6e;
      letter-spacing: -0.3px;
      margin: 0;
    }

    /* About section */
    .about-content {
      text-align: center;
      max-width: 780px;
      margin: 0 auto;
    }
    .greeting-badge {
      display: inline-block;
      background: #f5f7fa;
      padding: 0.3rem 1rem;
      border-radius: 40px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #2c7da0;
      margin-bottom: 1.2rem;
    }
    .name-title {
      font-size: 2.8rem;
      font-weight: 700;
      color: #1a2c3e;
      margin-bottom: 0.5rem;
      letter-spacing: -0.02em;
    }
    .role-tag {
      font-size: 1.1rem;
      color: #5a6e7e;
      margin-bottom: 1.5rem;
      font-weight: 450;
    }
    .bio-text {
      font-size: 1rem;
      line-height: 1.6;
      color: #2c3e4e;
      margin-bottom: 1rem;
    }
    .highlight {
      color: #2c7da0;
      font-weight: 600;
    }
    .signature {
      font-size: 1rem;
      font-weight: 500;
      color: #3b7c9e;
      margin-top: 1rem;
    }

    /* Social Links */
    .social-links {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin-top: 0.5rem;
    }
    .social-link {
      display: inline-flex;
      align-items: center;
      gap: 10px;
      padding: 0.6rem 1.4rem;
      border: 1px solid #e2e8f0;
      border-radius: 60px;
      text-decoration: none;
      color: #2c5a7a;
      font-weight: 500;
      font-size: 0.9rem;
      transition: all 0.2s;
      background: transparent;
    }
    .social-link i {
      font-size: 1.1rem;
    }
    .social-link:hover {
      border-color: #cbdde6;
      transform: translateY(-2px);
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.04);
    }

    /* Tech stack groups */
    .tech-group {
      margin-bottom: 1.8rem;
    }
    .tech-group-title {
      font-weight: 600;
      font-size: 1rem;
      color: #2c7da0;
      margin-bottom: 0.8rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }
    .tech-badge-list {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem;
    }
    .tech-badge {
      background: #f8fafc;
      border: 1px solid #e4e9ef;
      padding: 0.4rem 1rem;
      border-radius: 40px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #2c5f7a;
      transition: all 0.2s;
    }
    .tech-badge i {
      margin-right: 0.3rem;
      font-size: 0.75rem;
      color: #2c7da0;
    }
    .tech-badge:hover {
      background: #ffffff;
      border-color: #cbdbe0;
    }

    /* Stats grid - clean image cards */
    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 1.5rem;
      margin-bottom: 1.5rem;
    }
    .stat-card {
      border: 1px solid #eef2f8;
      border-radius: 24px;
      overflow: hidden;
      background: transparent;
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .stat-card:hover {
      transform: translateY(-3px);
      box-shadow: 0 12px 24px -12px rgba(0, 0, 0, 0.08);
    }
    .stat-card img {
      width: 100%;
      display: block;
    }

    .double-stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
      margin: 1.5rem 0;
    }
    .trophy-area {
      margin-top: 1.5rem;
    }
    .trophy-area img {
      width: 100%;
      border-radius: 20px;
    }

    /* Projects - clean minimal cards */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.8rem;
      margin-top: 1rem;
    }
    .project-item {
      border: 1px solid #eef2f6;
      border-radius: 24px;
      padding: 1.5rem;
      transition: all 0.2s;
      background: transparent;
    }
    .project-item:hover {
      border-color: #d4e0e8;
      transform: translateY(-4px);
    }
    .project-icon {
      font-size: 2rem;
      color: #2c7da0;
      margin-bottom: 1rem;
    }
    .project-title {
      font-size: 1.25rem;
      font-weight: 700;
      color: #1f4a6e;
      margin-bottom: 0.5rem;
    }
    .project-desc {
      font-size: 0.85rem;
      color: #5a6f82;
      line-height: 1.5;
      margin: 0.6rem 0;
    }
    .project-stack {
      display: inline-block;
      background: #f5f8fc;
      border: 1px solid #e6edf3;
      padding: 0.2rem 0.8rem;
      border-radius: 30px;
      font-size: 0.7rem;
      font-weight: 500;
      color: #2c7da0;
    }
    .project-link {
      margin-top: 1rem;
      display: inline-block;
      text-decoration: none;
      font-size: 0.85rem;
      font-weight: 500;
      color: #2c7da0;
    }
    .project-link i {
      font-size: 0.7rem;
      transition: transform 0.2s;
    }
    .project-link:hover i {
      transform: translateX(3px);
    }

    hr {
      margin: 2rem 0 1.5rem;
      border: 0;
      height: 1px;
      background: #e9edf2;
    }
    .footer {
      text-align: center;
      padding: 1rem 0;
    }
    .visit-badge {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 0.4rem 1.2rem;
      border: 1px solid #e2e8f0;
      border-radius: 40px;
      font-size: 0.8rem;
      color: #5a6e7e;
    }
    .footer-note {
      margin-top: 1rem;
      font-size: 0.7rem;
      color: #8ba0b0;
    }

    @media (max-width: 680px) {
      body { padding: 1rem; }
      .clean-card { padding: 1.2rem; }
      .name-title { font-size: 2rem; }
      .section-header h2 { font-size: 1.3rem; }
    }
  </style>
</head>
<body>
<div class="profile-container">
  
  <!-- Banner Image (exactly as original) -->
  <div class="banner-wrapper">
    <img src="git-banner2.png" alt="Header Banner" onerror="this.onerror=null; this.src='https://via.placeholder.com/1200x260/eef2f6/8ba0b0?text=Jaafar+·+Full+Stack+Engineer'">
  </div>

  <!-- About Me Section - Clean, no background -->
  <div class="clean-card">
    <div class="about-content">
      <div class="greeting-badge">
        <i class="fas fa-smile" style="margin-right: 4px;"></i> About Me
      </div>
      <h1 class="name-title">Jaafar Abdiwahid</h1>
      <div class="role-tag">Full-Stack Software Engineer · Creator · Problem Solver</div>
      <p class="bio-text">
        👋 Hi, I'm <span class="highlight">Jaafar</span>, a passionate Full-Stack Developer building scalable, 
        user-focused applications that blend performance with elegant design.
      </p>
      <p class="bio-text">
        Skilled in <span class="highlight">JavaScript, React, Next.js</span>, and <span class="highlight">Python ecosystems</span> — 
        I deliver clean, efficient code and intuitive user experiences.
      </p>
      <p class="signature">
        ✨ Let's build something extraordinary together.
      </p>
    </div>
  </div>

  <!-- Social Links Section -->
  <div class="clean-card">
    <div class="section-header">
      <i class="fas fa-share-alt"></i>
      <h2>Connect</h2>
    </div>
    <div class="social-links">
      <a href="https://www.linkedin.com/in/jaafar-abdiwahid/" target="_blank" class="social-link">
        <i class="fab fa-linkedin-in"></i> LinkedIn
      </a>
      <a href="mailto:jeyceejeyka635@gmail.com" class="social-link">
        <i class="fas fa-envelope"></i> Email
      </a>
      <a href="https://full-stack-portfolio-jade.vercel.app/" target="_blank" class="social-link">
        <i class="fas fa-globe"></i> Portfolio
      </a>
      <a href="https://github.com/Jeyceejeyka" target="_blank" class="social-link">
        <i class="fab fa-github"></i> GitHub
      </a>
    </div>
  </div>

  <!-- Tech Stack Section -->
  <div class="clean-card">
    <div class="section-header">
      <i class="fas fa-code"></i>
      <h2>Tech Stack</h2>
    </div>
    
    <div class="tech-group">
      <div class="tech-group-title"><i class="fas fa-paintbrush-fine"></i> Frontend</div>
      <div class="tech-badge-list">
        <span class="tech-badge"><i class="fab fa-react"></i> React</span>
        <span class="tech-badge"><i class="fab fa-js"></i> Next.js</span>
        <span class="tech-badge"><i class="fas fa-box"></i> Redux</span>
        <span class="tech-badge"><i class="fas fa-code-branch"></i> Redux-Saga</span>
        <span class="tech-badge"><i class="fab fa-js"></i> JavaScript</span>
        <span class="tech-badge"><i class="fas fa-terminal"></i> jQuery</span>
        <span class="tech-badge"><i class="fab fa-html5"></i> HTML5</span>
        <span class="tech-badge"><i class="fab fa-css3-alt"></i> CSS3</span>
        <span class="tech-badge"><i class="fab fa-sass"></i> SASS</span>
        <span class="tech-badge"><i class="fab fa-bootstrap"></i> Bootstrap</span>
        <span class="tech-badge"><i class="fas fa-wind"></i> TailwindCSS</span>
        <span class="tech-badge"><i class="fas fa-chart-line"></i> Chart.js</span>
      </div>
    </div>

    <div class="tech-group">
      <div class="tech-group-title"><i class="fas fa-server"></i> Backend & Databases</div>
      <div class="tech-badge-list">
        <span class="tech-badge"><i class="fas fa-flask"></i> Flask</span>
        <span class="tech-badge"><i class="fab fa-python"></i> Python</span>
        <span class="tech-badge"><i class="fas fa-database"></i> PostgreSQL</span>
        <span class="tech-badge"><i class="fas fa-table"></i> SQLAlchemy</span>
        <span class="tech-badge"><i class="fas fa-database"></i> SQLite</span>
        <span class="tech-badge"><i class="fas fa-lock"></i> JWT</span>
        <span class="tech-badge"><i class="fas fa-link"></i> REST API</span>
        <span class="tech-badge"><i class="fas fa-cloud-upload-alt"></i> Axios</span>
      </div>
    </div>

    <div class="tech-group">
      <div class="tech-group-title"><i class="fas fa-tools"></i> DevOps & Tools</div>
      <div class="tech-badge-list">
        <span class="tech-badge"><i class="fab fa-docker"></i> Docker</span>
        <span class="tech-badge"><i class="fas fa-sync-alt"></i> CI/CD</span>
        <span class="tech-badge"><i class="fab fa-git-alt"></i> Git/GitHub</span>
        <span class="tech-badge"><i class="fas fa-flask"></i> Postman</span>
        <span class="tech-badge"><i class="fas fa-code"></i> VS Code</span>
      </div>
    </div>

    <div class="tech-group">
      <div class="tech-group-title"><i class="fas fa-chart-line"></i> Upcoming</div>
      <div class="tech-badge-list">
        <span class="tech-badge"><i class="fas fa-brain"></i> Machine Learning</span>
        <span class="tech-badge"><i class="fas fa-chart-network"></i> TensorFlow</span>
      </div>
    </div>
  </div>

  <!-- GitHub Analytics Section -->
  <div class="clean-card">
    <div class="section-header">
      <i class="fab fa-github-alt"></i>
      <h2>GitHub Analytics</h2>
    </div>
    
    <div class="stats-grid">
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Jeyceejeyka&theme=default" alt="GitHub Profile Details">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Jeyceejeyka&theme=default" alt="Repos per language">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Jeyceejeyka&theme=default" alt="Most commit language">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Jeyceejeyka&theme=default" alt="GitHub Stats">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Jeyceejeyka&theme=default&utcOffset=0" alt="Productive time">
      </div>
    </div>

    <div class="double-stats">
      <div class="stat-card">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=Jeyceejeyka&theme=default&hide_border=true&background=FFFFFF&ring=2c7da0&fire=ffb347&currStreakNum=2c5f7a" alt="GitHub Streak">
      </div>
      <div class="stat-card">
        <img src="https://github-readme-activity-graph.vercel.app/graph?username=Jeyceejeyka&theme=minimal&bg_color=FFFFFF&color=2c5f7a&line=2c7da0&point=5f8b9f&hide_border=true" alt="Activity Graph">
      </div>
    </div>

    <div class="double-stats">
      <div class="stat-card">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jeyceejeyka&layout=compact&theme=default&hide_border=true&bg_color=FFFFFF&title_color=1f4a6e&text_color=2c5f7a" alt="Top Languages">
      </div>
      <div class="stat-card trophy-area">
        <img src="https://github-profile-trophy.vercel.app/?username=Jeyceejeyka&theme=flat&no-frame=true&no-bg=true&margin-w=8&row=2&column=4&title_color=2c7da0" alt="GitHub Trophies">
      </div>
    </div>
  </div>

  <!-- Featured Projects -->
  <div class="clean-card">
    <div class="section-header">
      <i class="fas fa-star"></i>
      <h2>Featured Projects</h2>
    </div>
    <div class="projects-grid">
      <div class="project-item">
        <div class="project-icon"><i class="fas fa-shopping-cart"></i></div>
        <div class="project-title">Elysian Market</div>
        <div class="project-desc">Full-stack e-commerce platform with secure user authentication, cart, and order management.</div>
        <span class="project-stack">React · Flask · PostgreSQL</span>
        <div><a href="https://github.com/Jeyceejeyka/project1" class="project-link">View project <i class="fas fa-arrow-right"></i></a></div>
      </div>
      <div class="project-item">
        <div class="project-icon"><i class="fas fa-comments"></i></div>
        <div class="project-title">Chroma Chat</div>
        <div class="project-desc">Real-time chat application with WebSockets, room support, and typing indicators.</div>
        <span class="project-stack">Next.js · Socket.io · TailwindCSS</span>
        <div><a href="https://github.com/Jeyceejeyka/project2" class="project-link">View project <i class="fas fa-arrow-right"></i></a></div>
      </div>
      <div class="project-item">
        <div class="project-icon"><i class="fas fa-chart-simple"></i></div>
        <div class="project-title">Insightify</div>
        <div class="project-desc">Data visualization dashboard for business analytics with interactive charts.</div>
        <span class="project-stack">React · Chart.js · Python</span>
        <div><a href="https://github.com/Jeyceejeyka/project3" class="project-link">View project <i class="fas fa-arrow-right"></i></a></div>
      </div>
    </div>
    <p style="text-align: center; margin-top: 1.5rem; font-size: 0.85rem;">
      <i class="fab fa-github"></i> Explore more on <a href="https://github.com/Jeyceejeyka" style="color:#2c7da0; text-decoration: none;">github.com/Jeyceejeyka</a>
    </p>
  </div>

  <!-- Footer -->
  <hr>
  <div class="footer">
    <div class="visit-badge">
      <i class="fas fa-eye"></i>
      <img src="https://visitcount.itsvg.in/api?id=Jeyceejeyka&icon=0&color=1" alt="visit counter" style="height: 18px;">
      <span>profile views</span>
    </div>
    <div class="footer-note">
      <i class="far fa-copyright"></i> Jaafar Abdiwahid · Full-Stack Engineer
    </div>
  </div>
</div>
</body>
</html>
