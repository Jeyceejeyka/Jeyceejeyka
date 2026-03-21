<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jaafar · Full-Stack Engineer | GitHub Profile</title>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <!-- Font Awesome 6 -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
      background: #ffffff;
      color: #1e293b;
      line-height: 1.5;
      padding: 2rem 1.5rem;
    }

    /* Main container */
    .readme-container {
      max-width: 1000px;
      margin: 0 auto;
    }

    /* Banner */
    .banner {
      width: 100%;
      height: 200px;
      overflow: hidden;
      border-radius: 24px;
      margin-bottom: 2rem;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
    }
    .banner img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
      display: block;
    }

    /* Section styling */
    .section {
      margin-bottom: 2.5rem;
    }
    
    .section-title {
      font-size: 1.75rem;
      font-weight: 700;
      letter-spacing: -0.02em;
      margin-bottom: 1.25rem;
      display: flex;
      align-items: center;
      gap: 0.75rem;
      border-bottom: 2px solid #eef2ff;
      padding-bottom: 0.5rem;
    }
    .section-title i {
      color: #3b82f6;
      font-size: 1.5rem;
    }

    /* About card */
    .about-card {
      background: #fafcff;
      border: 1px solid #eef2f6;
      border-radius: 24px;
      padding: 2rem;
      text-align: center;
    }
    .name {
      font-size: 2.5rem;
      font-weight: 800;
      background: linear-gradient(135deg, #1e293b, #3b82f6);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      margin-bottom: 0.5rem;
    }
    .tagline {
      font-size: 1.1rem;
      color: #4b5563;
      margin-bottom: 1.5rem;
      font-weight: 500;
    }
    .bio {
      max-width: 700px;
      margin: 0 auto;
      color: #334155;
      line-height: 1.6;
    }
    .bio p {
      margin-bottom: 0.75rem;
    }
    .highlight {
      color: #3b82f6;
      font-weight: 600;
    }
    .emoji-text {
      margin-top: 1rem;
      font-weight: 500;
      color: #3b82f6;
    }

    /* Social links */
    .social-grid {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
      margin-top: 0.5rem;
    }
    .social-btn {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.6rem 1.25rem;
      background: #f8fafc;
      border: 1px solid #e2e8f0;
      border-radius: 40px;
      text-decoration: none;
      color: #1e293b;
      font-weight: 500;
      font-size: 0.9rem;
      transition: all 0.2s ease;
    }
    .social-btn i {
      font-size: 1rem;
      color: #3b82f6;
    }
    .social-btn:hover {
      border-color: #3b82f6;
      transform: translateY(-2px);
      box-shadow: 0 4px 12px rgba(59,130,246,0.1);
    }

    /* Tech stack groups */
    .tech-group {
      margin-bottom: 1.5rem;
    }
    .tech-group-header {
      font-weight: 600;
      font-size: 1rem;
      margin-bottom: 0.75rem;
      color: #3b82f6;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }
    .badge-container {
      display: flex;
      flex-wrap: wrap;
      gap: 0.6rem;
    }
    .tech-badge {
      background: #f8fafc;
      border: 1px solid #e2e8f0;
      padding: 0.35rem 1rem;
      border-radius: 30px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #1e293b;
      transition: all 0.2s;
    }
    .tech-badge i {
      margin-right: 0.3rem;
      font-size: 0.75rem;
      color: #3b82f6;
    }
    .tech-badge:hover {
      border-color: #3b82f6;
      background: #ffffff;
    }

    /* Stats cards grid */
    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.25rem;
      margin-bottom: 1.25rem;
    }
    .stat-card {
      background: #fafcff;
      border: 1px solid #eef2f6;
      border-radius: 20px;
      overflow: hidden;
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .stat-card:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
    }
    .stat-card img {
      width: 100%;
      display: block;
    }

    .double-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.25rem;
      margin: 1.25rem 0;
    }

    /* Projects */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 1.5rem;
      margin-top: 0.5rem;
    }
    .project-card {
      background: #fafcff;
      border: 1px solid #eef2f6;
      border-radius: 20px;
      padding: 1.5rem;
      transition: all 0.2s;
    }
    .project-card:hover {
      border-color: #cbd5e1;
      transform: translateY(-3px);
    }
    .project-icon {
      font-size: 1.8rem;
      color: #3b82f6;
      margin-bottom: 0.75rem;
    }
    .project-name {
      font-size: 1.2rem;
      font-weight: 700;
      margin-bottom: 0.5rem;
      color: #0f172a;
    }
    .project-desc {
      font-size: 0.85rem;
      color: #475569;
      line-height: 1.5;
      margin: 0.5rem 0;
    }
    .project-stack {
      display: inline-block;
      background: #f1f5f9;
      padding: 0.2rem 0.8rem;
      border-radius: 20px;
      font-size: 0.7rem;
      font-weight: 500;
      color: #3b82f6;
      margin-top: 0.5rem;
    }
    .project-link {
      display: inline-block;
      margin-top: 1rem;
      text-decoration: none;
      font-size: 0.8rem;
      font-weight: 500;
      color: #3b82f6;
    }
    .project-link i {
      font-size: 0.7rem;
      transition: transform 0.2s;
    }
    .project-link:hover i {
      transform: translateX(3px);
    }

    /* Footer */
    hr {
      margin: 2rem 0 1rem;
      border: 0;
      height: 1px;
      background: #eef2f6;
    }
    .footer {
      text-align: center;
      padding: 1rem 0;
    }
    .visit-count {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.4rem 1.2rem;
      background: #f8fafc;
      border: 1px solid #e2e8f0;
      border-radius: 40px;
      font-size: 0.8rem;
      color: #475569;
    }
    .credit {
      margin-top: 1rem;
      font-size: 0.7rem;
      color: #94a3b8;
    }

    @media (max-width: 640px) {
      body { padding: 1rem; }
      .about-card { padding: 1.25rem; }
      .name { font-size: 1.8rem; }
      .section-title { font-size: 1.4rem; }
    }
  </style>
