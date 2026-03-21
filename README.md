<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Jaafar · Full-Stack Engineer | Glassmorphism Portfolio</title>
  <style>
    /* minimal global reset for consistency — only inline styles are used, but this ensures cross-browser */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      background: radial-gradient(circle at 10% 30%, #0b1120, #030617);
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
      padding: 2rem 1.5rem;
    }
    /* smooth scrolling & container */
    .readme-container {
      max-width: 1400px;
      margin: 0 auto;
    }
    /* glass card utility (inline styles used but fallback) */
    a {
      text-decoration: none;
    }
    /* responsive grid helpers */
    @media (max-width: 640px) {
      body {
        padding: 1rem;
      }
    }
  </style>
</head>
<body>
<div class="readme-container">

  <!-- 1. BANNER (glassmorphism infused: rounded + semi-transparent overlay effect) -->
  <div style="position: relative; width: 100%; border-radius: 28px; overflow: hidden; margin-bottom: 2rem; box-shadow: 0 20px 35px -12px rgba(0,0,0,0.4);">
    <div style="position: relative; width: 100%; height: 260px; background: linear-gradient(105deg, #0f1a2f 0%, #07121f 100%); overflow: hidden;">
      <img src="git-banner2.png" 
           alt="Header Banner" 
           style="width: 100%; height: 100%; object-fit: cover; object-position: center 30%; opacity: 0.85; mix-blend-mode: overlay;">
      <div style="position: absolute; inset: 0; background: radial-gradient(ellipse at 30% 40%, rgba(56,189,248,0.08), rgba(0,0,0,0.4)); backdrop-filter: blur(2px);"></div>
    </div>
  </div>

  <!-- 2. ABOUT ME – glass card (center aligned, glassmorphism) -->
  <div style="max-width: 1100px; margin: 0 auto 2.5rem auto; background: rgba(15, 25, 45, 0.55); backdrop-filter: blur(14px); border-radius: 32px; border: 1px solid rgba(255,255,255,0.2); box-shadow: 0 18px 35px -12px rgba(0,0,0,0.3); padding: 2rem 2rem; transition: transform 0.2s ease, border-color 0.2s;">
    <div style="text-align: center;">
      <h1 style="font-size: 2.5rem; font-weight: 700; background: linear-gradient(135deg, #90e0ff, #5dade2); -webkit-background-clip: text; background-clip: text; color: transparent; letter-spacing: -0.01em; margin-bottom: 1.25rem;">💫 About Me</h1>
      <p style="font-size: 1.25rem; font-weight: 500; color: #eef5ff; line-height: 1.6; margin-bottom: 1.25rem;">
        👋 Hi, I’m <span style="color:#FACC15; font-weight: 700;">Jaafar</span>, a passionate 
        <span style="color:#FACC15; font-weight: 700;">Full-Stack Software Engineer | Developer</span> 
        building scalable, user-focused applications.
      </p>
      <p style="font-size: 1.2rem; font-weight: 500; color: #e0edff; line-height: 1.6; margin-bottom: 1.5rem;">
        Skilled in <span style="color:#34d399; font-weight:600;">JavaScript, React</span>, 
        <span style="color:#f472b6; font-weight:600;">Next.js</span>, and 
        <span style="color:#a78bfa; font-weight:600;">Python + Libraries</span> — I deliver clean, efficient code and intuitive user experiences.
      </p>
      <p style="font-size: 1.3rem; font-weight: 600; color: #facc15; background: rgba(250,204,21,0.08); display: inline-block; padding: 0.5rem 1.2rem; border-radius: 60px; backdrop-filter: blur(2px);">
        ✨ Let’s build something extraordinary together.
      </p>
    </div>
  </div>

  <!-- 3. SOCIAL LINKS (glass card with inline badge row) -->
  <div style="max-width: 700px; margin: 0 auto 2.5rem auto; background: rgba(20, 30, 55, 0.5); backdrop-filter: blur(12px); border-radius: 40px; border: 1px solid rgba(255,255,255,0.2); padding: 1.25rem 1.8rem; text-align: center; transition: all 0.2s;">
    <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 1rem; align-items: center;">
      <a href="https://www.linkedin.com/in/jaafar-abdiwahid/" target="_blank" style="display: inline-flex; transition: transform 0.2s ease;">
        <img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white&style=for-the-badge" alt="LinkedIn" style="border-radius: 12px; box-shadow: 0 4px 8px rgba(0,0,0,0.2);">
      </a>
      <a href="mailto:jeyceejeyka635@gmail.com" target="_blank" style="display: inline-flex; transition: transform 0.2s ease;">
        <img src="https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white&style=for-the-badge" alt="Email" style="border-radius: 12px;">
      </a>
      <a href="https://full-stack-portfolio-jade.vercel.app/" target="_blank" style="display: inline-flex; transition: transform 0.2s ease;">
        <img src="https://img.shields.io/badge/Portfolio-%23000000.svg?logo=react&logoColor=white&style=for-the-badge" alt="Portfolio" style="border-radius: 12px;">
      </a>
    </div>
  </div>

  <!-- 4. TECH STACK (grid cards - Frontend, Backend, DevOps, Upcoming) -->
  <div style="margin: 3rem 0 2rem;">
    <div style="text-align: center; margin-bottom: 2rem;">
      <h2 style="font-size: 2rem; font-weight: 700; color: #cbd5ff; letter-spacing: -0.3px; background: linear-gradient(120deg, #e2e8ff, #a5b4fc); -webkit-background-clip: text; background-clip: text; color: transparent;">💻 Tech Stack</h2>
    </div>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 1.8rem;">
      
      <!-- Frontend Card -->
      <div style="background: rgba(15, 25, 45, 0.55); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.15); padding: 1.5rem; transition: all 0.25s ease; box-shadow: 0 12px 28px -10px rgba(0,0,0,0.25);">
        <h3 style="font-size: 1.55rem; font-weight: 600; margin-bottom: 1.2rem; color: #facc15; border-left: 4px solid #38bdf8; padding-left: 12px;">✨ Frontend</h3>
        <div style="display: flex; flex-wrap: wrap; gap: 10px; align-items: center;">
          <img src="https://img.shields.io/badge/React-20232a?style=for-the-badge&logo=react&logoColor=61DAFB" />
          <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" />
          <img src="https://img.shields.io/badge/Redux-764ABC?style=for-the-badge&logo=redux&logoColor=white" />
          <img src="https://img.shields.io/badge/Redux--Saga-999999?style=for-the-badge&logo=redux-saga&logoColor=white" />
          <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
          <img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white" />
          <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
          <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
          <img src="https://img.shields.io/badge/SASS-hotpink.svg?style=for-the-badge&logo=SASS&logoColor=white" />
          <img src="https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white" />
          <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
          <img src="https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chart.js&logoColor=white" />
        </div>
      </div>

      <!-- Backend Card -->
      <div style="background: rgba(15, 25, 45, 0.55); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.15); padding: 1.5rem; transition: all 0.25s ease; box-shadow: 0 12px 28px -10px rgba(0,0,0,0.25);">
        <h3 style="font-size: 1.55rem; font-weight: 600; margin-bottom: 1.2rem; color: #86efac; border-left: 4px solid #34d399; padding-left: 12px;">⚙️ Backend</h3>
        <div style="display: flex; flex-wrap: wrap; gap: 10px;">
          <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
          <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
          <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
          <img src="https://img.shields.io/badge/SQL_ORM-4479A1?style=for-the-badge" />
          <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
          <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens" />
          <img src="https://img.shields.io/badge/REST_API-FF6C37?style=for-the-badge" />
          <img src="https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white" />
        </div>
      </div>

      <!-- DevOps & Tools Card -->
      <div style="background: rgba(15, 25, 45, 0.55); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.15); padding: 1.5rem; transition: all 0.25s ease; box-shadow: 0 12px 28px -10px rgba(0,0,0,0.25);">
        <h3 style="font-size: 1.55rem; font-weight: 600; margin-bottom: 1.2rem; color: #90e0ff; border-left: 4px solid #38bdf8; padding-left: 12px;">🛠️ DevOps & Tools</h3>
        <div style="display: flex; flex-wrap: wrap; gap: 10px;">
          <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
          <img src="https://img.shields.io/badge/CI/CD-2088FF?style=for-the-badge&logo=github-actions&logoColor=white" />
          <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
          <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github" />
          <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" />
          <img src="https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white" />
        </div>
      </div>

      <!-- Upcoming Skills Card -->
      <div style="background: rgba(15, 25, 45, 0.55); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.15); padding: 1.5rem; transition: all 0.25s ease; box-shadow: 0 12px 28px -10px rgba(0,0,0,0.25);">
        <h3 style="font-size: 1.55rem; font-weight: 600; margin-bottom: 1.2rem; color: #fdba74; border-left: 4px solid #f97316; padding-left: 12px;">📈 Upcoming Skills</h3>
        <div style="display: flex; flex-wrap: wrap; gap: 10px;">
          <img src="https://img.shields.io/badge/Machine_Learning-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
          <span style="background: rgba(255,255,255,0.1); padding: 0.3rem 1rem; border-radius: 40px; color: #cbd5e6; font-weight: 500; font-size: 0.9rem;">LLM integration</span>
          <span style="background: rgba(255,255,255,0.1); padding: 0.3rem 1rem; border-radius: 40px; color: #cbd5e6; font-weight: 500;">AWS</span>
        </div>
      </div>
    </div>
  </div>

  <!-- 5. GITHUB ANALYTICS (stacked glass cards, grid layout for metrics) -->
  <div style="margin: 2rem 0 3rem;">
    <div style="text-align: center; margin-bottom: 2rem;">
      <h2 style="font-size: 2rem; font-weight: 700; background: linear-gradient(135deg,#c084fc,#38bdf8); -webkit-background-clip: text; background-clip: text; color: transparent;">📊 GitHub Analytics</h2>
    </div>
    
    <!-- Grid for analytics cards (2+ columns) -->
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 1.8rem;">
      
      <!-- Profile details card -->
      <div style="background: rgba(10, 20, 40, 0.5); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.2rem; transition: transform 0.2s;">
        <h3 style="color:#e2e8f0; margin-bottom: 1rem; font-weight: 600;">📌 Profile Overview</h3>
        <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Jeyceejeyka&theme=github_dark" style="width:100%; border-radius: 20px; box-shadow: 0 8px 20px rgba(0,0,0,0.3);" alt="profile details">
      </div>
      
      <!-- Activity + languages dual card using internal flex -->
      <div style="background: rgba(10, 20, 40, 0.5); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.2rem;">
        <div style="display: flex; flex-direction: column; gap: 1rem;">
          <div><h3 style="color:#e2e8f0; margin-bottom: 0.6rem;">⚡ Commit Languages</h3><img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Jeyceejeyka&theme=github_dark" style="width:100%; border-radius: 18px;"></div>
          <div><h3 style="color:#e2e8f0; margin-bottom: 0.6rem;">📚 Repos per Language</h3><img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Jeyceejeyka&theme=github_dark" style="width:100%; border-radius: 18px;"></div>
        </div>
      </div>
      
      <!-- stats + productive time -->
      <div style="background: rgba(10, 20, 40, 0.5); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.2rem;">
        <div style="display: flex; flex-direction: column; gap: 1rem;">
          <div><h3 style="color:#e2e8f0;">📈 GitHub Stats</h3><img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Jeyceejeyka&theme=github_dark" style="width:100%; border-radius: 18px;"></div>
          <div><h3 style="color:#e2e8f0;">⏰ Productive Time</h3><img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=Jeyceejeyka&theme=github_dark" style="width:100%; border-radius: 18px;"></div>
        </div>
      </div>
    </div>

    <!-- Streak & Contribution section full width glass card -->
    <div style="margin-top: 2rem; display: grid; grid-template-columns: repeat(auto-fit, minmax(340px, 1fr)); gap: 1.8rem;">
      <div style="background: rgba(10, 20, 40, 0.5); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.2rem; text-align: center;">
        <h3 style="color:#facc15; margin-bottom: 0.8rem;">🔥 Streak Stats</h3>
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=Jeyceejeyka&theme=github-dark&hide_border=true" style="width:100%; border-radius: 20px;">
      </div>
      <div style="background: rgba(10, 20, 40, 0.5); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.2rem;">
        <h3 style="color:#facc15; margin-bottom: 0.8rem;">📈 Contribution Graph</h3>
        <img src="https://github-readme-activity-graph.vercel.app/graph?username=Jeyceejeyka&theme=github-dark&hide_border=true&area=true" style="width:100%; border-radius: 20px;">
      </div>
    </div>

    <!-- Top Languages + Trophies Row -->
    <div style="margin-top: 2rem; display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 1.8rem;">
      <div style="background: rgba(10, 20, 40, 0.5); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.2rem;">
        <h3 style="color:#90e0ff; margin-bottom: 0.8rem;">🏆 Top Languages</h3>
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jeyceejeyka&layout=compact&theme=github_dark&hide_border=true" style="width:100%; border-radius: 20px;">
      </div>
      <div style="background: rgba(10, 20, 40, 0.5); backdrop-filter: blur(12px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.2rem;">
        <h3 style="color:#90e0ff; margin-bottom: 0.8rem;">🏅 Trophy Case</h3>
        <img src="https://github-profile-trophy.vercel.app/?username=Jeyceejeyka&theme=onedark&no-frame=true&no-bg=true&margin-w=4&row=2&column=4" style="width:100%; border-radius: 20px;">
      </div>
    </div>
  </div>

  <!-- 6. FEATURED PROJECTS (glass cards grid, no tables) -->
  <div style="margin: 2rem 0 2.5rem;">
    <div style="text-align: center; margin-bottom: 2rem;">
      <h2 style="font-size: 2rem; font-weight: 700; background: linear-gradient(120deg,#a78bfa,#facc15); -webkit-background-clip: text; background-clip: text; color: transparent;">🚀 Featured Projects</h2>
    </div>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem;">
      
      <!-- Project Card 1 -->
      <div style="background: rgba(20, 30, 55, 0.6); backdrop-filter: blur(14px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.6rem; transition: all 0.25s ease; box-shadow: 0 15px 30px -12px rgba(0,0,0,0.4);">
        <h3 style="font-size: 1.7rem; font-weight: 700; color: #facc15; margin-bottom: 0.5rem;">🛒 E‑commerce Platform</h3>
        <p style="color: #cbd5f0; margin: 0.8rem 0; line-height: 1.5;">Full-stack e-commerce platform with secure user authentication, cart management, and order processing.</p>
        <div style="display: flex; flex-wrap: wrap; gap: 8px; margin: 1rem 0 1.2rem;">
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px; font-size: 0.8rem; color:#90e0ff;">React</span>
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px; font-size: 0.8rem; color:#90e0ff;">Flask</span>
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px; font-size: 0.8rem; color:#90e0ff;">PostgreSQL</span>
        </div>
        <a href="https://github.com/Jeyceejeyka/project1" target="_blank" style="display: inline-block; background: rgba(255,255,255,0.1); border: 1px solid rgba(255,215,0,0.5); border-radius: 60px; padding: 0.45rem 1.3rem; color:#ffdf7e; font-weight: 500; transition: 0.2s;">🔗 View Project →</a>
      </div>
      
      <!-- Project Card 2 -->
      <div style="background: rgba(20, 30, 55, 0.6); backdrop-filter: blur(14px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.6rem; transition: all 0.25s ease;">
        <h3 style="font-size: 1.7rem; font-weight: 700; color: #facc15; margin-bottom: 0.5rem;">💬 Real‑time Chat</h3>
        <p style="color: #cbd5f0; margin: 0.8rem 0; line-height: 1.5;">Real-time chat application with WebSockets, private rooms, and responsive modern design.</p>
        <div style="display: flex; flex-wrap: wrap; gap: 8px; margin: 1rem 0 1.2rem;">
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px;">Next.js</span>
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px;">Socket.io</span>
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px;">TailwindCSS</span>
        </div>
        <a href="https://github.com/Jeyceejeyka/project2" target="_blank" style="display: inline-block; background: rgba(255,255,255,0.1); border: 1px solid rgba(255,215,0,0.5); border-radius: 60px; padding: 0.45rem 1.3rem; color:#ffdf7e; font-weight: 500;">🔗 View Project →</a>
      </div>
      
      <!-- Project Card 3 -->
      <div style="background: rgba(20, 30, 55, 0.6); backdrop-filter: blur(14px); border-radius: 28px; border: 1px solid rgba(255,255,255,0.2); padding: 1.6rem; transition: all 0.25s ease;">
        <h3 style="font-size: 1.7rem; font-weight: 700; color: #facc15; margin-bottom: 0.5rem;">📊 Data Viz Dashboard</h3>
        <p style="color: #cbd5f0; margin: 0.8rem 0; line-height: 1.5;">Interactive analytics dashboard with dynamic charts and real-time data visualization.</p>
        <div style="display: flex; flex-wrap: wrap; gap: 8px; margin: 1rem 0 1.2rem;">
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px;">React</span>
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px;">Chart.js</span>
          <span style="background: rgba(56,189,248,0.2); padding: 0.2rem 0.7rem; border-radius: 30px;">Python</span>
        </div>
        <a href="https://github.com/Jeyceejeyka/project3" target="_blank" style="display: inline-block; background: rgba(255,255,255,0.1); border: 1px solid rgba(255,215,0,0.5); border-radius: 60px; padding: 0.45rem 1.3rem; color:#ffdf7e; font-weight: 500;">🔗 View Project →</a>
      </div>
    </div>
  </div>

  <!-- 7. FOOTER (minimal glass style) -->
  <div style="margin-top: 3rem; text-align: center; background: rgba(8, 12, 25, 0.5); backdrop-filter: blur(10px); border-radius: 48px; border: 1px solid rgba(255,255,255,0.1); padding: 1rem 1.5rem; max-width: 500px; margin-left: auto; margin-right: auto;">
    <div style="display: flex; justify-content: center; gap: 0.6rem; flex-wrap: wrap; align-items: center;">
      <img src="https://visitcount.itsvg.in/api?id=Jeyceejeyka&icon=0&color=0" alt="visit counter" style="border-radius: 20px;">
      <span style="color:#b9c8ff; font-size: 0.85rem;">✨ Jaafar · Full‑Stack Architect</span>
    </div>
    <p style="color:#8190b0; font-size: 0.75rem; margin-top: 0.6rem;">Glassmorphism portfolio · modern grid layout</p>
  </div>

</div>
</body>
</html>
