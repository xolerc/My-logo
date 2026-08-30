<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>XOLERIC — Logo Variantlari</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&family=Space+Grotesk:wght@500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#07090b;
    --panel:#0d1114;
    --panel-2:#0f1417;
    --border:#1b2226;
    --border-soft:#161c1f;
    --text:#f2f5f7;
    --muted:#7c8890;
    --muted-2:#4d565b;
    --blue:#00d4ff;
    --green:#39ffa0;
    --blue-dim:#0090b8;
    --green-dim:#1e9e63;
  }
  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;background:var(--bg);color:var(--text);font-family:'Inter',sans-serif;}
  body{padding:0 0 80px;}

  .hero{
    padding:72px 24px 48px;
    max-width:1200px;
    margin:0 auto;
    border-bottom:1px solid var(--border-soft);
  }
  .eyebrow{
    font-family:'JetBrains Mono',monospace;
    font-size:12px;
    letter-spacing:0.18em;
    text-transform:uppercase;
    color:var(--green);
    display:flex;
    align-items:center;
    gap:10px;
    margin-bottom:20px;
  }
  .eyebrow::before{
    content:"";
    width:6px;height:6px;border-radius:50%;
    background:var(--green);
    box-shadow:0 0 8px var(--green);
  }
  .hero h1{
    font-family:'Space Grotesk',sans-serif;
    font-size:clamp(32px,5vw,54px);
    font-weight:700;
    margin:0 0 16px;
    line-height:1.05;
    letter-spacing:-0.02em;
  }
  .hero h1 span{
    background:linear-gradient(90deg,var(--blue),var(--green));
    -webkit-background-clip:text;
    background-clip:text;
    color:transparent;
  }
  .hero p{
    color:var(--muted);
    font-size:16px;
    line-height:1.6;
    max-width:640px;
    margin:0;
  }

  .grid{
    max-width:1200px;
    margin:48px auto 0;
    padding:0 24px;
    display:grid;
    grid-template-columns:repeat(auto-fill,minmax(320px,1fr));
    gap:20px;
  }

  .card{
    background:var(--panel);
    border:1px solid var(--border);
    border-radius:14px;
    overflow:hidden;
    display:flex;
    flex-direction:column;
    transition:border-color .2s ease, transform .2s ease;
  }
  .card:hover{
    border-color:#2a3338;
  }

  .preview{
    position:relative;
    aspect-ratio:16/9;
    display:flex;
    align-items:center;
    justify-content:center;
    background:
      radial-gradient(circle at 30% 20%, rgba(0,212,255,0.06), transparent 60%),
      radial-gradient(circle at 80% 80%, rgba(57,255,160,0.05), transparent 55%),
      #060809;
    padding:20px;
  }
  .preview svg{ max-width:88%; max-height:78%; }

  .index-tag{
    position:absolute;
    top:10px; left:12px;
    font-family:'JetBrains Mono',monospace;
    font-size:10px;
    color:var(--muted-2);
    letter-spacing:0.08em;
  }

  .meta{
    padding:14px 16px 12px;
    border-top:1px solid var(--border-soft);
  }
  .meta h3{
    margin:0 0 4px;
    font-family:'Space Grotesk',sans-serif;
    font-size:14.5px;
    font-weight:600;
    letter-spacing:0.01em;
  }
  .meta p{
    margin:0;
    font-size:12.5px;
    color:var(--muted);
    line-height:1.45;
  }

  .code-toggle{
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:10px 16px;
    background:var(--panel-2);
    border-top:1px solid var(--border-soft);
  }
  .code-toggle button{
    all:unset;
    cursor:pointer;
    font-family:'JetBrains Mono',monospace;
    font-size:11px;
    color:var(--muted);
    letter-spacing:0.04em;
    display:flex;
    align-items:center;
    gap:6px;
  }
  .code-toggle button:hover{ color:var(--blue); }
  .code-toggle .chev{ transition:transform .18s ease; font-size:10px; }
  .code-toggle button.open .chev{ transform:rotate(90deg); }

  .copy-btn{
    all:unset;
    cursor:pointer;
    font-family:'JetBrains Mono',monospace;
    font-size:11px;
    padding:5px 10px;
    border-radius:6px;
    border:1px solid var(--border);
    color:var(--text);
    background:#0a0e10;
    display:flex;
    align-items:center;
    gap:6px;
    transition:all .15s ease;
  }
  .copy-btn:hover{ border-color:var(--green); color:var(--green); }
  .copy-btn.copied{ border-color:var(--green); color:var(--green); background:rgba(57,255,160,0.08); }

  pre.code-block{
    margin:0;
    max-height:0;
    overflow:hidden;
    transition:max-height .25s ease;
    background:#08090b;
  }
  pre.code-block.open{
    max-height:340px;
    overflow:auto;
  }
  pre.code-block code{
    display:block;
    padding:14px 16px 18px;
    font-family:'JetBrains Mono',monospace;
    font-size:11px;
    line-height:1.6;
    color:#9fe8c8;
    white-space:pre;
  }

  footer{
    max-width:1200px;
    margin:56px auto 0;
    padding:0 24px;
    color:var(--muted-2);
    font-family:'JetBrains Mono',monospace;
    font-size:11.5px;
    letter-spacing:0.03em;
  }
