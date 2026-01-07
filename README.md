<!-- 
  ===============================================
  🚀 JAMSHIDBEK - PREMIUM GITHUB PROFILE README
  ===============================================
  Created: 2024
  Version: 3.0
  Features: Animated, Interactive, Analytics
  ===============================================
-->

<style>
  /* Premium Animations */
  @keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-10px); }
  }
  
  @keyframes glow {
    0%, 100% { box-shadow: 0 0 10px #00FF88; }
    50% { box-shadow: 0 0 25px #00FF88; }
  }
  
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  @keyframes typing {
    from { width: 0 }
    to { width: 100% }
  }
  
  @keyframes blink-caret {
    from, to { border-color: transparent }
    50% { border-color: #00FF88; }
  }
  
  .animate-float { animation: float 3s ease-in-out infinite; }
  .animate-glow { animation: glow 2s ease-in-out infinite; }
  .animate-fade { animation: fadeIn 1s ease-out; }
  
  /* Custom Styles */
  .header-wave {
    border-radius: 20px;
    margin-bottom: 30px;
    overflow: hidden;
  }
  
  .tech-badge:hover {
    animation: float 0.5s ease, glow 1s ease;
    transform: scale(1.1);
  }
  
  .stats-card {
    border-radius: 15px;
    padding: 20px;
    margin: 10px;
    background: rgba(0, 255, 136, 0.05);
    border: 2px solid rgba(0, 255, 136, 0.2);
    transition: all 0.3s ease;
  }
  
  .stats-card:hover {
    background: rgba(0, 255, 136, 0.1);
    border-color: #00FF88;
    transform: translateY(-5px);
  }
</style>

<!-- ===================== HEADER SECTION ===================== -->
<div align="center" class="header-wave">

<!-- Animated Typing Text -->
<div style="position: relative; padding: 20px;">
  <h1 style="font-size: 2.5rem; margin-bottom: 10px;">
    <span style="color: #00FF88;">❯</span> 
    <span id="typed-text" style="
      font-family: 'Fira Code', monospace;
      color: #00FF88;
      border-right: 3px solid;
      padding-right: 5px;
      white-space: nowrap;
      overflow: hidden;
      display: inline-block;
    ">Hello World! I'm Jamshidbek</span>
  </h1>
  
  <p style="color: #888; font-size: 1.2rem; margin-top: 10px;">
    🚀 Python Backend Developer | 💡 FastAPI & Django Specialist | 🎯 Problem Solver
  </p>
</div>

<script>
  // Typing animation script
  const texts = [
    "Hello World! I'm Jamshidbek",
    "Python Backend Developer 🚀",
    "FastAPI & Django Specialist 💡",
    "Open Source Enthusiast 🌟",
    "Problem Solver 🎯"
  ];
  
  let textIndex = 0;
  let charIndex = 0;
  let isDeleting = false;
  const speed = 100;
  const elem = document.getElementById('typed-text');
  
  function typeWriter() {
    const currentText = texts[textIndex];
    
    if (!isDeleting && charIndex < currentText.length) {
      elem.textContent = currentText.substring(0, charIndex + 1);
      charIndex++;
      setTimeout(typeWriter, speed);
    } else if (isDeleting && charIndex > 0) {
      elem.textContent = currentText.substring(0, charIndex - 1);
      charIndex--;
      setTimeout(typeWriter, speed / 2);
    } else {
      isDeleting = !isDeleting;
      if (!isDeleting) {
        textIndex = (textIndex + 1) % texts.length;
      }
      setTimeout(typeWriter, isDeleting ? 1200 : 500);
    }
  }
  
  window.onload = typeWriter;
</script>

<!-- Animated Badges -->
<div align="center" style="margin: 20px 0;">
  <img src="https://komarev.com/ghpvc/?username=Jamshidbekpy&label=👁️%20Profile%20Views&color=00FF88&style=for-the-badge" alt="Profile Views" class="animate-glow" />
  <img src="https://img.shields.io/github/followers/Jamshidbekpy?label=👥%20Followers&style=for-the-badge&color=00FF88" alt="Followers" />
  <img src="https://img.shields.io/github/stars/Jamshidbekpy?label=⭐%20Stars&style=for-the-badge&color=FFD700" alt="Stars" />
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=120&section=header&animation=fadeIn&fontAlignY=40" />

</div>

<!-- ===================== STATS SECTION ===================== -->
<div align="center">

<h2 style="color: #00FF88; margin: 30px 0 20px 0;">
  📊 <span style="border-bottom: 2px solid #00FF88; padding-bottom: 5px;">GitHub Analytics</span>
</h2>

<div style="display: flex; justify-content: center; flex-wrap: wrap; gap: 20px;">

<!-- Stats Card 1 -->
<div class="stats-card animate-fade" style="flex: 1; min-width: 300px;">
  <img height="160em" src="https://github-readme-stats.vercel.app/api?username=Jamshidbekpy&show_icons=true&theme=dark&hide_border=true&bg_color=0D1117&title_color=00FF88&icon_color=00FF88&text_color=FFFFFF&include_all_commits=true&count_private=true" alt="GitHub Stats" />
</div>

<!-- Stats Card 2 -->
<div class="stats-card animate-fade" style="flex: 1; min-width: 300px;">
  <img height="160em" src="https://github-readme-streak-stats.herokuapp.com/?user=Jamshidbekpy&theme=dark&hide_border=true&background=0D1117&stroke=00FF88&ring=00FF88&fire=FF6B6B&currStreakLabel=FFFFFF" alt="GitHub Streak" />
</div>

<!-- Stats Card 3 -->
<div class="stats-card animate-fade" style="flex: 1; min-width: 300px;">
  <img height="160em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Jamshidbekpy&layout=compact&theme=dark&hide_border=true&bg_color=0D1117&title_color=00FF88&text_color=FFFFFF&langs_count=8" alt="Top Languages" />
</div>

</div>

</div>

<!-- ===================== TECH STACK ===================== -->
<div align="center">

<h2 style="color: #00FF88; margin: 40px 0 20px 0;">
  🛠️ <span style="border-bottom: 2px solid #00FF88; padding-bottom: 5px;">Tech Stack</span>
</h2>

<!-- Programming Languages -->
<h3 style="color: #FFF; margin: 15px 0;">💻 Programming Languages</h3>
<p>
  <img src="https://skillicons.dev/icons?i=python" alt="Python" title="Python" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=javascript" alt="JavaScript" title="JavaScript" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=html" alt="HTML" title="HTML" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=css" alt="CSS" title="CSS" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=cpp" alt="C++" title="C++" class="tech-badge" style="height: 50px; margin: 5px;" />
</p>

<!-- Frameworks -->
<h3 style="color: #FFF; margin: 15px 0;">🚀 Frameworks & Libraries</h3>
<p>
  <img src="https://skillicons.dev/icons?i=fastapi" alt="FastAPI" title="FastAPI" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=django" alt="Django" title="Django" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=flask" alt="Flask" title="Flask" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=nodejs" alt="Node.js" title="Node.js" class="tech-badge" style="height: 50px; margin: 5px;" />
</p>

<!-- Databases -->
<h3 style="color: #FFF; margin: 15px 0;">🗄️ Databases</h3>
<p>
  <img src="https://skillicons.dev/icons?i=postgres" alt="PostgreSQL" title="PostgreSQL" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=mysql" alt="MySQL" title="MySQL" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=mongodb" alt="MongoDB" title="MongoDB" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=redis" alt="Redis" title="Redis" class="tech-badge" style="height: 50px; margin: 5px;" />
</p>

<!-- Tools -->
<h3 style="color: #FFF; margin: 15px 0;">🔧 Tools & DevOps</h3>
<p>
  <img src="https://skillicons.dev/icons?i=docker" alt="Docker" title="Docker" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=git" alt="Git" title="Git" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=linux" alt="Linux" title="Linux" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=nginx" alt="Nginx" title="Nginx" class="tech-badge" style="height: 50px; margin: 5px;" />
  <img src="https://skillicons.dev/icons?i=postman" alt="Postman" title="Postman" class="tech-badge" style="height: 50px; margin: 5px;" />
</p>

</div>

<!-- ===================== ACTIVITY GRAPH ===================== -->
<div align="center">

<h2 style="color: #00FF88; margin: 40px 0 20px 0;">
  📈 <span style="border-bottom: 2px solid #00FF88; padding-bottom: 5px;">Coding Activity</span>
</h2>

<!-- WakaTime Stats -->
<a href="https://wakatime.com/@Jamshidbekpy" target="_blank">
  <img src="https://wakatime.com/badge/user/YOUR_WAKATIME_ID.svg?style=for-the-badge&color=00FF88" alt="WakaTime" />
</a>

<br><br>

<!-- GitHub Activity Graph -->
<img src="https://github-readme-activity-graph.vercel.app/graph?username=Jamshidbekpy&theme=github-dark&bg_color=0D1117&hide_border=true&color=00FF88&line=00FF88&point=FFFFFF&area=true&area_color=00FF88&title_color=FFFFFF" alt="Activity Graph" style="width: 90%; max-width: 1000px; border-radius: 15px;" />

</div>

<!-- ===================== ABOUT ME ===================== -->
<div align="center">

<h2 style="color: #00FF88; margin: 40px 0 20px 0;">
  👨‍💻 <span style="border-bottom: 2px solid #00FF88; padding-bottom: 5px;">About Me</span>
</h2>

<div style="max-width: 800px; margin: 0 auto; text-align: left; padding: 20px; background: rgba(0, 255, 136, 0.05); border-radius: 15px; border: 2px solid rgba(0, 255, 136, 0.2);">

```python
class Jamshidbek:
    
    def __init__(self):
        self.name = "Jamshidbek"
        self.role = "Backend Developer"
        self.location = "Uzbekistan"
        self.focus = "High-Performance APIs"
        self.passion = "Systems Architecture"
        
    @property
    def skills(self):
        return {
            "backend": ["FastAPI", "Django", "Flask", "DRF"],
            "databases": ["PostgreSQL", "MySQL", "MongoDB", "Redis"],
            "devops": ["Docker", "Nginx", "Linux", "Git"],
            "message_brokers": ["RabbitMQ", "Celery"]
        }
    
    def current_learning(self):
        return ["System Design", "Microservices", "Kubernetes", "AWS"]
    
    def contact(self):
        return {
            "email": "jamshidbek@example.com",
            "telegram": "@perfect_IQ",
            "linkedin": "linkedin.com/in/jamshidbek"
        }
    
    def __str__(self):
        return f"{self.name} - {self.role}"

# Instance
me = Jamshidbek()
print(f"✨ {me}")
print(f"📍 Based in: {me.location}")
print(f"🎯 Focus: {me.focus}")

</div></div><!-- ===================== TROPHIES ===================== --><div align="center"><h2 style="color: #00FF88; margin: 40px 0 20px 0;"> 🏆 <span style="border-bottom: 2px solid #00FF88; padding-bottom: 5px;">GitHub Trophies</span> </h2><img src="https://github-profile-trophy.vercel.app/?username=Jamshidbekpy&theme=onedark&no-frame=true&row=2&column=4&margin-w=15&margin-h=15&no-bg=true" alt="GitHub Trophies" style="width: 90%; max-width: 1000px;" /></div><!-- ===================== PINNED REPOS ===================== --><div align="center"><h2 style="color: #00FF88; margin: 40px 0 20px 0;"> 📌 <span style="border-bottom: 2px solid #00FF88; padding-bottom: 5px;">Featured Projects</span> </h2><div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; width: 90%; max-width: 1200px; margin: 0 auto;"><!-- Project 1 --><a href="https://github.com/Jamshidbekpy/Jamshidbekpy-Structure" style="text-decoration: none;"> <div class="stats-card" style="text-align: left;"> <h3 style="color: #00FF88; margin-top: 0;">📁 Project Structure</h3> <p style="color: #CCC;">Modern Python project structure template with best practices</p> <div style="display: flex; gap: 10px; margin-top: 15px;"> <span style="background: rgba(0, 255, 136, 0.2); color: #00FF88; padding: 3px 10px; border-radius: 15px; font-size: 0.8rem;">Python</span> <span style="background: rgba(0, 150, 255, 0.2); color: #0096FF; padding: 3px 10px; border-radius: 15px; font-size: 0.8rem;">Template</span> </div> </div> </a><!-- Project 2 --><a href="#" style="text-decoration: none;"> <div class="stats-card" style="text-align: left;"> <h3 style="color: #00FF88; margin-top: 0;">⚡ FastAPI Boilerplate</h3> <p style="color: #CCC;">Production-ready FastAPI template with authentication, docs, and tests</p> <div style="display: flex; gap: 10px; margin-top: 15px;"> <span style="background: rgba(0, 255, 136, 0.2); color: #00FF88; padding: 3px 10px; border-radius: 15px; font-size: 0.8rem;">FastAPI</span> <span style="background: rgba(255, 105, 180, 0.2); color: #FF69B4; padding: 3px 10px; border-radius: 15px; font-size: 0.8rem;">Backend</span> </div> </div> </a><!-- Project 3 --><a href="#" style="text-decoration: none;"> <div class="stats-card" style="text-align: left;"> <h3 style="color: #00FF88; margin-top: 0;">🔐 Auth Service</h3> <p style="color: #CCC;">Microservice for authentication with JWT, OAuth2, and social logins</p> <div style="display: flex; gap: 10px; margin-top: 15px;"> <span style="background: rgba(0, 255, 136, 0.2); color: #00FF88; padding: 3px 10px; border-radius: 15px; font-size: 0.8rem;">Django</span> <span style="background: rgba(255, 215, 0, 0.2); color: #FFD700; padding: 3px 10px; border-radius: 15px; font-size: 0.8rem;">Security</span> </div> </div> </a></div></div><!-- ===================== CONNECT ===================== --><div align="center"><h2 style="color: #00FF88; margin: 40px 0 20px 0;"> 🌐 <span style="border-bottom: 2px solid #00FF88; padding-bottom: 5px;">Connect With Me</span> </h2><div style="display: flex; justify-content: center; flex-wrap: wrap; gap: 15px;"><a href="https://linkedin.com/in/jamshidbek" target="_blank"> <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white&logoWidth=20" style="transition: transform 0.3s;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'" /> </a><a href="https://t.me/perfect_IQ" target="_blank"> <img src="https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white&logoWidth=20" style="transition: transform 0.3s;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'" /> </a><a href="mailto:jamshidbek@example.com" target="_blank"> <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white&logoWidth=20" style="transition: transform 0.3s;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'" /> </a><a href="https://leetcode.com/jamshidbek" target="_blank"> <img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black&logoWidth=20" style="transition: transform 0.3s;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'" /> </a><a href="https://stackoverflow.com/users/jamshidbek" target="_blank"> <img src="https://img.shields.io/badge/Stack_Overflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white&logoWidth=20" style="transition: transform 0.3s;" onmouseover="this.style.transform='scale(1.1)'" onmouseout="this.style.transform='scale(1)'" /> </a></div></div><!-- ===================== SNAKE ANIMATION ===================== --><div align="center" style="margin: 40px 0;"><h2 style="color: #00FF88; margin-bottom: 20px;"> 🐍 <span style="border-bottom: 2px solid #00FF88; padding-bottom: 5px;">Contribution Snake</span> </h2><!-- GitHub Contribution Snake -->
https://raw.githubusercontent.com/Jamshidbekpy/Jamshidbekpy/output/github-contribution-grid-snake.svg

</div><!-- ===================== FOOTER ===================== --><div align="center"><!-- Quote --><div style="background: rgba(0, 255, 136, 0.05); padding: 20px; border-radius: 15px; border: 2px solid rgba(0, 255, 136, 0.2); max-width: 800px; margin: 30px auto;"> <p style="color: #FFF; font-size: 1.1rem; font-style: italic; margin: 0;"> "Code is like humor. When you have to explain it, it's bad." </p> <p style="color: #00FF88; text-align: right; margin: 10px 0 0 0;">- Cory House</p> </div><!-- Final Wave --><img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer&reversal=true&animation=fadeIn" /><p style="color: #888; margin-top: 20px;"> ⭐️ <b>Thanks for visiting!</b> Don't forget to star my repositories if you find them useful! ⭐️ </p><p style="color: #00FF88; font-size: 0.9rem;"> Last Updated: December 2024 | 🚀 Built with GitHub Readme Magic </p><!-- Visitor Counter --><p> <img src="https://profile-counter.glitch.me/Jamshidbekpy/count.svg" alt="Visitor Count" /> </p></div><!-- ===================== SETUP NOTES ===================== --><!-- TO SETUP WAKATIME: 1. Go to https://wakatime.com/signup 2. Create account and get API key 3. Replace YOUR_WAKATIME_ID with your actual ID 4. Install WakaTime plugin in your IDE TO ENABLE SNAKE: 1. Create .github/workflows/snake.yml 2. Add workflow from: https://github.com/Platane/snk 3. It will auto-generate snake animation TO CHANGE USERNAME: 1. Replace ALL "Jamshidbekpy" with your username 2. Update email and social links 3. Update pinned repositories -->
