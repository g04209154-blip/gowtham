<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1">

<title>Gowtham B | Cyber Security Student</title>

<style>

&#x20; :root {

&#x20;   --bg: #050806;

&#x20;   --panel: rgba(8, 18, 12, 0.88);

&#x20;   --line: #12361f;

&#x20;   --green: #39ff7a;

&#x20;   --dim: #6fae85;

&#x20;   --amber: #ffb454;

&#x20;   --text: #cfeedd;

&#x20; }

&#x20; \* { box-sizing: border-box; }

&#x20; html { scroll-behavior: smooth; }

&#x20; body {

&#x20;   margin: 0; background: var(--bg); color: var(--text);

&#x20;   font-family: "JetBrains Mono", "Fira Code", Consolas, "Courier New", monospace;

&#x20;   line-height: 1.7; font-size: 16px;

&#x20; }

&#x20; #rain { position: fixed; inset: 0; z-index: 0; opacity: .35; }

&#x20; .scan {

&#x20;   position: fixed; inset: 0; z-index: 1; pointer-events: none;

&#x20;   background: repeating-linear-gradient(0deg, rgba(0,0,0,.18) 0 1px, transparent 1px 3px);

&#x20; }

&#x20; main { position: relative; z-index: 2; max-width: 900px; margin: 0 auto; padding: 24px 20px 80px; }

&#x20; a { color: var(--green); }

&#x20; a:focus-visible, button:focus-visible { outline: 2px solid var(--amber); outline-offset: 3px; }

&#x20; nav { display: flex; gap: 20px; flex-wrap: wrap; padding: 12px 0; border-bottom: 1px solid var(--line); }

&#x20; nav a { text-decoration: none; color: var(--dim); }

&#x20; nav a:hover { color: var(--green); }



&#x20; .term {

&#x20;   margin-top: 40px; background: var(--panel); border: 1px solid var(--line);

&#x20;   border-radius: 6px; box-shadow: 0 0 40px rgba(57,255,122,.08);

&#x20; }

&#x20; .term-bar { display: flex; gap: 8px; padding: 10px 14px; border-bottom: 1px solid var(--line); align-items: center; color: var(--dim); font-size: 13px; }

&#x20; .dot { width: 10px; height: 10px; border-radius: 50%; background: var(--line); }

&#x20; .term-body { padding: 22px 20px 26px; min-height: 270px; }

&#x20; .prompt { color: var(--green); }

&#x20; .out { color: var(--text); margin: 2px 0 14px; }

&#x20; h1 { font-size: clamp(30px, 6vw, 52px); line-height: 1.1; margin: 10px 0 8px; color: var(--green); text-shadow: 0 0 14px rgba(57,255,122,.5); display: inline; }

&#x20; .cursor { display: inline-block; width: 10px; height: 1.1em; background: var(--green); vertical-align: text-bottom; animation: blink 1s steps(1) infinite; }

&#x20; @keyframes blink { 50% { opacity: 0; } }



&#x20; section { margin-top: 70px; }

&#x20; h2 { font-size: 22px; color: var(--green); margin: 0 0 18px; font-weight: 600; }

&#x20; h2::before { content: "$ "; color: var(--amber); }

&#x20; .grid { display: grid; gap: 16px; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); }

&#x20; .card { background: var(--panel); border: 1px solid var(--line); border-radius: 6px; padding: 18px; }

&#x20; .card h3 { margin: 0 0 6px; font-size: 16px; color: var(--amber); }

&#x20; .card p { margin: 0; font-size: 14px; color: var(--text); }

&#x20; .tags { display: flex; flex-wrap: wrap; gap: 10px; }

&#x20; .tag { border: 1px solid var(--line); padding: 4px 12px; border-radius: 4px; background: var(--panel); font-size: 14px; }

&#x20; .bar { height: 6px; background: var(--line); border-radius: 3px; margin-top: 8px; overflow: hidden; }

&#x20; .bar i { display: block; height: 100%; background: var(--green); }

&#x20; .skill { margin-bottom: 14px; font-size: 14px; }

&#x20; .contact a { display: inline-block; margin-right: 18px; }

&#x20; footer { margin-top: 80px; color: var(--dim); font-size: 13px; border-top: 1px solid var(--line); padding-top: 16px; }

&#x20; @media (prefers-reduced-motion: reduce) { .cursor { animation: none; } html { scroll-behavior: auto; } }

</style>

</head>

<body>

<canvas id="rain" aria-hidden="true"></canvas>

<div class="scan" aria-hidden="true"></div>



<main>

&#x20; <nav aria-label="Main">

&#x20;   <a href="#about">about</a>

&#x20;   <a href="#skills">skills</a>

&#x20;   <a href="#projects">projects</a>

&#x20;   <a href="#contact">contact</a>

&#x20; </nav>



&#x20; <div class="term" role="region" aria-label="Introduction">

