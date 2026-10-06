## Hi there 👋

Affaan Asif
I like to learn and train LLM and AI with a bit of cybersec...

🚀 Currently building Archangel — a software AI agency.

![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black)
![Three.js](https://img.shields.io/badge/Three.js-r165-000000?style=flat-square&logo=threedotjs)
![GSAP](https://img.shields.io/badge/GSAP-3-88CE02?style=flat-square&logo=greensock)
![Gemini](https://img.shields.io/badge/Gemini_3.1_Pro-AI-4285F4?style=flat-square&logo=google&logoColor=white)
![Status](https://img.shields.io/badge/status-active-brightgreen?style=flat-square)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

Projects
>>>> Project Hail Mary — 3D web simulation with custom shaders, physics engine, and embedded Gemini AI. Built in React + Three.js.
>>>> Geopoliticoo — Chatbot combining Claude, GPT, and Gemini for balanced geopolitical analysis.
>>>> Anomaly Detection System — Real-time brute-force detection tool built in C++ for Linux.


Credentials
· Google Cybersecurity
· CS50x 
· Python for Everybody (Michigan)
· Cisco Intro to Cybersecurity


<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Bandit completed | Muhammad Affaan</title>
<meta name="description" content="All 34 levels of OverTheWire Bandit, completed by Muhammad Affaan.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Figtree:wght@400;500;600;800&display=swap" rel="stylesheet">
<style>
:root{--bg:#fbfcfe;--ink:#0d1b2a;--mute:#5a6b7d;--line:#dbe3ec;--ok:#0b8a5f;--ok-bg:#e6f5ee;--card:#fff}
@media (prefers-color-scheme:dark){:root{--bg:#0b1420;--ink:#eaf0f7;--mute:#93a4b8;--line:#223348;--ok:#4cd9a3;--ok-bg:#10302a;--card:#101c2b}}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--ink);font:17px/1.6 "Google Sans","Figtree",system-ui,-apple-system,"Segoe UI",sans-serif;-webkit-font-smoothing:antialiased}
main{max-width:860px;margin:0 auto;padding:72px 24px 56px}
h1{font-size:clamp(2.6rem,8vw,4.6rem);line-height:1.02;font-weight:800;letter-spacing:-.035em;margin:0 0 18px}
.lead{font-size:1.2rem;color:var(--mute);max-width:36em;margin:0 0 38px}
.progress{display:flex;align-items:center;gap:16px;margin-bottom:44px}
.bar{flex:1;height:12px;border-radius:6px;background:var(--line);overflow:hidden}
.bar i{display:block;height:100%;width:100%;background:var(--ok);border-radius:6px;transform-origin:left;animation:fill 1.1s cubic-bezier(.2,.7,.2,1) both}
.progress b{font-size:1.15rem;font-weight:800;white-space:nowrap}
.levels{list-style:none;margin:0 0 64px;padding:0;display:grid;grid-template-columns:repeat(auto-fill,minmax(76px,1fr));gap:10px}
.levels a{display:flex;flex-direction:column;align-items:center;gap:2px;padding:12px 4px 10px;border-radius:12px;border:1px solid var(--line);background:var(--card);color:var(--ink);text-decoration:none;opacity:0;animation:pop .35s ease-out forwards;animation-delay:calc(var(--i)*22ms + 250ms)}
.levels a:hover{border-color:var(--ok)}
.levels a:focus-visible{outline:3px solid var(--ok);outline-offset:2px}
.levels strong{font-size:1.25rem;font-weight:800;line-height:1.1}
.levels svg{width:16px;height:16px;color:var(--ok)}
.levels .done{background:var(--ok-bg);border-color:transparent}
.levels .open{border-style:dashed}
.levels .open svg{display:none}
h2{font-size:1.5rem;font-weight:800;letter-spacing:-.02em;margin:0 0 6px}
.topics{margin:0 0 56px;padding:0;list-style:none;border-top:1px solid var(--line)}
.topics li{display:grid;grid-template-columns:190px 1fr;gap:16px;padding:14px 0;border-bottom:1px solid var(--line)}
.topics b{font-weight:600}
.topics span{color:var(--mute)}
@media (max-width:620px){.topics li{grid-template-columns:1fr;gap:2px}}
footer{color:var(--mute);font-size:.95rem}
footer a{color:var(--ok);font-weight:600}
@keyframes fill{from{transform:scaleX(0)}}
@keyframes pop{from{opacity:0;transform:translateY(6px) scale(.96)}to{opacity:1;transform:none}}
@media (prefers-reduced-motion:reduce){.bar i,.levels a{animation:none;opacity:1}}
</style>
</head>
<body>
<main>
  <h1>I finished Bandit.</h1>
  <p class="lead">All 34 levels of OverTheWire's Bandit wargame, solved over SSH on the live servers. It's the standard first stop for learning the Linux command line the way attackers and defenders actually use it.</p>

  <div class="progress">
    <div class="bar"><i></i></div>
    <b id="count">34 of 34</b>
  </div>

  <ul class="levels" id="levels" aria-label="Bandit levels"></ul>

  <h2>What the levels covered</h2>
  <ul class="topics">
    <li><b>Shell basics</b><span>Moving around, reading files with awkward names, hidden files, and working out what a machine is hiding in plain sight.</span></li>
    <li><b>Searching</b><span>find and grep against size, owner and group, then sort, uniq and strings to dig one line out of a mountain of output.</span></li>
    <li><b>Encoding and archives</b><span>Base64, ROT13, hexdumps, and files that have been compressed several layers deep.</span></li>
    <li><b>Networking</b><span>Talking to services with netcat and openssl, scanning ports with nmap, and finding the one port that answers correctly.</span></li>
    <li><b>Permissions</b><span>setuid binaries, file modes, and getting a program to run as another user.</span></li>
    <li><b>Cron and scripting</b><span>Reading scheduled jobs, working out what they run, and writing small Bash scripts to automate the grind.</span></li>
    <li><b>Git and escapes</b><span>Recovering secrets from repository history, and breaking out of restricted shells.</span></li>
  </ul>

  <footer>
    Muhammad Affaan. The wargame is free to play at <a href="https://overthewire.org/wargames/bandit/" target="_blank" rel="noopener">overthewire.org</a>, and each level above links to its task page.
  </footer>
</main>

<script>
/* Change this number if you ever want to show partial progress. */
const CLEARED = 34, TOTAL = 34;
const list = document.getElementById("levels");
const tick = '<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M5 12.5l4.5 4.5L19 7.5"/></svg>';
for (let i = 0; i < TOTAL; i++) {
  const done = i < CLEARED;
  const li = document.createElement("li");
  li.innerHTML = '<a class="' + (done ? "done" : "open") + '" style="--i:' + i + '" href="https://overthewire.org/wargames/bandit/bandit' + (i + 1) + '.html" target="_blank" rel="noopener" title="Level ' + i + ' to ' + (i + 1) + '" aria-label="Level ' + i + (done ? ', completed' : ', not completed') + '"><strong>' + i + '</strong>' + tick + '</a>';
  list.appendChild(li);
}
document.getElementById("count").textContent = CLEARED + " of " + TOTAL;
document.querySelector(".bar i").style.width = (CLEARED / TOTAL * 100) + "%";
</script>
</body>
</html>


