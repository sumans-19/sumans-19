<div align="center">

<!-- Animated SVG Hero Section -->
<svg width="100%" height="600" viewBox="0 0 1200 600" style="background: linear-gradient(135deg, #0a0e27 0%, #1a1a3e 50%, #0a0e27 100%); display: block; margin: 0 auto;">
  <defs>
    <style>
      @keyframes float {
        0%, 100% { transform: translateY(-20px); }
        50% { transform: translateY(20px); }
      }
      @keyframes glow {
        0%, 100% { filter: drop-shadow(0 0 5px #00D9FF); }
        50% { filter: drop-shadow(0 0 20px #00D9FF); }
      }
      @keyframes rotate {
        0% { transform: rotate(0deg); }
        100% { transform: rotate(360deg); }
      }
      @keyframes pulse {
        0%, 100% { opacity: 1; }
        50% { opacity: 0.5; }
      }
      .floating { animation: float 3s ease-in-out infinite; }
      .glow-text { animation: glow 2s ease-in-out infinite; }
      .rotating { animation: rotate 20s linear infinite; }
      .pulsing { animation: pulse 2s ease-in-out infinite; }
    </style>
    
    <!-- Gradient Definitions -->
    <linearGradient id="bodyGradient" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#1E90FF;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#00D9FF;stop-opacity:1" />
    </linearGradient>
    
    <radialGradient id="glowGradient" cx="50%" cy="50%" r="50%">
      <stop offset="0%" style="stop-color:#FF00FF;stop-opacity:0.8" />
      <stop offset="100%" style="stop-color:#00D9FF;stop-opacity:0" />
    </radialGradient>
  </defs>
  
  <!-- Background Grid -->
  <g opacity="0.1" stroke="#00D9FF" stroke-width="1">
    <line x1="0" y1="0" x2="1200" y2="0" />
    <line x1="0" y1="100" x2="1200" y2="100" />
    <line x1="0" y1="200" x2="1200" y2="200" />
    <line x1="0" y1="300" x2="1200" y2="300" />
    <line x1="0" y1="400" x2="1200" y2="400" />
    <line x1="0" y1="500" x2="1200" y2="500" />
    <line x1="0" y1="600" x2="1200" y2="600" />
    <line x1="150" y1="0" x2="150" y2="600" />
    <line x1="300" y1="0" x2="300" y2="600" />
    <line x1="450" y1="0" x2="450" y2="600" />
    <line x1="600" y1="0" x2="600" y2="600" />
    <line x1="750" y1="0" x2="750" y2="600" />
    <line x1="900" y1="0" x2="900" y2="600" />
    <line x1="1050" y1="0" x2="1050" y2="600" />
  </g>
  
  <!-- Floating Elements (Left Side) -->
  <g class="floating" style="animation-delay: 0s;">
    <circle cx="100" cy="150" r="40" fill="url(#glowGradient)" />
    <text x="100" y="160" font-size="50" fill="#FF00FF" text-anchor="middle" font-weight="bold" class="glow-text">{'{'}</text>
  </g>
  
  <g class="floating" style="animation-delay: 0.5s;">
    <rect x="80" y="400" width="60" height="60" fill="none" stroke="#00D9FF" stroke-width="2" rx="5" />
    <text x="110" y="440" font-size="35" fill="#00D9FF" text-anchor="middle" font-family="monospace" class="glow-text">&lt;/&gt;</text>
  </g>
  
  <!-- Animated Rotating Circle (Right Side) -->
  <g class="rotating">
    <circle cx="1100" cy="150" r="50" fill="none" stroke="url(#glowGradient)" stroke-width="2" />
    <circle cx="1100" cy="100" r="8" fill="#FF00FF" />
  </g>
  
  <!-- Central Character - Animated Developer -->
  <!-- Head -->
  <g class="floating" style="animation-delay: 0.2s;">
    <circle cx="600" cy="180" r="45" fill="url(#bodyGradient)" />
    <!-- Eyes -->
    <circle cx="585" cy="165" r="6" fill="#0a0e27" />
    <circle cx="615" cy="165" r="6" fill="#0a0e27" />
    <!-- Smile -->
    <path d="M 585 185 Q 600 195 615 185" stroke="#0a0e27" stroke-width="2" fill="none" stroke-linecap="round" />
  </g>
  
  <!-- Body -->
  <g class="floating" style="animation-delay: 0.3s;">
    <rect x="560" y="220" width="80" height="100" rx="10" fill="url(#bodyGradient)" />
    <!-- Shirt pattern -->
    <line x1="570" y1="230" x2="630" y2="230" stroke="#FF00FF" stroke-width="1" opacity="0.5" />
    <line x1="570" y1="250" x2="630" y2="250" stroke="#FF00FF" stroke-width="1" opacity="0.5" />
    <line x1="570" y1="270" x2="630" y2="270" stroke="#FF00FF" stroke-width="1" opacity="0.5" />
  </g>
  
  <!-- Arms with Keyboards/Code -->
  <!-- Left Arm -->
  <g class="floating" style="animation-delay: 0.4s;">
    <rect x="520" y="240" width="40" height="70" rx="5" fill="url(#bodyGradient)" />
    <!-- Keyboard -->
    <rect x="480" y="310" width="60" height="35" rx="3" fill="#1E90FF" stroke="#00D9FF" stroke-width="1" />
    <text x="510" y="335" font-size="16" fill="#00D9FF" text-anchor="middle" font-family="monospace" class="glow-text">CODE</text>
  </g>
  
  <!-- Right Arm -->
  <g class="floating" style="animation-delay: 0.5s;">
    <rect x="640" y="240" width="40" height="70" rx="5" fill="url(#bodyGradient)" />
    <!-- Database -->
    <ellipse cx="720" cy="325" rx="35" ry="15" fill="#FF00FF" stroke="#00D9FF" stroke-width="2" />
    <path d="M 685 325 L 685 345 Q 720 360 755 345 L 755 325" fill="#FF00FF" opacity="0.7" stroke="#00D9FF" stroke-width="2" />
    <text x="720" y="350" font-size="12" fill="#fff" text-anchor="middle" font-family="monospace">DB</text>
  </g>
  
  <!-- Legs -->
  <g class="floating" style="animation-delay: 0.6s;">
    <rect x="575" y="320" width="15" height="60" rx="7" fill="url(#bodyGradient)" />
    <rect x="610" y="320" width="15" height="60" rx="7" fill="url(#bodyGradient)" />
  </g>
  
  <!-- Floating Tech Icons (Background) -->
  <!-- Cloud -->
  <g class="pulsing" style="animation-delay: 0s; opacity: 0.6;">
    <path d="M 250 100 Q 230 80 210 90 Q 190 70 170 90 Q 150 80 150 100 Q 130 110 150 130 L 280 130 Q 300 120 280 100" 
          fill="#00D9FF" stroke="#FF00FF" stroke-width="1" />
    <text x="215" y="115" font-size="14" fill="#0a0e27" text-anchor="middle" font-family="monospace">CLOUD</text>
  </g>
  
  <!-- API Symbol -->
  <g class="pulsing" style="animation-delay: 1s; opacity: 0.6;">
    <rect x="1000" y="350" width="80" height="80" rx="5" fill="none" stroke="#FF00FF" stroke-width="2" />
    <circle cx="1015" cy="365" r="8" fill="#00D9FF" />
    <circle cx="1065" cy="365" r="8" fill="#00D9FF" />
    <circle cx="1015" cy="415" r="8" fill="#00D9FF" />
    <circle cx="1065" cy="415" r="8" fill="#00D9FF" />
    <line x1="1023" y1="365" x2="1057" y2="365" stroke="#FF00FF" stroke-width="1" />
    <line x1="1023" y1="415" x2="1057" y2="415" stroke="#FF00FF" stroke-width="1" />
    <line x1="1015" y1="373" x2="1015" y2="407" stroke="#FF00FF" stroke-width="1" />
    <line x1="1065" y1="373" x2="1065" y2="407" stroke="#FF00FF" stroke-width="1" />
  </g>
  
  <!-- System Symbol -->
  <g class="pulsing" style="animation-delay: 0.5s; opacity: 0.6;">
    <rect x="100" y="450" width="90" height="70" rx="5" fill="none" stroke="#00D9FF" stroke-width="2" />
    <line x1="110" y1="460" x2="180" y2="460" stroke="#00D9FF" stroke-width="1" />
    <line x1="110" y1="475" x2="180" y2="475" stroke="#FF00FF" stroke-width="1" />
    <line x1="110" y1="490" x2="180" y2="490" stroke="#00D9FF" stroke-width="1" />
    <line x1="110" y1="505" x2="165" y2="505" stroke="#FF00FF" stroke-width="1" />
  </g>
  
  <!-- Main Title with Glow -->
  <text x="600" y="520" font-size="70" font-weight="bold" fill="#00D9FF" text-anchor="middle" 
        font-family="Arial, sans-serif" class="glow-text" letter-spacing="3">SUMAN S</text>
  
  <!-- Subtitle -->
  <text x="600" y="570" font-size="28" fill="#FF00FF" text-anchor="middle" 
        font-family="Arial, sans-serif" class="glow-text">Full Stack Developer | System Design Architect</text>
  
  <!-- Bottom Border Line -->
  <line x1="50" y1="595" x2="1150" y2="595" stroke="#00D9FF" stroke-width="2" opacity="0.5" />
</svg>

---

<br/>

## About Me

I'm a passionate **Full Stack Developer** and **System Design Architect** from Mysore, India. I specialize in building scalable applications, cloud infrastructure, and innovative solutions using cutting-edge technologies.

**Currently:** Architecting enterprise solutions | Mastering system design | Exploring AI/ML applications

---

## Technical Credentials

### Programming Languages
<div align="center">
  <img src="https://skillicons.dev/icons?i=c,cpp,python,java,javascript,typescript" />
</div>

### Frontend Development
<div align="center">
  <img src="https://skillicons.dev/icons?i=html,css,react,nextjs,tailwind" />
</div>

### Backend & Databases
<div align="center">
  <img src="https://skillicons.dev/icons?i=nodejs,express,mongodb,mysql,postgresql,firebase" />
</div>

### Cloud & DevOps
<div align="center">
  <img src="https://skillicons.dev/icons?i=docker,kubernetes,aws,linux" />
</div>

### Tools & Platforms
<div align="center">
  <img src="https://skillicons.dev/icons?i=git,github,vscode,postman" />
</div>

---

## Achievements & Recognition

| | | | |
|:---:|:---:|:---:|:---:|
| **AI/ML Hackathon** | **InfoThon 2025** | **LeetCode** | **GDG Lead** |
| Winner 2025 | Winner | 150+ Problems | VVCE Community |
| **CGPA** | **ISRO Project** | **Projects** | **Experience** |
| 9.39 / 10.0 | Moon Detection (YOLO) | 10+ Deployed | Enterprise Solutions |

---

## What I Do

**Core Expertise**
- System Architecture & Microservices
- Full-Stack Web Development
- Cloud & DevOps Infrastructure
- AI/ML Integration
- Cybersecurity & System Hardening

**Professional Experience**
- Software Development Consultant
- Enterprise ERP Solutions
- Scalable Travel Platform Architecture
- Technical Mentoring & Community Building

---

## GitHub Statistics

<p align="center">
  <img width="48%" src="https://github-readme-stats.vercel.app/api?username=sumans-19&show_icons=true&theme=dark&bg_color=0D1117&title_color=00D9FF&icon_color=00D9FF&text_color=FFFFFF&hide_border=true&count_private=true" />
  <img width="48%" src="https://github-readme-streak-stats.herokuapp.com?user=sumans-19&theme=dark&hide_border=true&stroke=00D9FF&ring=FF00FF&fire=FF6B35&currStreakNum=00D9FF&sideNums=00D9FF&background=0D1117" />
</p>

---

## Key Projects

| Project | Description |
|:---|:---|
| **ERP System** | Enterprise resource planning for Ethics Connect Ltd |
| **Travel Platform** | Scalable application for Venti Company |
| **Moon Detection** | ISRO YOLO crater detection project |
| **GDG Community** | Leading 500+ members at VVCE |

---

## Connect With Me

<p align="center">
  <a href="https://linkedin.com/in/sumans-19">
    <img src="https://img.shields.io/badge/LINKEDIN-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://github.com/sumans-19">
    <img src="https://img.shields.io/badge/GITHUB-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
  <a href="https://leetcode.com/sumans-19">
    <img src="https://img.shields.io/badge/LEETCODE-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" />
  </a>
  <a href="mailto:sumanshanthakumar@gmail.com">
    <img src="https://img.shields.io/badge/EMAIL-FF6B6B?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

<p align="center">
  <strong>📍 Mysore, India</strong> | <strong>📞 +91 7483907615</strong><br>
  <strong>✉️ sumanshanthakumar@gmail.com</strong>
</p>

---

## Available For

- Collaborations on innovative tech projects
- Full-time/Part-time opportunities
- Technical mentoring
- Open-source contributions
- Freelance consulting

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=sumans-19&color=00D9FF&style=for-the-badge&label=PROFILE+VIEWS" />
</p>

<p align="center">
  <strong>Last Updated:</strong> June 2025 | <strong>Status:</strong> Open to Opportunities
</p>

</div>