</style>
</head>
<body>

<div class="hero">
  <div class="eyebrow">20 VARIANT — XOLERIC IDENTITY</div>
  <h1>XOLERIC uchun <span>20 ta logo</span> variant</h1>
  <p>Qora fon + neon ko'k va yashil ranglar asosida, professional aniqlik va kreativlik ramzini ifodalovchi 20 xil yechim. Har bir kartochka ostida SVG kodi bor — "Kodni ko'rish" tugmasi bilan ochib, "Nusxalash" orqali to'g'ridan-to'g'ri loyihangizga qo'yishingiz mumkin.</p>
</div>

<div class="grid" id="grid"></div>

<footer>XOLERIC © 2026 — SVG format, istalgan o'lchamda sifat yo'qotmaydi.</footer>

<script>
const NS = "http://www.w3.org/2000/svg";

// ---- Reusable svg fragments as raw strings ----
const logos = [
{
  title: "01 · Sof Wordmark",
  desc: "Inter Black, keng oraliq, X harfi gradient bilan urg'ulangan.",
  svg: `<svg viewBox="0 0 320 100" xmlns="http://www.w3.org/2000/svg">
  <defs><linearGradient id="g1" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0" stop-color="#00d4ff"/><stop offset="1" stop-color="#39ffa0"/>
  </linearGradient></defs>
  <text x="160" y="58" text-anchor="middle" font-family="Inter, sans-serif" font-weight="800" font-size="34" letter-spacing="6" fill="#f2f5f7">
    <tspan fill="url(#g1)">X</tspan>OLERIC
  </text>
</svg>`
},
{
  title: "02 · Nishon Monogram",
  desc: "Aylana ichida aniq kesishgan X — presizion va fokus ramzi.",
  svg: `<svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <circle cx="100" cy="100" r="86" fill="none" stroke="#1b2226" stroke-width="2"/>
  <circle cx="100" cy="100" r="86" fill="none" stroke="#00d4ff" stroke-width="2.5" stroke-dasharray="10 400" stroke-linecap="round"/>
  <line x1="55" y1="55" x2="145" y2="145" stroke="#00d4ff" stroke-width="7" stroke-linecap="round"/>
  <line x1="145" y1="55" x2="55" y2="145" stroke="#39ffa0" stroke-width="7" stroke-linecap="round"/>
  <circle cx="100" cy="100" r="5" fill="#f2f5f7"/>
</svg>`
},
{
  title: "03 · Waveform Wordmark",
  desc: "Harflar ostida audio to'lqin chiziqlari — musiqa mahsuloti uchun.",
  svg: `<svg viewBox="0 0 320 110" xmlns="http://www.w3.org/2000/svg">
  <text x="160" y="52" text-anchor="middle" font-family="Inter, sans-serif" font-weight="800" font-size="30" letter-spacing="5" fill="#f2f5f7">XOLERIC</text>
  <g stroke-linecap="round" stroke-width="4">
    <line x1="60" y1="70" x2="60" y2="82" stroke="#00d4ff"/>
    <line x1="80" y1="64" x2="80" y2="88" stroke="#00d4ff"/>
    <line x1="100" y1="70" x2="100" y2="82" stroke="#1fb8dd"/>
    <line x1="120" y1="60" x2="120" y2="92" stroke="#39ffa0"/>
    <line x1="140" y1="68" x2="140" y2="84" stroke="#39ffa0"/>
    <line x1="160" y1="66" x2="160" y2="86" stroke="#39ffa0"/>
    <line x1="180" y1="70" x2="180" y2="82" stroke="#00d4ff"/>
    <line x1="200" y1="62" x2="200" y2="90" stroke="#00d4ff"/>
    <line x1="220" y1="70" x2="220" y2="82" stroke="#1fb8dd"/>
    <line x1="240" y1="66" x2="240" y2="86" stroke="#39ffa0"/>
    <line x1="260" y1="70" x2="260" y2="82" stroke="#00d4ff"/>
  </g>
</svg>`
},
{
  title: "04 · Outline Wordmark",
  desc: "Faqat kontur chiziqli harflar — texnik chizma uslubi.",
  svg: `<svg viewBox="0 0 320 100" xmlns="http://www.w3.org/2000/svg">
  <text x="160" y="60" text-anchor="middle" font-family="Inter, sans-serif" font-weight="800" font-size="34" letter-spacing="6" fill="none" stroke="#00d4ff" stroke-width="1.4">XOLERIC</text>
</svg>`
},
{
  title: "05 · Split Duo Wordmark",
  desc: "Diagonal chegara bo'ylab yarmi ko'k, yarmi yashil.",
  svg: `<svg viewBox="0 0 320 100" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <clipPath id="clipL"><polygon points="0,0 170,0 150,100 0,100"/></clipPath>
    <clipPath id="clipR"><polygon points="170,0 320,0 320,100 150,100"/></clipPath>
  </defs>
  <g clip-path="url(#clipL)">
    <text x="160" y="60" text-anchor="middle" font-family="Inter, sans-serif" font-weight="800" font-size="34" letter-spacing="6" fill="#00d4ff">XOLERIC</text>
  </g>
  <g clip-path="url(#clipR)">
    <text x="160" y="60" text-anchor="middle" font-family="Inter, sans-serif" font-weight="800" font-size="34" letter-spacing="6" fill="#39ffa0">XOLERIC</text>
  </g>
  <line x1="160" y1="10" x2="140" y2="90" stroke="#f2f5f7" stroke-width="1" opacity="0.25"/>
</svg>`
},
{
  title: "06 · Olti burchak Belgi",
  desc: "Hexagon ramka ichida geometrik X — muhandislik hissi.",
  svg: `<svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <polygon points="100,14 172,56 172,144 100,186 28,144 28,56" fill="none" stroke="#39ffa0" stroke-width="2.5"/>
  <line x1="70" y1="70" x2="130" y2="130" stroke="#f2f5f7" stroke-width="8" stroke-linecap="round"/>
  <line x1="130" y1="70" x2="70" y2="130" stroke="#f2f5f7" stroke-width="8" stroke-linecap="round"/>
  <line x1="70" y1="70" x2="130" y2="130" stroke="#00d4ff" stroke-width="8" stroke-linecap="round" stroke-dasharray="6 82"/>
</svg>`
},
{
  title: "07 · Qavs Lockup",
  desc: "Kvadrat qavslar orasida nom — texnik/kod estetikasi.",
  svg: `<svg viewBox="0 0 320 100" xmlns="http://www.w3.org/2000/svg">
  <text x="30" y="60" font-family="JetBrains Mono, monospace" font-weight="500" font-size="34" fill="#39ffa0">[</text>
  <text x="160" y="58" text-anchor="middle" font-family="Inter, sans-serif" font-weight="700" font-size="26" letter-spacing="4" fill="#f2f5f7">XOLERIC</text>
  <text x="290" y="60" font-family="JetBrains Mono, monospace" font-weight="500" font-size="34" fill="#39ffa0">]</text>
</svg>`
},
{
  title: "08 · Gradient Chip + Wordmark",
  desc: "Mesh-gradient kvadrat belgi va yoniga wordmark joylashuvi.",
  svg: `<svg viewBox="0 0 320 100" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <radialGradient id="g8a" cx="30%" cy="30%" r="80%">
      <stop offset="0" stop-color="#39ffa0"/><stop offset="1" stop-color="#00d4ff"/>
    </radialGradient>
  </defs>
  <rect x="10" y="16" width="68" height="68" rx="18" fill="url(#g8a)"/>
  <path d="M30 34 L58 66 M58 34 L30 66" stroke="#07090b" stroke-width="6" stroke-linecap="round"/>
  <text x="96" y="52" font-family="Inter, sans-serif" font-weight="800" font-size="24" letter-spacing="2" fill="#f2f5f7">XOLERIC</text>
  <text x="96" y="70" font-family="JetBrains Mono, monospace" font-weight="400" font-size="10" letter-spacing="4" fill="#7c8890">STUDIO</text>
</svg>`
},
{
  title: "09 · Kompas Monogram",
  desc: "Konsentrik yoylar — chizmachilik asboblari ilhomi, aniqlik ramzi.",
  svg: `<svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <circle cx="100" cy="100" r="70" fill="none" stroke="#161c1f" stroke-width="2"/>
  <path d="M100 30 A70 70 0 0 1 170 100" fill="none" stroke="#00d4ff" stroke-width="3"/>
  <path d="M100 170 A70 70 0 0 1 30 100" fill="none" stroke="#39ffa0" stroke-width="3"/>
  <line x1="100" y1="55" x2="100" y2="145" stroke="#f2f5f7" stroke-width="4" stroke-linecap="round" transform="rotate(45 100 100)"/>
  <line x1="100" y1="55" x2="100" y2="145" stroke="#f2f5f7" stroke-width="4" stroke-linecap="round" transform="rotate(-45 100 100)"/>
  <circle cx="100" cy="100" r="4" fill="#00d4ff"/>
</svg>`
},
{
  title: "10 · Skanerlash Chizig'i",
  desc: "Wordmark ostida o'lchov belgilari — interfeys/UI hissi.",
  svg: `<svg viewBox="0 0 320 110" xmlns="http://www.w3.org/2000/svg">
  <text x="160" y="54" text-anchor="middle" font-family="Inter, sans-serif" font-weight="800" font-size="32" letter-spacing="5" fill="#f2f5f7">XOLERIC</text>
  <line x1="40" y1="76" x2="280" y2="76" stroke="#1b2226" stroke-width="1"/>
  <line x1="40" y1="76" x2="130" y2="76" stroke="#00d4ff" stroke-width="2"/>
  <line x1="130" y1="76" x2="220" y2="76" stroke="#39ffa0" stroke-width="2"/>
  <line x1="40" y1="72" x2="40" y2="80" stroke="#7c8890" stroke-width="1"/>
  <line x1="280" y1="72" x2="280" y2="80" stroke="#7c8890" stroke-width="1"/>
</svg>`
},
{
  title: "11 · Ikki qatorli Blok",
  desc: "XOL / ERIC — zich stack, monospace kodli estetika.",
  svg: `<svg viewBox="0 0 220 120" xmlns="http://www.w3.org/2000/svg">
  <text x="20" y="52" font-family="Inter, sans-serif" font-weight="900" font-size="38" letter-spacing="2" fill="#00d4ff">XOL</text>
  <text x="20" y="94" font-family="Inter, sans-serif" font-weight="900" font-size="38" letter-spacing="2" fill="#39ffa0">ERIC</text>
</svg>`
},
{
  title: "12 · Piksel Grid X",
  desc: "Kvadratchalar to'ridan yig'ilgan X — raqamli/matritsa uslubi.",
  svg: `<svg viewBox="0 0 160 160" xmlns="http://www.w3.org/2000/svg">
  <g fill="#00d4ff">
    <rect x="10" y="10" width="20" height="20"/><rect x="130" y="10" width="20" height="20"/>
    <rect x="40" y="40" width="20" height="20"/><rect x="100" y="40" width="20" height="20"/>
    <rect x="70" y="70" width="20" height="20" fill="#f2f5f7"/>
    <rect x="40" y="100" width="20" height="20" fill="#39ffa0"/><rect x="100" y="100" width="20" height="20" fill="#39ffa0"/>
    <rect x="10" y="130" width="20" height="20" fill="#39ffa0"/><rect x="130" y="130" width="20" height="20" fill="#39ffa0"/>
  </g>
</svg>`
},
{
  title: "13 · X Belgi + Mikro Wordmark",
  desc: "Katta X ikonka chapda, o'ngda ism va subline joylashuvi.",
  svg: `<svg viewBox="0 0 320 110" xmlns="http://www.w3.org/2000/svg">
  <path d="M14 20 L58 90 M58 20 L14 90" stroke="#00d4ff" stroke-width="9" stroke-linecap="round"/>
  <path d="M14 20 L58 90" stroke="#39ffa0" stroke-width="9" stroke-linecap="round" stroke-dasharray="8 100"/>
  <text x="80" y="52" font-family="Inter, sans-serif" font-weight="800" font-size="24" letter-spacing="2" fill="#f2f5f7">OLERIC</text>
  <text x="80" y="72" font-family="JetBrains Mono, monospace" font-weight="400" font-size="11" letter-spacing="3" fill="#7c8890">MUSIC PLAYER</text>
</svg>`
},
{
  title: "14 · Strelka-Xoch",
  desc: "Ikki o'q shakli kesishib X hosil qiladi — harakat va aniqlik.",
  svg: `<svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <path d="M40 40 L150 150 M150 150 L150 115 M150 150 L115 150" stroke="#00d4ff" stroke-width="8" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
  <path d="M160 40 L50 150 M50 150 L50 115 M50 150 L85 150" stroke="#39ffa0" stroke-width="8" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
</svg>`
},
{
  title: "15 · Neon Pill Belgi",
  desc: "Yumaloq pill ramka, markazda nom va glow nuqta.",
  svg: `<svg viewBox="0 0 320 100" xmlns="http://www.w3.org/2000/svg">
  <rect x="8" y="14" width="304" height="72" rx="36" fill="#0a0e10" stroke="#00d4ff" stroke-width="1.5"/>
  <circle cx="42" cy="50" r="6" fill="#39ffa0"/>
  <text x="170" y="58" text-anchor="middle" font-family="Inter, sans-serif" font-weight="700" font-size="24" letter-spacing="5" fill="#f2f5f7">XOLERIC</text>
</svg>`
},
{
  title: "16 · Gradient Fade Wordmark",
  desc: "Chapdan o'ngga ko'kdan yashilga tekis o'tuvchi harflar.",
  svg: `<svg viewBox="0 0 320 100" xmlns="http://www.w3.org/2000/svg">
  <defs><linearGradient id="g16" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0" stop-color="#00d4ff"/><stop offset="1" stop-color="#39ffa0"/>
  </linearGradient></defs>
  <text x="160" y="60" text-anchor="middle" font-family="Inter, sans-serif" font-weight="900" font-size="36" letter-spacing="4" fill="url(#g16)">XOLERIC</text>
</svg>`
},
{
  title: "17 · Sxema Tugunlari X",
  desc: "Elektron sxema uslubidagi tugun va chiziqlardan X.",
  svg: `<svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <g stroke="#39ffa0" stroke-width="2" fill="none">
    <line x1="40" y1="40" x2="100" y2="100"/><line x1="100" y1="100" x2="160" y2="160"/>
    <line x1="160" y1="40" x2="100" y2="100"/><line x1="100" y1="100" x2="40" y2="160"/>
  </g>
  <g fill="#00d4ff">
    <circle cx="40" cy="40" r="7"/><circle cx="160" cy="40" r="7"/>
    <circle cx="40" cy="160" r="7"/><circle cx="160" cy="160" r="7"/>
  </g>
  <circle cx="100" cy="100" r="9" fill="#f2f5f7"/>
</svg>`
},
{
  title: "18 · Vinil Disk Monogram",
  desc: "Aylanma disk/tugma shakli — musiqa mahsulotiga ishora.",
  svg: `<svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <circle cx="100" cy="100" r="82" fill="none" stroke="#161c1f" stroke-width="2"/>
  <circle cx="100" cy="100" r="82" fill="none" stroke="#00d4ff" stroke-width="2" stroke-dasharray="2 10"/>
  <circle cx="100" cy="100" r="46" fill="none" stroke="#39ffa0" stroke-width="2"/>
  <line x1="100" y1="54" x2="100" y2="18" stroke="#f2f5f7" stroke-width="5" stroke-linecap="round"/>
  <circle cx="100" cy="100" r="6" fill="#f2f5f7"/>
</svg>`
},
{
  title: "19 · Ritmik Og'irlik Wordmark",
  desc: "Harflar navbatma-navbat qalin/yupqa — vizual ritm.",
  svg: `<svg viewBox="0 0 320 100" xmlns="http://www.w3.org/2000/svg">
  <text x="160" y="60" text-anchor="middle" font-family="Inter, sans-serif" font-size="32" letter-spacing="6" fill="#f2f5f7">
    <tspan font-weight="900" fill="#00d4ff">X</tspan><tspan font-weight="300">O</tspan><tspan font-weight="900">L</tspan><tspan font-weight="300">E</tspan><tspan font-weight="900">R</tspan><tspan font-weight="300">I</tspan><tspan font-weight="900" fill="#39ffa0">C</tspan>
  </text>
</svg>`
},
{
  title: "20 · Sinus-to'lqin X",
  desc: "Ikki kesishgan to'lqin chizig'idan X — tovush + aniqlik.",
  svg: `<svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
  <path d="M20 60 Q 60 20 100 60 T 180 60" stroke="#00d4ff" stroke-width="6" fill="none" stroke-linecap="round" transform="rotate(45 100 100)"/>
  <path d="M20 60 Q 60 20 100 60 T 180 60" stroke="#39ffa0" stroke-width="6" fill="none" stroke-linecap="round" transform="rotate(-45 100 100)"/>
  <circle cx="100" cy="100" r="5" fill="#f2f5f7"/>
</svg>`
}
];

