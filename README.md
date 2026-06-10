<!-- SECTION A: ANIMATED HEADER -->
<!-- <div align="center">
 <img src="" width="100" height="100" />
 <h1> 👋 Hello there!</h1>
 <h2>I'm a <a href=" https://readme-typing-svg.demolab.com/?lines=Python+Full+Stack+Developer;Passionate+About+Coding;Always+Learning;Enjoy+Building+Projects!&center=true&size=30&font=Architects+Daughter&color=F7C74C ">Python Full Stack Developer</a></h2>
</div> -->
cat > /mnt/user-data/outputs/farooq44_github_header.html << 'HTMLEOF'
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Farooq44 — GitHub Header</title>
<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body { background: #010409; display: flex; align-items: center; justify-content: center; min-height: 100vh; padding: 24px; }
  #gh-banner {
    width: 100%;
    max-width: 1280px;
    aspect-ratio: 3840 / 1080;
    background: #0d1117;
    position: relative;
    overflow: hidden;
    border-radius: 12px;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  }
  canvas#starfield { position: absolute; inset: 0; width: 100%; height: 100%; }
  .grid-overlay {
    position: absolute; inset: 0;
    background-image:
      linear-gradient(rgba(48,220,137,0.04) 1px, transparent 1px),
      linear-gradient(90deg, rgba(48,220,137,0.04) 1px, transparent 1px);
    background-size: 4% 4%;
    animation: gridPulse 6s ease-in-out infinite;
  }
  @keyframes gridPulse { 0%,100%{opacity:.5}50%{opacity:1} }
  .glow-orb { position: absolute; border-radius: 50%; filter: blur(80px); animation: orbFloat 8s ease-in-out infinite; }
  .orb1 { width:40%;height:120%;top:-10%;left:-8%;background:radial-gradient(circle,rgba(48,220,137,.18) 0%,transparent 70%);animation-duration:9s; }
  .orb2 { width:35%;height:100%;top:0;right:-5%;background:radial-gradient(circle,rgba(88,166,255,.15) 0%,transparent 70%);animation-duration:11s;animation-delay:-3s; }
  .orb3 { width:25%;height:80%;top:10%;left:38%;background:radial-gradient(circle,rgba(163,113,247,.12) 0%,transparent 70%);animation-duration:7s;animation-delay:-5s; }
  @keyframes orbFloat { 0%,100%{transform:translateY(0) scale(1)}50%{transform:translateY(-8%) scale(1.06)} }
  .scan-line { position:absolute;left:0;right:0;height:2px;background:linear-gradient(90deg,transparent,rgba(48,220,137,.5),transparent);animation:scanMove 5s linear infinite;z-index:5; }
  @keyframes scanMove { from{top:-2px;opacity:.8}80%{opacity:.8}to{top:101%;opacity:0} }
  .corner { position:absolute;width:clamp(16px,3vw,40px);height:clamp(16px,3vw,40px);border-color:rgba(48,220,137,.45);border-style:solid;z-index:8; }
  .corner.tl{top:4%;left:2%;border-width:2px 0 0 2px;animation:cornerBlink 3s ease-in-out infinite}
  .corner.tr{top:4%;right:2%;border-width:2px 2px 0 0;animation:cornerBlink 3s ease-in-out infinite .5s}
  .corner.bl{bottom:4%;left:2%;border-width:0 0 2px 2px;animation:cornerBlink 3s ease-in-out infinite 1s}
  .corner.br{bottom:4%;right:2%;border-width:0 2px 2px 0;animation:cornerBlink 3s ease-in-out infinite 1.5s}
  @keyframes cornerBlink{0%,100%{opacity:.4}50%{opacity:1}}
  .content {
    position:absolute;inset:0;
    display:flex;flex-direction:column;
    align-items:center;justify-content:center;
    gap:0;z-index:10;
    padding: 2% 4%;
  }
  .top-row { display:flex;align-items:center;gap:clamp(6px,1.4vw,20px);margin-bottom:1.2%; }
  .octocat-wrap { animation:logoBounce 3s ease-in-out infinite;flex-shrink:0; }
  @keyframes logoBounce{0%,100%{transform:translateY(0)}50%{transform:translateY(-8%)}}
  .octocat-wrap svg { width:clamp(28px,6vw,78px);height:auto;filter:drop-shadow(0 0 14px rgba(48,220,137,.6)); }
  .name-block { display:flex;flex-direction:column;align-items:flex-start;gap:0.15em; }
  .username {
    font-size:clamp(16px,4vw,62px);
    font-weight:700;letter-spacing:-0.02em;line-height:1;
    background:linear-gradient(135deg,#fff 30%,#30dc89 65%,#58a6ff 100%);
    -webkit-background-clip:text;-webkit-text-fill-color:transparent;background-clip:text;
    background-size:200% auto;
    animation:shimmer 4s ease-in-out infinite;
  }
  @keyframes shimmer{0%{background-position:0% 50%}50%{background-position:100% 50%}100%{background-position:0% 50%}}
  .handle { font-size:clamp(7px,1.3vw,18px);color:#58a6ff;letter-spacing:0.04em;animation:fadeInUp 1s ease both;animation-delay:.3s; }
  @keyframes fadeInUp{from{opacity:0;transform:translateY(12px)}to{opacity:1;transform:translateY(0)}}
  .sub {
    font-size:clamp(6px,1.2vw,18px);font-weight:400;color:#8b949e;
    letter-spacing:0.06em;text-transform:uppercase;text-align:center;
    animation:fadeInUp 1.2s ease both;animation-delay:.5s;
    margin-bottom:1.6%;
  }
  .skills-row { display:flex;gap:clamp(4px,0.9vw,12px);flex-wrap:wrap;justify-content:center;margin-bottom:1.5%; }
  .skill {
    display:flex;align-items:center;gap:0.4em;
    padding:0.28em 0.85em;border-radius:999px;
    font-size:clamp(6px,0.95vw,13px);font-weight:500;letter-spacing:0.03em;border:1px solid;
    animation:badgePop .6s cubic-bezier(.34,1.56,.64,1) both;
  }
  .skill-dot { width:.6em;height:.6em;border-radius:50%;flex-shrink:0; }
  .sk-py  { background:rgba(55,118,171,.12);border-color:rgba(55,118,171,.45);color:#4da6e8; }
  .sk-py  .skill-dot { background:#4da6e8; }
  .sk-fl  { background:rgba(0,179,113,.1);border-color:rgba(0,179,113,.4);color:#30dc89; }
  .sk-fl  .skill-dot { background:#30dc89; }
  .sk-my  { background:rgba(0,117,143,.1);border-color:rgba(0,117,143,.4);color:#1ab9d4; }
  .sk-my  .skill-dot { background:#1ab9d4; }
  .sk-js  { background:rgba(247,223,30,.08);border-color:rgba(247,223,30,.35);color:#f7df1e; }
  .sk-js  .skill-dot { background:#f7df1e; }
  .sk-ht  { background:rgba(227,76,38,.1);border-color:rgba(227,76,38,.4);color:#e34c26; }
  .sk-ht  .skill-dot { background:#e34c26; }
  .sk-cs  { background:rgba(38,77,228,.1);border-color:rgba(38,77,228,.4);color:#6fa8f5; }
  .sk-cs  .skill-dot { background:#6fa8f5; }
  .skill:nth-child(1){animation-delay:.5s}
  .skill:nth-child(2){animation-delay:.65s}
  .skill:nth-child(3){animation-delay:.8s}
  .skill:nth-child(4){animation-delay:.95s}
  .skill:nth-child(5){animation-delay:1.1s}
  .skill:nth-child(6){animation-delay:1.25s}
  @keyframes badgePop{from{opacity:0;transform:scale(.6)}to{opacity:1;transform:scale(1)}}
  .stat-bar { display:flex;gap:clamp(8px,2vw,28px);align-items:center;animation:fadeInUp 1.4s ease both;animation-delay:.8s; }
  .stat { display:flex;flex-direction:column;align-items:center;gap:.2em; }
  .stat-val { font-size:clamp(8px,1.5vw,22px);font-weight:700;color:#fff; }
  .stat-lbl { font-size:clamp(5px,.65vw,9px);color:#8b949e;text-transform:uppercase;letter-spacing:.08em; }
  .stat-sep { width:1px;background:rgba(139,148,158,.3);align-self:stretch;margin:.2em 0; }
</style>
</head>
<body>

<div id="gh-banner" aria-label="Farooq44 GitHub profile banner">
  <canvas id="starfield"></canvas>
  <div class="grid-overlay"></div>
  <div class="glow-orb orb1"></div>
  <div class="glow-orb orb2"></div>
  <div class="glow-orb orb3"></div>
  <div class="scan-line"></div>
  <div class="corner tl"></div>
  <div class="corner tr"></div>
  <div class="corner bl"></div>
  <div class="corner br"></div>

  <div class="content">
    <div class="top-row">
      <div class="octocat-wrap">
        <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
          <circle cx="50" cy="50" r="48" fill="#161b22" stroke="rgba(48,220,137,0.4)" stroke-width="1.5"/>
          <path fill="#30dc89" d="M50 18C32.33 18 18 32.33 18 50c0 14.18 9.19 26.2 21.94 30.44 1.6.29 2.19-.7 2.19-1.54 0-.76-.03-3.26-.04-5.91-8.9 1.93-10.78-3.79-10.78-3.79-1.46-3.7-3.55-4.68-3.55-4.68-2.9-1.98.22-1.94.22-1.94 3.21.23 4.9 3.3 4.9 3.3 2.85 4.88 7.48 3.47 9.3 2.65.29-2.07 1.11-3.47 2.03-4.27-7.1-.81-14.57-3.55-14.57-15.8 0-3.49 1.25-6.34 3.29-8.58-.33-.81-1.43-4.06.31-8.46 0 0 2.68-.86 8.79 3.27A30.6 30.6 0 0 1 50 33.08c2.72.01 5.45.37 8.01 1.08 6.1-4.13 8.78-3.27 8.78-3.27 1.74 4.4.64 7.65.31 8.46 2.05 2.24 3.28 5.09 3.28 8.58 0 12.28-7.48 14.98-14.6 15.77 1.15 1 2.17 2.95 2.17 5.95 0 4.3-.04 7.76-.04 8.82 0 .85.58 1.85 2.2 1.54C72.82 76.19 82 64.17 82 50 82 32.33 67.67 18 50 18z"/>
        </svg>
      </div>
      <div class="name-block">
        <div class="username">Farooq44</div>
        <div class="handle">@Farooq44 &nbsp;·&nbsp; github.com/Farooq44</div>
      </div>
    </div>

    <div class="sub">Build · Ship · Repeat &nbsp;·&nbsp; Code is the canvas</div>

    <div class="skills-row">
      <span class="skill sk-py"><span class="skill-dot"></span>Python</span>
      <span class="skill sk-fl"><span class="skill-dot"></span>Flask</span>
      <span class="skill sk-my"><span class="skill-dot"></span>MySQL</span>
      <span class="skill sk-js"><span class="skill-dot"></span>JavaScript</span>
      <span class="skill sk-ht"><span class="skill-dot"></span>HTML</span>
      <span class="skill sk-cs"><span class="skill-dot"></span>CSS</span>
    </div>

    <div class="stat-bar">
      <div class="stat"><span class="stat-val" id="commits">0</span><span class="stat-lbl">Commits</span></div>
      <div class="stat-sep"></div>
      <div class="stat"><span class="stat-val" id="repos">0</span><span class="stat-lbl">Repos</span></div>
      <div class="stat-sep"></div>
      <div class="stat"><span class="stat-val" id="stars">0</span><span class="stat-lbl">Stars</span></div>
      <div class="stat-sep"></div>
      <div class="stat"><span class="stat-val" id="prs">0</span><span class="stat-lbl">Pull Requests</span></div>
    </div>
  </div>
</div>

<script>
(function(){
  const canvas = document.getElementById('starfield');
  const ctx = canvas.getContext('2d');
  const banner = document.getElementById('gh-banner');

  function resize(){ canvas.width = banner.offsetWidth; canvas.height = banner.offsetHeight; }
  resize();
  window.addEventListener('resize', resize);

  const stars = Array.from({length:220},()=>({
    x:Math.random(),y:Math.random(),
    r:Math.random()*1.4+0.3,
    alpha:Math.random()*.7+.15,
    speed:Math.random()*.00012+.00004,
    twinkle:Math.random()*Math.PI*2,
    twinkleSpeed:Math.random()*.03+.01
  }));

  const meteors=[];
  let lastMeteor=0;
  function spawnMeteor(){
    meteors.push({x:Math.random()*.6+.1,y:Math.random()*.2,len:Math.random()*.12+.06,speed:Math.random()*.003+.002,alpha:1,angle:Math.PI/5+(Math.random()-.5)*.2});
  }

  function draw(ts){
    const W=canvas.width,H=canvas.height;
    ctx.clearRect(0,0,W,H);
    for(const s of stars){
      s.twinkle+=s.twinkleSpeed;
      const a=s.alpha*(0.6+0.4*Math.sin(s.twinkle));
      ctx.beginPath();ctx.arc(s.x*W,s.y*H,s.r,0,Math.PI*2);
      ctx.fillStyle=`rgba(200,220,255,${a})`;ctx.fill();
      s.x-=s.speed;
      if(s.x<0){s.x=1;s.y=Math.random();}
    }
    if(ts-lastMeteor>2800+Math.random()*2000&&meteors.length<3){spawnMeteor();lastMeteor=ts;}
    for(let i=meteors.length-1;i>=0;i--){
      const m=meteors[i];
      const dx=Math.cos(m.angle)*m.len*W,dy=Math.sin(m.angle)*m.len*H;
      const grd=ctx.createLinearGradient(m.x*W,m.y*H,m.x*W+dx,m.y*H+dy);
      grd.addColorStop(0,'rgba(255,255,255,0)');
      grd.addColorStop(1,`rgba(180,230,255,${m.alpha*.9})`);
      ctx.beginPath();ctx.moveTo(m.x*W,m.y*H);ctx.lineTo(m.x*W+dx,m.y*H+dy);
      ctx.strokeStyle=grd;ctx.lineWidth=1.5;ctx.stroke();
      m.x+=Math.cos(m.angle)*m.speed;m.y+=Math.sin(m.angle)*m.speed;
      m.alpha-=.018;
      if(m.alpha<=0||m.x>1.1)meteors.splice(i,1);
    }
    requestAnimationFrame(draw);
  }
  requestAnimationFrame(draw);

  function animateCount(el,target,duration){
    let start=null;
    function step(ts){
      if(!start)start=ts;
      const p=Math.min((ts-start)/duration,1);
      const ease=1-Math.pow(1-p,3);
      el.textContent=Math.round(ease*target).toLocaleString();
      if(p<1)requestAnimationFrame(step);
    }
    requestAnimationFrame(step);
  }

  setTimeout(()=>{
    animateCount(document.getElementById('commits'),2847,2000);
    animateCount(document.getElementById('repos'),142,1800);
    animateCount(document.getElementById('stars'),9310,2200);
    animateCount(document.getElementById('prs'),634,1900);
  },600);
})();
</script>
</body>
</html>
HTMLEOF
echo "Done"


<!-- SECTION B: ABOUT ME -->
### About Me
I am a dedicated Python Full Stack Developer with a knack for creating efficient and scalable web applications. With 0.6 years of experience, I enjoy tackling challenges and learning new technologies.

- 🚀 Hobbies: Coding, Traveling, and Reading Tech Blogs 
- 🎓 Self-taught with a passion for continuous learning 
- ☕ Coffee enthusiast 
- 🎮 Gamer at heart 

<!-- SECTION C: TECH STACK -->
### Tech Stack
#### Frontend
![HTML]( https://img.shields.io/badge/HTML-E34F26?style=flat&logo=html5&logoColor=white ) 
![CSS]( https://img.shields.io/badge/CSS-1572B6?style=flat&logo=css3&logoColor=white ) 
![JavaScript]( https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black )

#### Backend
![Python]( https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white ) 
![Flask]( https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white ) 
![MySQL]( https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white )

#### Tools
![Git]( https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white ) 

<!-- SECTION E: GITHUB STATS -->
### GitHub Stats
![My GitHub Stats]( https://github-readme-stats.vercel.app/api?username=Farooq44&show_icons=true&theme=tokyonight )
![GitHub Streak Stats]( https://github-readme-streak-stats.herokuapp.com/?user=Farooq44&theme=tokyonight )
![Top Languages]( https://github-readme-stats.vercel.app/api/top-langs/?username=Farooq44&layout=compact&theme=tokyonight )

<!-- SECTION F: GITHUB TROPHIES -->
### GitHub Trophies
![GitHub Profile Trophy]( https://github-profile-trophy.vercel.app/?username=Farooq44&theme=darkhub )

<!-- SECTION G: VISITOR COUNTER -->
![Profile Views]( https://komarev.com/ghpvc/?username=Farooq44 )

<!-- SECTION H: FOOTER -->
### Let's Connect 
Thank you for visiting my profile! 🚀 