</head>
<body>
<div class="readme-container">
  
  <!-- Banner Image -->
  <div class="banner">
    <img src="git-banner2.png" alt="Jaafar Banner" onerror="this.onerror=null; this.src='https://placehold.co/1200x200/eef2ff/3b82f6?text=Jaafar+·+Full+Stack+Engineer'">
  </div>

  <!-- About Section -->
  <div class="section">
    <div class="about-card">
      <h1 class="name">Jaafar Abdiwahid</h1>
      <div class="tagline">
        <i class="fas fa-code"></i> Full-Stack Software Engineer
      </div>
      <div class="bio">
        <p>👋 Hi, I'm <span class="highlight">Jaafar</span>, a passionate Full-Stack Developer building scalable, user-focused applications that blend performance with elegant design.</p>
        <p>Skilled in <span class="highlight">JavaScript, React, Next.js</span>, and <span class="highlight">Python ecosystems</span> — I deliver clean, efficient code and intuitive user experiences.</p>
        <div class="emoji-text">✨ Let's build something extraordinary together.</div>
      </div>
    </div>
  </div>

  <!-- Social Links -->
  <div class="section">
    <div class="section-title">
      <i class="fas fa-share-alt"></i>
      <span>Connect</span>
    </div>
    <div class="social-grid">
      <a href="https://www.linkedin.com/in/jaafar-abdiwahid/" target="_blank" class="social-btn">
        <i class="fab fa-linkedin-in"></i> LinkedIn
      </a>
      <a href="mailto:jeyceejeyka635@gmail.com" class="social-btn">
        <i class="fas fa-envelope"></i> Email
      </a>
      <a href="https://full-stack-portfolio-jade.vercel.app/" target="_blank" class="social-btn">
        <i class="fas fa-globe"></i> Portfolio
      </a>
      <a href="https://github.com/Jeyceejeyka" target="_blank" class="social-btn">
        <i class="fab fa-github"></i> GitHub
      </a>
    </div>
  </div>

  <!-- Tech Stack -->
  <div class="section">
    <div class="section-title">
      <i class="fas fa-layer-group"></i>
      <span>Tech Stack</span>
    </div>
    
    <div class="tech-group">
      <div class="tech-group-header"><i class="fas fa-palette"></i> Frontend</div>
      <div class="badge-container">
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
      <div class="tech-group-header"><i class="fas fa-server"></i> Backend & Databases</div>
      <div class="badge-container">
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
      <div class="tech-group-header"><i class="fas fa-tools"></i> DevOps & Tools</div>
      <div class="badge-container">
        <span class="tech-badge"><i class="fab fa-docker"></i> Docker</span>
        <span class="tech-badge"><i class="fas fa-sync-alt"></i> CI/CD</span>
        <span class="tech-badge"><i class="fab fa-git-alt"></i> Git/GitHub</span>
        <span class="tech-badge"><i class="fas fa-flask"></i> Postman</span>
        <span class="tech-badge"><i class="fas fa-code"></i> VS Code</span>
      </div>
    </div>

    <div class="tech-group">
      <div class="tech-group-header"><i class="fas fa-chart-line"></i> Learning Next</div>
      <div class="badge-container">
        <span class="tech-badge"><i class="fas fa-brain"></i> Machine Learning</span>
        <span class="tech-badge"><i class="fas fa-chart-network"></i> TensorFlow</span>
      </div>
    </div>
  </div>

  <!-- GitHub Analytics -->
  <div class="section">
    <div class="section-title">
      <i class="fab fa-github-alt"></i>
      <span>GitHub Analytics</span>
    </div>
    
    <div class="stats-grid">
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Jeyceejeyka&theme=default" alt="Profile Details">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Jeyceejeyka&theme=default" alt="Repos per Language">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Jeyceejeyka&theme=default" alt="Most Commit Language">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Jeyceejeyka&theme=default" alt="GitHub Stats">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Jeyceejeyka&theme=default&utcOffset=0" alt="Productive Time">
      </div>
    </div>

    <div class="double-grid">
      <div class="stat-card">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=Jeyceejeyka&theme=default&hide_border=true&background=FFFFFF&ring=3b82f6&fire=f97316&currStreakNum=1e293b" alt="GitHub Streak">
      </div>
      <div class="stat-card">
        <img src="https://github-readme-activity-graph.vercel.app/graph?username=Jeyceejeyka&theme=minimal&bg_color=FFFFFF&color=3b82f6&line=3b82f6&point=94a3b8&hide_border=true" alt="Activity Graph">
      </div>
    </div>

    <div class="double-grid">
      <div class="stat-card">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jeyceejeyka&layout=compact&theme=default&hide_border=true&bg_color=FFFFFF&title_color=3b82f6&text_color=475569" alt="Top Languages">
      </div>
      <div class="stat-card">
        <img src="https://github-profile-trophy.vercel.app/?username=Jeyceejeyka&theme=flat&no-frame=true&no-bg=true&margin-w=8&row=2&column=4&title_color=3b82f6" alt="GitHub Trophies">
      </div>
    </div>
  </div>

  <!-- Featured Projects -->
  <div class="section">
    <div class="section-title">
      <i class="fas fa-star"></i>
      <span>Featured Projects</span>
    </div>
    <div class="projects-grid">
      <div class="project-card">
        <div class="project-icon"><i class="fas fa-shopping-cart"></i></div>
        <div class="project-name">Elysian Market</div>
        <div class="project-desc">Full-stack e-commerce platform with secure authentication, cart system, and order management.</div>
        <span class="project-stack">React · Flask · PostgreSQL</span>
        <div><a href="https://github.com/Jeyceejeyka/project1" class="project-link">Explore <i class="fas fa-arrow-right"></i></a></div>
      </div>
      <div class="project-card">
        <div class="project-icon"><i class="fas fa-comments"></i></div>
        <div class="project-name">Chroma Chat</div>
        <div class="project-desc">Real-time messaging application with WebSockets, room support, and typing indicators.</div>
        <span class="project-stack">Next.js · Socket.io · TailwindCSS</span>
        <div><a href="https://github.com/Jeyceejeyka/project2" class="project-link">Explore <i class="fas fa-arrow-right"></i></a></div>
      </div>
      <div class="project-card">
        <div class="project-icon"><i class="fas fa-chart-simple"></i></div>
        <div class="project-name">Insightify</div>
        <div class="project-desc">Interactive data visualization dashboard for business analytics with dynamic charts.</div>
        <span class="project-stack">React · Chart.js · Python</span>
        <div><a href="https://github.com/Jeyceejeyka/project3" class="project-link">Explore <i class="fas fa-arrow-right"></i></a></div>
      </div>
    </div>
    <div style="text-align: center; margin-top: 1.5rem;">
      <a href="https://github.com/Jeyceejeyka?tab=repositories" style="color: #3b82f6; text-decoration: none; font-size: 0.9rem;">
        <i class="fab fa-github"></i> View all repositories →
      </a>
    </div>
  </div>

  <!-- Footer -->
  <hr>
  <div class="footer">
    <div class="visit-count">
      <i class="fas fa-eye"></i>
      <img src="https://visitcount.itsvg.in/api?id=Jeyceejeyka&icon=0&color=1" alt="Profile Views" style="height: 18px;">
      <span>visitors</span>
    </div>
    <div class="credit">
      <i class="far fa-copyright"></i> Jaafar Abdiwahid · Full-Stack Software Engineer
    </div>
  </div>
</div>
</body>
</html>