// ---- Render ----
const grid = document.getElementById('grid');

function escapeHtml(str){
  return str.replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;');
}

logos.forEach((logo, i) => {
  const card = document.createElement('div');
  card.className = 'card';

  const codeId = `code-${i}`;

  card.innerHTML = `
    <div class="preview">${logo.svg}</div>
    <div class="meta">
      <h3>${logo.title}</h3>
      <p>${logo.desc}</p>
    </div>
    <div class="code-toggle">
      <button class="toggle-btn" data-target="${codeId}"><span class="chev">▸</span> Kodni ko'rish</button>
      <button class="copy-btn" data-copy="${i}">Nusxalash</button>
    </div>
    <pre class="code-block" id="${codeId}"><code>${escapeHtml(logo.svg)}</code></pre>
  `;
  grid.appendChild(card);
});

// Toggle code blocks
grid.addEventListener('click', (e) => {
  const toggleBtn = e.target.closest('.toggle-btn');
  if (toggleBtn) {
    const target = document.getElementById(toggleBtn.dataset.target);
    target.classList.toggle('open');
    toggleBtn.classList.toggle('open');
    toggleBtn.innerHTML = target.classList.contains('open')
      ? '<span class="chev">▸</span> Kodni yopish'
      : '<span class="chev">▸</span> Kodni ko\'rish';
    return;
  }
  const copyBtn = e.target.closest('.copy-btn');
  if (copyBtn) {
    const idx = copyBtn.dataset.copy;
    const text = logos[idx].svg;
    navigator.clipboard.writeText(text).then(() => {
      const original = copyBtn.textContent;
      copyBtn.textContent = 'Nusxalandi ✓';
      copyBtn.classList.add('copied');
      setTimeout(() => {
        copyBtn.textContent = original;
        copyBtn.classList.remove('copied');
      }, 1600);
    });
  }
});
</script>
</body>
</html>