&#x20;   <div class="term-bar"><span class="dot"></span><span class="dot"></span><span class="dot"></span><span>gowtham@lab:\~</span></div>

&#x20;   <div class="term-body">

&#x20;     <div><span class="prompt">gowtham@lab:\~$</span> whoami</div>

&#x20;     <h1 id="typed" aria-label="Gowtham B, cyber security student"></h1><span class="cursor" aria-hidden="true"></span>

&#x20;     <div class="out" id="sub" style="opacity:0">Cyber security student. Learning to break things so I can help fix them.</div>

&#x20;   </div>

&#x20; </div>



&#x20; <section id="about">

&#x20;   <h2>cat about.txt</h2>

&#x20;   <p>I'm Gowtham, a cyber security student focused on ethical hacking, network defense and web application security. I practice on legal labs and CTF platforms, and I document what I learn. Replace this paragraph with your own story: your college, your goals and what you are working towards.</p>

&#x20; </section>



&#x20; <section id="skills">

&#x20;   <h2>ls skills/</h2>

&#x20;   <div class="skill">Network security <div class="bar"><i style="width:75%"></i></div></div>

&#x20;   <div class="skill">Web app security (OWASP Top 10) <div class="bar"><i style="width:65%"></i></div></div>

&#x20;   <div class="skill">Linux and Bash <div class="bar"><i style="width:80%"></i></div></div>

&#x20;   <div class="skill">Python scripting <div class="bar"><i style="width:70%"></i></div></div>

&#x20;   <h3 style="color:var(--amber);font-size:15px;margin:26px 0 12px">Tools</h3>

&#x20;   <div class="tags">

&#x20;     <span class="tag">Kali Linux</span><span class="tag">Wireshark</span><span class="tag">Nmap</span>

&#x20;     <span class="tag">Burp Suite</span><span class="tag">Metasploit</span><span class="tag">Git</span>

&#x20;   </div>

&#x20; </section>



&#x20; <section id="projects">

&#x20;   <h2>ls projects/</h2>

&#x20;   <div class="grid">

&#x20;     <div class="card"><h3>Home lab</h3><p>Virtual network with Kali, a vulnerable target machine and a SIEM for practicing attack and detection.</p></div>

&#x20;     <div class="card"><h3>CTF writeups</h3><p>Step by step solutions from TryHackMe and Hack The Box rooms, explaining the thinking behind each step.</p></div>

&#x20;     <div class="card"><h3>Port scanner in Python</h3><p>A small tool that checks open ports on hosts I own, built to learn sockets and threading.</p></div>

&#x20;   </div>

&#x20; </section>



&#x20; <section id="contact" class="contact">

&#x20;   <h2>./contact.sh</h2>

&#x20;   <p>Open to internships, collaborations and CTF teams.</p>

&#x20;   <a href="mailto:you@example.com">email</a>

&#x20;   <a href="https://github.com/yourname">github</a>

&#x20;   <a href="https://linkedin.com/in/yourname">linkedin</a>

&#x20; </section>



&#x20; <footer>All testing on this site's projects is done on systems I own or have permission to test.</footer>

</main>



<script>

&#x20; // Matrix rain background

&#x20; const c = document.getElementById('rain'), x = c.getContext('2d');

&#x20; const chars = '01アイウエオカキクケコ{}\[]<>/\\\\$#%\&\*+=';

&#x20; let cols, drops, size = 16;

&#x20; function setup() {

&#x20;   c.width = innerWidth; c.height = innerHeight;

&#x20;   cols = Math.floor(c.width / size);

&#x20;   drops = Array.from({ length: cols }, () => Math.random() \* c.height / size);

&#x20; }

&#x20; function draw() {

&#x20;   x.fillStyle = 'rgba(5,8,6,0.08)'; x.fillRect(0, 0, c.width, c.height);

&#x20;   x.fillStyle = '#39ff7a'; x.font = size + 'px monospace';

&#x20;   drops.forEach((y, i) => {

&#x20;     x.fillText(chars\[Math.floor(Math.random() \* chars.length)], i \* size, y \* size);

&#x20;     if (y \* size > c.height \&\& Math.random() > 0.975) drops\[i] = 0;

&#x20;     drops\[i]++;

&#x20;   });

&#x20; }

&#x20; setup(); addEventListener('resize', setup);

&#x20; const still = matchMedia('(prefers-reduced-motion: reduce)').matches;

&#x20; if (still) { for (let i = 0; i < 40; i++) draw(); } else { setInterval(draw, 55); }



&#x20; // Typing effect for the name

&#x20; const name = 'Gowtham.B', el = document.getElementById('typed'), sub = document.getElementById('sub');

&#x20; let i = 0;

&#x20; function type() {

&#x20;   el.textContent = name.slice(0, ++i);

&#x20;   if (i < name.length \&\& !still) setTimeout(type, 110); else sub.style.opacity = 1;

&#x20; }

&#x20; still ? (el.textContent = name, sub.style.opacity = 1) : type();

</script>

</body>

</html>

