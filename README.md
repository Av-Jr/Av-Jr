<table width="100%">
  <tr>
    <td width="20%" align="center" valign="center">
      <h1>Av-Jr</h1>
    </td>
    <td width="80%" align="center" valign="center">
      <style>
        @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@500;700&display=swap');
        .glitch-terminal { font-family: 'JetBrains Mono', monospace; color: #00FFCC; background: #0D1117; font-size: 1.5rem; text-shadow: 0 0 8px rgba(0, 255, 204, 0.4); display: flex; align-items: center; justify-content: center; height: 100px; position: relative; }
        .glitch-text { position: relative; white-space: nowrap; }
        .glitch-text::before, .glitch-text::after { content: attr(data-text); position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: #0D1117; overflow: hidden; }
        .glitch-text::before { left: 3px; text-shadow: -2px 0 #ff003c; animation: glitch-anim 2s infinite linear alternate-reverse; }
        .glitch-text::after { left: -3px; text-shadow: -2px 0 #00fff9; animation: glitch-anim2 2.5s infinite linear alternate-reverse; }
        @keyframes glitch-anim { 0% { clip: rect(24px, 9999px, 14px, 0); } 20% { clip: rect(85px, 9999px, 98px, 0); } 40% { clip: rect(12px, 9999px, 56px, 0); } 60% { clip: rect(74px, 9999px, 22px, 0); } 80% { clip: rect(44px, 9999px, 83px, 0); } 100% { clip: rect(93px, 9999px, 35px, 0); } }
        @keyframes glitch-anim2 { 0% { clip: rect(65px, 9999px, 100px, 0); } 20% { clip: rect(23px, 9999px, 55px, 0); } 40% { clip: rect(88px, 9999px, 11px, 0); } 60% { clip: rect(12px, 9999px, 77px, 0); } 80% { clip: rect(55px, 9999px, 33px, 0); } 100% { clip: rect(77px, 9999px, 88px, 0); } }
        .cursor-blink { display: inline-block; width: 10px; height: 1.2em; background-color: #00FFCC; margin-left: 8px; animation: blink 1s step-end infinite; }
        @keyframes blink { 50% { opacity: 0; } }
      </style>
      <div class="glitch-terminal">
        <span id="glitch-text" class="glitch-text" data-text="> System Booting...">> System Booting...</span><span class="cursor-blink"></span>
      </div>
      <script>
        const phrases = ["> Full-Stack Architect", "> AI & Robotics Engineer", "> C++ Problem Solver", "> Directive: UNIV-Platform", "> Directive: InsightFlow", "> Directive: Wake-Watch", "> Directive: Triumph-Archive"];
        class TextScramble {
          constructor(el) { this.el = el; this.chars = '!<>-_\\\\/[]{}—=+*^?#________01'; this.update = this.update.bind(this); }
          setText(newText) {
            const oldText = this.el.innerText; const length = Math.max(oldText.length, newText.length); const promise = new Promise((resolve) => this.resolve = resolve);
            this.queue = []; for (let i = 0; i < length; i++) { const from = oldText[i] || ''; const to = newText[i] || ''; const start = Math.floor(Math.random() * 40); const end = start + Math.floor(Math.random() * 40); this.queue.push({ from, to, start, end }); }
            cancelAnimationFrame(this.frameRequest); this.frame = 0; this.update(); return promise;
          }
          update() {
            let output = ''; let complete = 0;
            for (let i = 0, n = this.queue.length; i < n; i++) {
              let { from, to, start, end, char } = this.queue[i];
              if (this.frame >= end) { complete++; output += to; }
              else if (this.frame >= start) { if (!char || Math.random() < 0.28) { char = this.randomChar(); this.queue[i].char = char; } output += `<span style="opacity: 0.6">${char}</span>`; }
              else { output += from; }
            }
            this.el.innerHTML = output; this.el.setAttribute('data-text', this.el.innerText);
            if (complete === this.queue.length) { this.resolve(); } else { this.frameRequest = requestAnimationFrame(this.update); this.frame++; }
          }
          randomChar() { return this.chars[Math.floor(Math.random() * this.chars.length)]; }
        }
        const el = document.getElementById('glitch-text'); const fx = new TextScramble(el); let counter = 0;
        const next = () => { fx.setText(phrases[counter]).then(() => { setTimeout(next, 2500); }); counter = (counter + 1) % phrases.length; };
        next();
      </script>
    </td>
  </tr>
</table>

<div align="center">
  <a href="https://www.linkedin.com/in/aryansh-vashishtha" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="28" alt="linkedin logo"  />
  </a>
  <a href="mailto:emailtoav09@gmail.com" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Gmail&logo=gmail&label=&color=D14836&logoColor=white&labelColor=&style=for-the-badge" height="28" alt="gmail logo"  />
  </a>
  <a href="https://www.instagram.com/aryanshvashishtha" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="28" alt="instagram logo"  />
  </a>
</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=4" width="100%"/>

<table width="100%">
  <tr>
    <td width="55%" valign="top">
      <h3>💼 Active Directives</h3>
      <ul>
        <li><b><a href="https://github.com/Av-Jr/UNIV-Platform">UNIV-Platform</a></b><br/>Integrated online exam & classroom system. (<code>React 19</code>, <code>Node.js</code>)</li>
        <li><b><a href="https://github.com/Av-Jr/InsightFlow">InsightFlow</a></b><br/>Automated data analysis platform. (<code>React 19</code>, <code>Python</code>)</li>
        <li><b><a href="https://github.com/Av-Jr/Wake-Watch">Wake-Watch</a></b><br/>Real-time driver fatigue monitoring. (<code>Python</code>, <code>OpenCV</code>)</li>
        <li><b><a href="https://github.com/Av-Jr/Triumph-Archive">Triumph-Archive</a></b><br/>Secure data management tool. (<code>React 19</code>, <code>Express</code>)</li>
      </ul>
    </td>
    <td width="45%" valign="top">
      <h3>🛠️ Tech Arsenal</h3>
      <b>Core Languages & Algorithms</b><br/>
      <img src="https://skillicons.dev/icons?i=cpp,py,cs" height="40" /> <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/kotlin/kotlin-original.svg" height="40" /><br/><br/>
      <b>Full-Stack Engineering</b><br/>
      <img src="https://skillicons.dev/icons?i=react,nextjs,nodejs,tailwind" height="40" /><br/><br/>
      <b>AI, Cloud & Infrastructure</b><br/>
      <img src="https://skillicons.dev/icons?i=tensorflow,aws" height="40" />
    </td>
  </tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=4" width="100%"/>

<table width="100%">
  <tr>
    <td width="60%" valign="center">
      <h3>🚀 System Diagnostics: About Me</h3>
      Operating in my <b>3rd year of college</b>, I specialize in building high-performance, scalable systems and bridging the gap between software and hardware.<br><br>
      - 🧠 <b>Current Focus:</b> Advanced Data Structures & Algorithms, C++ optimization, and robust web architectures.<br>
      - 🦾 <b>Offline Mode:</b> Football, Robotics, and building things that actually matter.
    </td>
    <td width="40%" align="center" valign="center">
      <img height="180" src="https://64.media.tumblr.com/72983cdb4492cdf2d6bde233e050b106/tumblr_n6bvd8orqp1s4vw07o5_250.gif" alt="Iron Man HUD GIF" />
    </td>
  </tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=4" width="100%"/>

### 📊 Tactical Telemetry (GitHub Stats)

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Av-Jr&radius=16&area=true&hide_border=true&bg_color=0D1117&color=00FFCC&line=00FFCC&point=FFFFFF&area_color=00FFCC&title_color=00FFCC&area=true" height="300" alt="activity-graph graph"  />
</div>

<br/>

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Av-Jr&show_icons=true&hide_border=true&title_color=00FFCC&icon_color=00FFCC&bg_color=0D1117&text_color=F8F8F2" height="165" alt="stats graph"  />
  <img src="https://streak-stats.demolab.com?user=Av-Jr&hide_border=true&title_color=00FFCC&icon_color=00FFCC&bg_color=0D1117&text_color=F8F8F2&sideLabels=F8F8F2&sideNums=00FFCC&currStreakNum=00FFCC&ring=00FFCC&fire=00FFCC" height="165" alt="streak graph"  />
</div>

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=Av-Jr&layout=compact&langs_count=5&hide_border=true&title_color=00FFCC&icon_color=00FFCC&bg_color=0D1117&text_color=F8F8F2" height="165" alt="languages graph"  />
</div>

### 👾 Contribution Matrix

<div align="center">
  <a href="https://github.com/Av-Jr">
    <img src="https://ghchart.rshah.org/00FFCC/Av-Jr" alt="AV's GitHub Contribution Chart" width="800" />
  </a>
</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=4" width="100%"/>

> <div align="center">
>  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=15&pause=4000&color=F8F8F2&center=true&vCenter=true&width=800&lines=%22Next+time,+baby.%22+-+War+Machine;%22Sometimes+you+gotta+run+before+you+can+walk.%22+-+Iron+Man;%22It's+not+who+I+am+underneath,+but+what+I+do+that+defines+me.%22+-+Batman;%22Sir,+I+have+upgraded+the+system.%22+-+J.A.R.V.I.S." alt="Dynamic Quotes" />
> </div>

<div>
  <img style="width: 100%" src="https://capsule-render.vercel.app/api?type=waving&height=120&section=footer&reversal=false&fontSize=70&fontColor=FFFFFF&fontAlign=50&fontAlignY=50&stroke=-&animation=fadeIn&descSize=20&descAlign=50&descAlignY=50&textBg=false&color=gradient"  />
</div>
