<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:var(--font-sans);background:transparent}
.wrap{background:var(--color-background-secondary);border-radius:14px;padding:14px;border:0.5px solid var(--color-border-tertiary)}
.tabs{display:flex;gap:6px;margin-bottom:12px}
.tab{font-size:11px;padding:4px 12px;border-radius:4px;cursor:pointer;border:0.5px solid var(--color-border-tertiary);background:transparent;color:var(--color-text-secondary);font-family:'Courier New',monospace}
.tab.on{background:var(--color-background-primary);color:var(--color-text-primary)}
.gh{background:#000;border-radius:10px;overflow:hidden;border:1px solid #222;font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif}
.hero-svg{width:100%;display:block}
.body{padding:28px 36px;max-width:860px;margin:0 auto}
.center{text-align:center}
.badges{display:flex;justify-content:center;gap:8px;flex-wrap:wrap;margin:0 0 18px}
.badge{display:inline-flex;align-items:center;gap:5px;font-size:11px;padding:6px 14px;border-radius:4px;font-weight:600;letter-spacing:0.04em;font-family:-apple-system,sans-serif}
.bw{background:#fff;color:#000}
.bs{background:#c0c0c0;color:#000}
.bd{background:#222;color:#c0c0c0;border:1px solid #333}
.typing-bar{background:#111;border:1px solid #222;border-radius:6px;padding:12px 20px;margin:0 auto 0;max-width:560px;text-align:center;font-family:'Fira Code','Courier New',monospace;font-size:13px;color:#c0c0c0;position:relative;overflow:hidden}
.cursor{display:inline-block;width:2px;height:14px;background:#c0c0c0;vertical-align:middle;margin-left:2px;animation:blink 1s step-end infinite}
@keyframes blink{0%,100%{opacity:1}50%{opacity:0}}
.divider{border:none;border-top:1px solid #1a1a1a;margin:22px 0}
.code-block{background:#0d0d0d;border:1px solid #222;border-radius:6px;padding:18px 22px;font-family:'Fira Code','Courier New',monospace;font-size:12.5px;line-height:2;margin:0 0 22px}
.kw{color:#999}.cn{color:#fff;font-weight:600}.st{color:#c0c0c0}.va{color:#888}
h2.sh{font-size:17px;font-weight:600;color:#fff;margin:26px 0 12px;padding-bottom:6px;border-bottom:1px solid #1a1a1a;display:flex;align-items:center;gap:8px}
p.bp{font-size:13.5px;color:#888;line-height:1.75;margin-bottom:10px}
p.bp strong{color:#fff}
blockquote{border-left:2px solid #333;padding:10px 16px;margin:14px 0;background:#0d0d0d;border-radius:0 5px 5px 0}
blockquote p{font-size:13px;color:#666;font-style:italic;line-height:1.65}
.stack-badges{display:flex;flex-wrap:wrap;justify-content:center;gap:6px;margin-bottom:16px}
.sbadge{display:inline-flex;align-items:center;gap:4px;font-size:11px;padding:5px 12px;border-radius:3px;font-weight:500;font-family:'Courier New',monospace}
.sb1{background:#111;border:1px solid #333;color:#fff}
.sb2{background:#0d0d0d;border:1px solid #2a2a2a;color:#c0c0c0}
.stack-table{width:100%;border-collapse:collapse;font-size:13px;margin:0 0 8px}
.stack-table th{background:#0d0d0d;color:#555;font-size:10px;letter-spacing:0.1em;text-transform:uppercase;padding:8px 14px;text-align:left;border:1px solid #1a1a1a;font-weight:500}
.stack-table td{padding:8px 14px;border:1px solid #1a1a1a;color:#888}
.stack-table td:first-child{font-weight:600;color:#fff;background:#0a0a0a;width:130px}
.stack-table td code{background:#1a1a1a;border:1px solid #2a2a2a;border-radius:3px;padding:1px 6px;font-size:11px;color:#c0c0c0;font-family:'Courier New',monospace}
.trophy-row{display:flex;justify-content:center;gap:8px;flex-wrap:wrap;margin:4px 0 0}
.trophy{background:#0d0d0d;border:1px solid #222;border-radius:6px;padding:8px 14px;text-align:center;min-width:88px}
.trophy-icon{font-size:20px;display:block;margin-bottom:3px}
.trophy-val{font-size:13px;font-weight:600;color:#fff;font-family:'Courier New',monospace}
.trophy-lbl{font-size:9px;color:#444;letter-spacing:0.1em;text-transform:uppercase;font-family:'Courier New',monospace}
.proj{background:#0d0d0d;border:1px solid #1a1a1a;border-radius:7px;padding:15px 18px;margin-bottom:12px;position:relative;overflow:hidden}
.proj::before{content:'';position:absolute;left:0;top:0;bottom:0;width:2px}
.p1::before{background:#fff}
.p2::before{background:#888}
.p3::before{background:#c0c0c0}
.p4::before{background:#555}
.proj-title{font-size:14px;font-weight:600;color:#fff;margin-bottom:5px}
.proj-title a{color:inherit;text-decoration:none}
.proj-title a:hover{text-decoration:underline}
.ptags{display:flex;gap:5px;flex-wrap:wrap;margin-bottom:8px}
.ptag{font-size:10px;font-family:'Courier New',monospace;padding:2px 8px;border-radius:20px;background:#111;border:1px solid #2a2a2a;color:#888}
.proj-desc{font-size:12.5px;color:#666;line-height:1.65;font-family:-apple-system,sans-serif}
.exp-table{width:100%;border-collapse:collapse}
.exp-table td{padding:12px 14px;border-bottom:1px solid #111;vertical-align:top;font-size:13px;color:#888}
.exp-table td:first-child{width:50px;text-align:center;font-size:18px}
.exp-table td strong{color:#fff}
.exp-table td em{color:#555;font-style:normal;font-size:11px;font-family:'Courier New',monospace}
.now-block{background:#0d0d0d;border:1px solid #1a1a1a;border-radius:6px;padding:16px 20px;font-family:'Courier New',monospace;font-size:12.5px;color:#666;line-height:2}
.now-block span{color:#c0c0c0}
.activity-mock{background:#0d0d0d;border:1px solid #1a1a1a;border-radius:6px;padding:16px;margin:4px 0}
.graph-row{display:flex;gap:3px;align-items:flex-end;height:60px}
.bar{flex:1;background:#222;border-radius:2px 2px 0 0;min-height:4px;transition:background 0.2s}
.bar.active{background:#555}
.bar.bright{background:#c0c0c0}
.graph-label{font-size:9px;color:#333;font-family:'Courier New',monospace;text-align:center;margin-top:4px}
.snake-mock{background:#0d0d0d;border:1px solid #1a1a1a;border-radius:6px;padding:14px;margin:4px 0;font-family:'Courier New',monospace;font-size:11px;color:#333;line-height:1.6;text-align:center}
.footer-svg{width:100%;display:block;margin-top:-1px}
.footer-type{text-align:center;font-family:'Courier New',monospace;font-size:11px;color:#333;padding:8px 0 18px;letter-spacing:0.1em}
.copy-zone textarea{width:100%;height:320px;font-size:11px;font-family:'Courier New',monospace;background:#0d0d0d;border:1px solid #222;border-radius:8px;padding:12px;color:#666;resize:vertical}
.copy-zone button{margin-top:6px;font-size:11px;font-family:'Courier New',monospace;padding:5px 14px}
</style>

<div class="wrap">
<div class="tabs">
  <div class="tab on" onclick="sw('pv',this)">preview</div>
  <div class="tab" onclick="sw('cd',this)">readme.md</div>
</div>

<div id="pv">
<div class="gh">

  <svg class="hero-svg" viewBox="0 0 860 240" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="hg" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#000"/>
        <stop offset="50%" stop-color="#0d0d0d"/>
        <stop offset="100%" stop-color="#000"/>
      </linearGradient>
      <radialGradient id="glow" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stop-color="#ffffff" stop-opacity="0.03"/>
        <stop offset="100%" stop-color="#000" stop-opacity="0"/>
      </radialGradient>
    </defs>
    <rect width="860" height="240" fill="url(#hg)"/>
    <rect width="860" height="240" fill="url(#glow)"/>
    <g opacity="0.07" stroke="#ffffff" stroke-width="0.5" fill="none">
      <line x1="0" y1="48" x2="860" y2="48"/>
      <line x1="0" y1="96" x2="860" y2="96"/>
      <line x1="0" y1="144" x2="860" y2="144"/>
      <line x1="0" y1="192" x2="860" y2="192"/>
      <line x1="86" y1="0" x2="86" y2="240"/>
      <line x1="172" y1="0" x2="172" y2="240"/>
      <line x1="258" y1="0" x2="258" y2="240"/>
      <line x1="344" y1="0" x2="344" y2="240"/>
      <line x1="430" y1="0" x2="430" y2="240"/>
      <line x1="516" y1="0" x2="516" y2="240"/>
      <line x1="602" y1="0" x2="602" y2="240"/>
      <line x1="688" y1="0" x2="688" y2="240"/>
      <line x1="774" y1="0" x2="774" y2="240"/>
    </g>
    <circle cx="172" cy="60" r="1.5" fill="#fff" opacity="0.4"><animate attributeName="opacity" values="0.4;1;0.4" dur="3s" repeatCount="indefinite"/></circle>
    <circle cx="344" cy="144" r="1.5" fill="#c0c0c0" opacity="0.4"><animate attributeName="opacity" values="0.4;1;0.4" dur="4.5s" repeatCount="indefinite"/></circle>
    <circle cx="516" cy="48" r="1.5" fill="#fff" opacity="0.3"><animate attributeName="opacity" values="0.3;0.9;0.3" dur="2.8s" repeatCount="indefinite"/></circle>
    <circle cx="688" cy="192" r="1.5" fill="#c0c0c0" opacity="0.5"><animate attributeName="opacity" values="0.5;1;0.5" dur="3.7s" repeatCount="indefinite"/></circle>
    <circle cx="86" cy="144" r="1" fill="#fff" opacity="0.3"><animate attributeName="opacity" values="0.3;0.8;0.3" dur="5s" repeatCount="indefinite"/></circle>
    <circle cx="774" cy="96" r="1.5" fill="#888" opacity="0.4"><animate attributeName="opacity" values="0.4;1;0.4" dur="3.2s" repeatCount="indefinite"/></circle>
    <circle cx="258" cy="192" r="1" fill="#fff" opacity="0.2"><animate attributeName="opacity" values="0.2;0.7;0.2" dur="4s" repeatCount="indefinite"/></circle>
    <circle cx="602" cy="96" r="1.5" fill="#c0c0c0" opacity="0.3"><animate attributeName="opacity" values="0.3;0.9;0.3" dur="6s" repeatCount="indefinite"/></circle>
    <line x1="172" y1="60" x2="344" y2="144" stroke="#333" stroke-width="0.4"/>
    <line x1="344" y1="144" x2="516" y2="48" stroke="#2a2a2a" stroke-width="0.4"/>
    <line x1="516" y1="48" x2="688" y2="192" stroke="#333" stroke-width="0.4"/>
    <text x="430" y="100" text-anchor="middle" font-family="-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif" font-size="38" font-weight="600" fill="#ffffff" letter-spacing="0.015em">Aiswarya Rose Jacob</text>
    <line x1="310" y1="115" x2="356" y2="115" stroke="#222" stroke-width="1"/>
    <circle cx="430" cy="115" r="3" fill="none" stroke="#555" stroke-width="1"/>
    <circle cx="430" cy="115" r="1.5" fill="#888"/>
    <line x1="504" y1="115" x2="550" y2="115" stroke="#222" stroke-width="1"/>
    <text x="430" y="142" text-anchor="middle" font-family="'Courier New',monospace" font-size="12" fill="#555" letter-spacing="0.18em">AI · MACHINE LEARNING · SYSTEMS ENGINEERING</text>
    <text x="430" y="172" text-anchor="middle" font-family="'Courier New',monospace" font-size="10" fill="#333" letter-spacing="0.12em">B.Tech CSE · AI &amp; ML Specialisation · Open to Opportunities</text>
    <path d="M0 218 Q215 200 430 212 Q645 224 860 205 L860 240 L0 240 Z" fill="#000"/>
  </svg>

  <div class="body">

    <div class="badges">
      <span class="badge bw">🔗 LinkedIn</span>
      <span class="badge bw">✉ Email</span>
      <span class="badge bs">● Open to Opportunities</span>
      <span class="badge bd">🎓 B.Tech CSE · AI & ML</span>
    </div>

    <div class="typing-bar">
      <span id="typed"></span><span class="cursor"></span>
    </div>

    <div class="divider"></div>

    <div class="code-block">
<span class="kw"># ── profile ──────────────────────────────────────────────────────</span>
<span class="kw">class</span> <span class="cn">AiswaryaRoseJacob</span>:
    role       <span class="va">=</span> <span class="st">"AI & Machine Learning Undergraduate"</span>
    education  <span class="va">=</span> <span class="st">"B.Tech CSE · AI & ML Specialisation"</span>
    focus      <span class="va">=</span> [<span class="st">"Vector Search"</span>, <span class="st">"Multi-Agent Systems"</span>, <span class="st">"NLP Pipelines"</span>]
    stack      <span class="va">=</span> [<span class="st">"Python"</span>, <span class="st">"Sentence-Transformers"</span>, <span class="st">"Scikit-learn"</span>, <span class="st">"SQL"</span>]
    internship <span class="va">=</span> <span class="st">"Infosys Springboard · Workflow Automation"</span>
    learning   <span class="va">=</span> [<span class="st">"Linear Regression"</span>, <span class="st">"Decision Trees"</span>, <span class="st">"RAG Systems"</span>]
    status     <span class="va">=</span> <span class="st">"open to opportunities"</span>
<span class="kw"># ───────────────────────────────────────────────────────────────</span>
    </div>

    <div class="divider"></div>
    <h2 class="sh">About</h2>
    <p class="bp">Computer Science undergraduate specialising in the architecture of <strong>intelligent systems</strong> — bridging raw data to actionable intelligence through clean code, modular design, and rigorous application of machine learning.</p>
    <p class="bp">I build systems that think: from <strong>semantic retrieval pipelines</strong> that understand intent, to <strong>multi-agent frameworks</strong> that coordinate autonomous workflows. Currently deepening expertise in production-grade ML and exploring RAG architecture. Passionate about systems that scale — not just prototypes that demo.</p>
    <blockquote><p>"Documenting growth as an AI & ML student through real projects, continuous learning, and building with precision."</p></blockquote>

    <div class="divider"></div>
    <h2 class="sh">Technical Stack</h2>
    <div class="stack-badges">
      <span class="sbadge sb1">Python</span>
      <span class="sbadge sb2">SQL</span>
      <span class="sbadge sb1">C</span>
      <span class="sbadge sb2">NumPy</span>
      <span class="sbadge sb1">Pandas</span>
      <span class="sbadge sb2">Scikit-learn</span>
      <span class="sbadge sb1">Streamlit</span>
      <span class="sbadge sb2">SQLite</span>
      <span class="sbadge sb1">Git</span>
      <span class="sbadge sb2">GitHub</span>
    </div>
    <table class="stack-table">
      <tr><th>Category</th><th>Technologies</th></tr>
      <tr><td>Languages</td><td><code>Python</code> <code>SQL</code> <code>C</code></td></tr>
      <tr><td>AI / ML</td><td><code>Sentence-Transformers</code> <code>Scikit-learn</code> <code>NumPy</code> <code>Pandas</code></td></tr>
      <tr><td>Engineering</td><td><code>Streamlit</code> <code>SQLite</code> <code>Git</code> <code>GitHub</code></td></tr>
      <tr><td>Concepts</td><td><code>Vector Embeddings</code> <code>Cosine Similarity</code> <code>Multi-Agent Systems</code> <code>Relational DB</code></td></tr>
    </table>

    <div class="divider"></div>
    <h2 class="sh">Trophies</h2>
    <div class="trophy-row">
      <div class="trophy"><span class="trophy-icon">⭐</span><div class="trophy-val">—</div><div class="trophy-lbl">Stars</div></div>
      <div class="trophy"><span class="trophy-icon">💻</span><div class="trophy-val">—</div><div class="trophy-lbl">Commits</div></div>
      <div class="trophy"><span class="trophy-icon">🔀</span><div class="trophy-val">—</div><div class="trophy-lbl">Pull Req</div></div>
      <div class="trophy"><span class="trophy-icon">📦</span><div class="trophy-val">4</div><div class="trophy-lbl">Repos</div></div>
      <div class="trophy"><span class="trophy-icon">🔥</span><div class="trophy-val">—</div><div class="trophy-lbl">Streak</div></div>
      <div class="trophy"><span class="trophy-icon">👥</span><div class="trophy-val">—</div><div class="trophy-lbl">Followers</div></div>
    </div>

    <div class="divider"></div>
    <h2 class="sh">Featured Projects</h2>

    <div class="proj p1">
      <div class="proj-title"><a href="#">○ Semantic Local Search</a></div>
      <div class="ptags"><span class="ptag">transformer embeddings</span><span class="ptag">cosine similarity</span><span class="ptag">retrieval pipeline</span><span class="ptag">no cloud</span></div>
      <p class="proj-desc">Custom pipeline mapping text to a 384-dimensional vector space using Sentence-Transformers. Cosine Similarity for conceptual intent matching — meaning over keyword matching. Fully local, zero cloud dependency.</p>
    </div>

    <div class="proj p2">
      <div class="proj-title"><a href="#">○ Multi-Agent Research System</a></div>
      <div class="ptags"><span class="ptag">multi-agent</span><span class="ptag">autonomous delegation</span><span class="ptag">state management</span><span class="ptag">Infosys Springboard</span></div>
      <p class="proj-desc">Developed during Infosys Springboard Virtual Internship. Multi-agent framework with autonomous task routing and lifecycle state management. Modular multi-file Python architecture for long-term scalability.</p>
    </div>

    <div class="proj p3">
      <div class="proj-title">○ Pathwise.ai</div>
      <div class="ptags"><span class="ptag">AI/ML</span><span class="ptag">career recommendation</span><span class="ptag">decision logic</span></div>
      <p class="proj-desc">AI-driven career path recommendation providing personalised guidance from structured student input. Structured decision logic with explainable user-data mapping and outcome reasoning.</p>
    </div>

    <div class="proj p4">
      <div class="proj-title">○ Blood Bank Management System</div>
      <div class="ptags"><span class="ptag">DBMS</span><span class="ptag">SQL</span><span class="ptag">relational schema</span><span class="ptag">team project</span></div>
      <p class="proj-desc">Full relational schema for donor records and blood inventory management. Complex SQL across normalised tables. Led database architecture decisions in collaborative team delivery.</p>
    </div>

    <div class="divider"></div>
    <h2 class="sh">Experience & Education</h2>
    <table class="exp-table">
      <tr>
        <td>💼</td>
        <td><strong>Virtual Intern — Workflow Automation</strong> &nbsp;<em>· Infosys Springboard</em><br/>Built the Multi-Agent Research System using Python and Streamlit. Explored agent orchestration, state management, and professional multi-file project structure. First real-world software delivery.</td>
      </tr>
      <tr>
        <td>🎓</td>
        <td><strong>B.Tech — Computer Science Engineering</strong> &nbsp;<em>· AI & ML Specialisation</em><br/>Core focus on intelligent systems architecture, relational database management, and algorithmic foundations. Applying coursework through real builds across ML, NLP, and systems design.</td>
      </tr>
    </table>

    <div class="divider"></div>
    <h2 class="sh">Currently</h2>
    <div class="now-block">
<span>◈</span>  Building supervised ML models — Linear Regression &amp; Decision Trees on real datasets
<span>◈</span>  Deepening NumPy array computation &amp; Pandas data analysis
<span>◈</span>  Expanding Semantic Local Search with richer retrieval features
<span>◈</span>  Exploring RAG (Retrieval-Augmented Generation) architecture
<span>◈</span>  Next milestone → end-to-end ML pipeline with Scikit-learn deployment
    </div>

    <div class="divider"></div>
    <h2 class="sh">GitHub Activity</h2>
    <div class="activity-mock">
      <div class="graph-label" style="color:#333;font-size:9px;margin-bottom:6px;font-family:'Courier New',monospace">contribution activity · AiswaryaRJ</div>
      <div class="graph-row" id="bars"></div>
    </div>

    <div class="divider"></div>
    <h2 class="sh">Contribution Snake</h2>
    <div class="snake-mock" id="snake-area">
      ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
    </div>

  </div>

  <svg class="footer-svg" viewBox="0 0 860 80" xmlns="http://www.w3.org/2000/svg">
    <path d="M0 0 Q215 35 430 18 Q645 0 860 28 L860 80 L0 80 Z" fill="#000"/>
    <g opacity="0.06" stroke="#fff" stroke-width="0.5" fill="none">
      <line x1="0" y1="40" x2="860" y2="40"/>
    </g>
  </svg>
  <div class="footer-type">// building systems with precision · open to opportunities</div>

</div>
</div>

<div id="cd" style="display:none">
<div class="copy-zone">
  <textarea id="rmt" readonly></textarea>
  <button onclick="cp()">copy to clipboard ↗</button>
</div>
</div>
</div>

<script>
const lines = [
  "Building intelligent systems from raw data —",
  "Semantic retrieval · Multi-agent frameworks · ML pipelines"
];
let li=0,ci=0,txt='';
const el = document.getElementById('typed');
function typeNext(){
  if(ci < lines[li].length){
    txt += lines[li][ci++];
    el.textContent = txt;
    setTimeout(typeNext, 38 + Math.random()*22);
  } else {
    setTimeout(()=>{
      li=(li+1)%lines.length;
      ci=0;txt='';
      el.textContent='';
      typeNext();
    },2800);
  }
}
typeNext();

const bars = document.getElementById('bars');
const heights=[12,20,8,35,18,45,60,22,14,50,38,25,55,10,42,30,16,48,20,58,12,40,28,52,18,44,8,36,24,52,14,46,20,60,10,38,28,54,16,42,22,50,30,44,12,56,20,48,36,60,18,42,28,54,10];
heights.forEach((h,i)=>{
  const b=document.createElement('div');
  b.className='bar'+(h>50?' bright':h>35?' active':'');
  b.style.height=h+'px';
  bars.appendChild(b);
});

const sa = document.getElementById('snake-area');
let snakePos = 5, dir = 1;
const gridW = 49;
function animSnake(){
  let grid = Array(gridW).fill('░');
  const dots=[2,8,15,22,29,36,43];
  dots.forEach(d=>{ if(d<gridW) grid[d]='▪'; });
  grid[snakePos]='●';
  snakePos += dir;
  if(snakePos >= gridW-1) dir=-1;
  if(snakePos <= 0) dir=1;
  sa.textContent = grid.join('');
}
setInterval(animSnake,80);

const README = `<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,50:1a1a1a,100:000000&height=240&section=header&text=Aiswarya%20Rose%20Jacob&fontSize=44&fontColor=ffffff&fontAlignY=42&fontAlign=50&desc=AI%20%C2%B7%20Machine%20Learning%20%C2%B7%20Systems%20Engineering&descSize=15&descAlignY=60&descColor=999999&descAlign=50&animation=twinkling&stroke=333333&strokeWidth=1" width="100%" />

<br/>

<a href="https://linkedin.com/in/aiswaryarosejacob">
  <img src="https://img.shields.io/badge/LinkedIn-ffffff?style=for-the-badge&logo=linkedin&logoColor=000000" />
</a>
<a href="mailto:aiswaryarosejacob@email.com">
  <img src="https://img.shields.io/badge/Email-ffffff?style=for-the-badge&logo=gmail&logoColor=000000" />
</a>
<img src="https://img.shields.io/badge/Open%20to%20Opportunities-c0c0c0?style=for-the-badge&logo=checkmarx&logoColor=000000" />
<img src="https://img.shields.io/badge/B.Tech%20CSE%20%7C%20AI%20%26%20ML-333333?style=for-the-badge&logo=academia&logoColor=silver" />

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=15&duration=3500&pause=1200&color=C0C0C0&center=true&vCenter=true&multiline=true&width=650&height=58&lines=Building+intelligent+systems+from+raw+data+%E2%80%94;Semantic+retrieval+%C2%B7+Multi-agent+frameworks+%C2%B7+ML+pipelines" alt="Typing SVG" />

<br/><br/>

</div>

---

\`\`\`python
# ── profile ────────────────────────────────────────────────────────────────
class AiswaryaRoseJacob:
    role       = "AI & Machine Learning Undergraduate"
    education  = "B.Tech CSE · AI & ML Specialisation"
    focus      = ["Vector Search", "Multi-Agent Systems", "NLP Pipelines"]
    stack      = ["Python", "Sentence-Transformers", "Scikit-learn", "SQL"]
    internship = "Infosys Springboard · Workflow Automation"
    learning   = ["Linear Regression", "Decision Trees", "RAG Systems"]
    status     = "open to opportunities"
# ──────────────────────────────────────────────────────────────────────────
\`\`\`

---

## About

Computer Science undergraduate specialising in the architecture of **intelligent systems** — bridging raw data to actionable intelligence through clean code, modular design, and rigorous application of machine learning.

I build systems that think: from **semantic retrieval pipelines** that understand intent, to **multi-agent frameworks** that coordinate autonomous workflows. Currently deepening expertise in production-grade ML and exploring RAG architecture. Passionate about systems that scale — not just prototypes that demo.

> *"Documenting growth as an AI & ML student through real projects, continuous learning, and building with precision."*

---

## Technical Stack

<div align="center">

![Python](https://img.shields.io/badge/Python-000000?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-1a1a1a?style=for-the-badge&logo=mysql&logoColor=silver)
![C](https://img.shields.io/badge/C-000000?style=for-the-badge&logo=c&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1a1a1a?style=for-the-badge&logo=numpy&logoColor=silver)
![Pandas](https://img.shields.io/badge/Pandas-000000?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-1a1a1a?style=for-the-badge&logo=scikit-learn&logoColor=silver)
![Streamlit](https://img.shields.io/badge/Streamlit-000000?style=for-the-badge&logo=streamlit&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-1a1a1a?style=for-the-badge&logo=sqlite&logoColor=silver)
![Git](https://img.shields.io/badge/Git-000000?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-1a1a1a?style=for-the-badge&logo=github&logoColor=silver)

</div>

<br/>

| Category | Technologies |
| :--- | :--- |
| **Languages** | Python · SQL · C |
| **AI / ML** | Sentence-Transformers · Scikit-learn · NumPy · Pandas |
| **Engineering** | Streamlit · SQLite · Git · GitHub |
| **Concepts** | Vector Embeddings · Cosine Similarity · Multi-Agent Systems · Relational DB |

---

## Trophies

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=AiswaryaRJ&theme=onestar&no-frame=true&no-bg=true&margin-w=8&column=6" width="100%" />

</div>

---

## Featured Projects

<br/>

**○ [Semantic Local Search](https://github.com/AiswaryaRJ/semantic-local-search)**

![Python](https://img.shields.io/badge/-Python-000000?style=flat-square&logo=python&logoColor=white)
![NLP](https://img.shields.io/badge/-NLP-1a1a1a?style=flat-square)
![Sentence Transformers](https://img.shields.io/badge/-Sentence%20Transformers-333333?style=flat-square)
![Cosine Similarity](https://img.shields.io/badge/-Cosine%20Similarity-1a1a1a?style=flat-square)

> Custom pipeline mapping text to a **384-dimensional vector space** using Sentence-Transformers. Cosine Similarity for conceptual intent matching — prioritising meaning over keyword matching. Fully local, zero cloud dependency.

<br/>

**○ [Multi-Agent Research System](https://github.com/AiswaryaRJ/multi-agent-research-system)**

![Python](https://img.shields.io/badge/-Python-000000?style=flat-square&logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/-Streamlit-1a1a1a?style=flat-square&logo=streamlit&logoColor=white)
![Infosys Springboard](https://img.shields.io/badge/-Infosys%20Springboard-333333?style=flat-square)
![Multi-Agent](https://img.shields.io/badge/-Multi--Agent%20Framework-1a1a1a?style=flat-square)

> Developed during the **Infosys Springboard Virtual Internship**. Multi-agent framework with autonomous task routing and lifecycle state management. Modular multi-file Python architecture built for scalability and reproducibility.

<br/>

**○ Pathwise.ai**

![AI/ML](https://img.shields.io/badge/-AI%2FML-000000?style=flat-square)
![Decision Logic](https://img.shields.io/badge/-Decision%20Logic-1a1a1a?style=flat-square)
![Career Recommendation](https://img.shields.io/badge/-Career%20Recommendation-333333?style=flat-square)

> AI-driven career path recommendation providing personalised guidance from structured student input. Structured decision logic with explainable user-data mapping and outcome reasoning.

<br/>

**○ Blood Bank Management System**

![SQL](https://img.shields.io/badge/-SQL-000000?style=flat-square&logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/-SQLite-1a1a1a?style=flat-square&logo=sqlite&logoColor=white)
![DBMS](https://img.shields.io/badge/-DBMS-333333?style=flat-square)
![Team Project](https://img.shields.io/badge/-Team%20Project-1a1a1a?style=flat-square)

> Full relational schema for donor records and blood inventory management. Complex SQL across normalised tables. Led database architecture decisions in collaborative team delivery.

---

## Experience & Education

<br/>

<table>
  <tr>
    <td width="60px" align="center">💼</td>
    <td>
      <strong>Virtual Intern — Workflow Automation</strong> &nbsp;·&nbsp; <em>Infosys Springboard</em><br/>
      Built the Multi-Agent Research System using Python and Streamlit. Explored agent orchestration, application state management, and professional multi-file project structure. First real-world software delivery experience.
    </td>
  </tr>
  <tr>
    <td width="60px" align="center">🎓</td>
    <td>
      <strong>B.Tech — Computer Science Engineering</strong> &nbsp;·&nbsp; <em>AI & ML Specialisation</em><br/>
      Core focus on intelligent systems architecture, relational database management, and algorithmic foundations. Applying coursework through real builds across ML, NLP, and systems design.
    </td>
  </tr>
</table>

---

## Currently

<br/>

\`\`\`
◈   Building supervised ML models — Linear Regression & Decision Trees on real datasets
◈   Deepening NumPy array computation & Pandas data analysis
◈   Expanding Semantic Local Search with richer retrieval features
◈   Exploring RAG (Retrieval-Augmented Generation) architecture
◈   Next milestone → end-to-end ML pipeline with Scikit-learn deployment
\`\`\`

---

## GitHub Activity

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=AiswaryaRJ&theme=github-compact&hide_border=true&bg_color=000000&color=c0c0c0&line=ffffff&point=c0c0c0&area=true&area_color=1a1a1a" width="100%" />

</div>

---

## Contribution Snake

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AiswaryaRJ/AiswaryaRJ/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AiswaryaRJ/AiswaryaRJ/output/github-contribution-grid-snake.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/AiswaryaRJ/AiswaryaRJ/output/github-contribution-grid-snake.svg" />
</picture>

</div>

<details>
<summary>↳ Activate snake animation (one-time setup)</summary>

Create <code>.github/workflows/snake.yml</code>:

\`\`\`yaml
name: Generate Snake
on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:
jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk/svg-only@v3
        with:
          github_user_name: AiswaryaRJ
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: \${{ secrets.GITHUB_TOKEN }}
\`\`\`

Then go to **Actions → Generate Snake → Run workflow**.

</details>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:000000,50:1a1a1a,100:000000&height=120&section=footer&animation=twinkling" width="100%" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=12&duration=5000&pause=1000&color=555555&center=true&vCenter=true&width=500&lines=%2F%2F+building+systems+with+precision+%C2%B7+open+to+opportunities" alt="footer" />

</div>`;

document.getElementById('rmt').value=README;
function cp(){
  navigator.clipboard.writeText(README).then(()=>{
    document.querySelector('.copy-zone button').textContent='copied ✓';
    setTimeout(()=>document.querySelector('.copy-zone button').textContent='copy to clipboard ↗',2500);
  });
}
function sw(id,el){
  document.getElementById('pv').style.display=id==='pv'?'':'none';
  document.getElementById('cd').style.display=id==='cd'?'':'none';
  document.querySelectorAll('.wrap>.tabs .tab').forEach(t=>t.classList.remove('on'));
  el.classList.add('on');
}
</script>
