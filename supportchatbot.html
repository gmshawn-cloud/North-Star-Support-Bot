<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>North Star Outfitters — Scout Support Chat (Demo)</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Staatliches&family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root{
    --pine:      #1F2E23;
    --pine-dim:  #263F2C;
    --parchment: #E3DCC4;
    --parchment-hi: #EDE7D2;
    --blaze:     #A8461F;
    --blaze-hi:  #C2551F;
    --denim:     #46707A;
    --bark:      #6B5A46;
    --ink:       #2A2620;
    --ink-soft:  #52493d;
    --white:     #fdfaf3;

    --font-display: 'Staatliches', 'Arial Narrow', sans-serif;
    --font-body: 'Inter', system-ui, -apple-system, sans-serif;
    --font-mono: 'JetBrains Mono', 'Courier New', monospace;
  }

  * { box-sizing: border-box; }
  html, body { margin:0; padding:0; }
  body{
    font-family: var(--font-body);
    color: var(--ink);
    background: var(--pine);
    min-height: 100vh;
    position: relative;
    overflow-x: hidden;
  }

  @media (prefers-reduced-motion: reduce){
    * { animation-duration: 0.001ms !important; transition-duration: 0.001ms !important; }
  }

  /* ---------- topographic texture (used in a few places) ---------- */
  .topo-bg{
    background-image:
      repeating-radial-gradient(circle at 20% 30%, rgba(42,38,32,0.06) 0px, rgba(42,38,32,0.06) 1px, transparent 2px, transparent 26px),
      repeating-radial-gradient(circle at 80% 70%, rgba(42,38,32,0.05) 0px, rgba(42,38,32,0.05) 1px, transparent 2px, transparent 34px);
  }

  /* ================= mock storefront backdrop ================= */
  .storefront{ min-height: 100vh; }

  .site-nav{
    display:flex; align-items:center; justify-content:space-between;
    padding: 18px 5vw;
    background: var(--pine);
    border-bottom: 1px solid rgba(227,220,196,0.15);
  }
  .brand{
    display:flex; align-items:center; gap:10px;
    color: var(--parchment-hi);
  }
  .brand-mark{
    width: 16px; height: 16px;
    background: var(--blaze);
    transform: rotate(45deg);
    border-radius: 2px;
    flex-shrink:0;
  }
  .brand-name{
    font-family: var(--font-display);
    font-size: 22px;
    letter-spacing: 2px;
    text-transform: uppercase;
  }
  .nav-links{ display:flex; gap: 28px; }
  .nav-links a{
    color: rgba(227,220,196,0.75);
    text-decoration:none;
    font-size: 13px;
    letter-spacing: 0.5px;
    text-transform: uppercase;
  }
  .nav-links a:hover{ color: var(--parchment-hi); }
  @media (max-width: 720px){ .nav-links{ display:none; } }

  .hero{
    padding: 64px 5vw 56px;
    background: var(--parchment);
    position: relative;
  }
  .hero::before{
    content:"";
    position:absolute; inset:0;
    background-image: repeating-linear-gradient(0deg, rgba(42,38,32,0.05) 0 1px, transparent 1px 34px),
                       repeating-linear-gradient(90deg, rgba(42,38,32,0.035) 0 1px, transparent 1px 34px);
    pointer-events:none;
  }
  .hero-inner{ max-width: 560px; position:relative; }
  .hero-eyebrow{
    font-family: var(--font-mono);
    font-size: 12px;
    color: var(--blaze);
    letter-spacing: 1.5px;
    text-transform: uppercase;
    margin-bottom: 10px;
  }
  .hero h1{
    font-family: var(--font-display);
    font-size: clamp(38px, 6vw, 58px);
    line-height: 0.95;
    letter-spacing: 1px;
    text-transform: uppercase;
    margin: 0 0 14px;
    color: var(--ink);
  }
  .hero p{ font-size: 15px; color: var(--ink-soft); max-width: 420px; line-height:1.5; margin: 0 0 22px; }
  .hero-cta{
    display:inline-block;
    border: 1.5px solid var(--ink);
    color: var(--ink);
    padding: 11px 22px;
    font-size: 13px;
    letter-spacing: 1px;
    text-transform: uppercase;
    text-decoration:none;
    font-weight:600;
  }

  .product-teaser{
    padding: 48px 5vw 100px;
    background: var(--pine-dim);
    display:grid;
    grid-template-columns: repeat(auto-fit, minmax(180px,1fr));
    gap: 20px;
  }
  .p-card{ color: var(--parchment-hi); }
  .p-swatch{
    height: 130px;
    border-radius: 3px;
    margin-bottom: 10px;
    position: relative;
    overflow:hidden;
  }
  .p-swatch svg{ position:absolute; bottom:10px; right:12px; opacity:0.55; }
  .swatch-1{ background: linear-gradient(160deg, #5c7a5f, #3a4f3d); }
  .swatch-2{ background: linear-gradient(160deg, #7a5c46, #4a3a2c); }
  .swatch-3{ background: linear-gradient(160deg, #46606b, #2b3d44); }
  .p-title{ font-size: 13px; font-weight: 600; margin-bottom: 2px; }
  .p-sub{ font-size: 12px; color: rgba(227,220,196,0.6); font-family: var(--font-mono); }

  /* ================= chat launcher ================= */
  .launcher{
    position: fixed; right: 24px; bottom: 24px;
    display:flex; align-items:center; gap:10px;
    background: var(--blaze);
    color: var(--white);
    padding: 12px 18px 12px 14px;
    border-radius: 999px;
    cursor:pointer;
    box-shadow: 0 10px 24px rgba(0,0,0,0.35);
    border:none;
    font-family: var(--font-body); font-weight:600; font-size:14px;
    z-index: 50;
  }
  .launcher-dot{
    width:9px; height:9px; border-radius:50%;
    background:#6fcf7c;
    box-shadow: 0 0 0 3px rgba(111,207,124,0.25);
  }
  .launcher[hidden]{ display:none; }

  /* ================= chat widget ================= */
  .widget{
    position: fixed;
    right: 24px; bottom: 24px;
    width: 380px;
    max-width: calc(100vw - 32px);
    height: min(640px, calc(100vh - 48px));
    background: var(--parchment-hi);
    border-radius: 10px;
    box-shadow: 0 24px 60px rgba(0,0,0,0.45);
    display:flex; flex-direction:column;
    overflow:hidden;
    z-index: 60;
    border: 1px solid rgba(42,38,32,0.15);
  }
  .widget[hidden]{ display:none; }

  @media (max-width: 480px){
    .widget{
      right:0; bottom:0; left:0; top:0;
      width:100%; height:100%; max-width:100%;
      border-radius:0;
    }
    .launcher{ right:16px; bottom:16px; }
  }

  .widget-header{
    background: var(--pine);
    color: var(--parchment-hi);
    padding: 14px 16px;
    display:flex; align-items:center; gap: 10px;
  }
  .avatar{
    width: 34px; height:34px;
    background: var(--blaze);
    border-radius: 8px;
    display:flex; align-items:center; justify-content:center;
    transform: rotate(0deg);
    flex-shrink:0;
  }
  .avatar svg{ width:18px; height:18px; }
  .header-text{ flex:1; min-width:0; }
  .header-title{
    font-family: var(--font-display);
    font-size: 18px;
    letter-spacing: 1px;
    text-transform: uppercase;
    line-height:1.1;
  }
  .header-sub{
    font-size: 11px;
    color: rgba(227,220,196,0.65);
    display:flex; align-items:center; gap:6px;
    margin-top:2px;
  }
  .status-dot{ width:6px; height:6px; border-radius:50%; background:#6fcf7c; }
  .header-actions{ display:flex; gap:6px; }
  .icon-btn{
    width:28px; height:28px;
    background: transparent;
    border: 1px solid rgba(227,220,196,0.3);
    border-radius: 6px;
    color: rgba(227,220,196,0.85);
    cursor:pointer;
    display:flex; align-items:center; justify-content:center;
  }
  .icon-btn:hover{ background: rgba(227,220,196,0.1); }
  .icon-btn:focus-visible, button:focus-visible, input:focus-visible{
    outline: 2px solid var(--blaze-hi); outline-offset:2px;
  }

  /* ---- signature element: blaze trail progress ---- */
  .blaze-trail{
    display:flex; align-items:center; justify-content:space-between;
    padding: 10px 18px;
    background: var(--pine-dim);
    gap: 4px;
  }
  .blaze-step{
    flex:1;
    display:flex; flex-direction:column; align-items:center; gap:5px;
    position:relative;
  }
  .blaze-step:not(:last-child)::after{
    content:"";
    position:absolute;
    top:5px; left: 50%;
    width: 100%; height: 2px;
    background: rgba(227,220,196,0.18);
    z-index:0;
  }
  .blaze-mark{
    width: 10px; height:10px;
    background: rgba(227,220,196,0.22);
    transform: rotate(45deg);
    border-radius:2px;
    z-index:1;
    transition: background 0.25s ease, box-shadow 0.25s ease;
  }
  .blaze-step.visited .blaze-mark{
    background: var(--blaze);
    box-shadow: 0 0 0 3px rgba(168,70,31,0.25);
  }
  .blaze-step.current .blaze-mark{
    background: var(--blaze-hi);
    box-shadow: 0 0 0 4px rgba(194,85,31,0.35);
  }
  .blaze-label{
    font-family: var(--font-mono);
    font-size: 9px;
    letter-spacing: 0.5px;
    text-transform: uppercase;
    color: rgba(227,220,196,0.45);
    text-align:center;
  }
  .blaze-step.visited .blaze-label, .blaze-step.current .blaze-label{ color: rgba(227,220,196,0.85); }

  /* ---- messages ---- */
  .messages{
    flex:1;
    overflow-y:auto;
    padding: 18px 16px;
    background: var(--parchment);
    display:flex; flex-direction:column; gap: 12px;
  }
  .msg-row{ display:flex; gap:8px; max-width: 92%; animation: rise 0.18s ease; }
  @keyframes rise{ from{ opacity:0; transform: translateY(4px);} to{ opacity:1; transform:none; } }
  .msg-row.bot{ align-self:flex-start; }
  .msg-row.user{ align-self:flex-end; flex-direction:row-reverse; }
  .msg-row.system{ align-self:center; max-width:100%; }

  .msg-avatar{
    width: 22px; height:22px;
    background: var(--blaze);
    border-radius: 5px;
    flex-shrink:0;
    margin-top:2px;
  }
  .msg-bubble{
    padding: 10px 13px;
    font-size: 14px;
    line-height: 1.45;
  }
  .msg-row.bot .msg-bubble{
    background: var(--white);
    border: 1px solid rgba(42,38,32,0.12);
    border-radius: 3px 10px 10px 10px;
    color: var(--ink);
  }
  .msg-row.user .msg-bubble{
    background: var(--denim);
    color: var(--white);
    border-radius: 10px 3px 10px 10px;
    clip-path: polygon(0 0, 100% 0, 100% 100%, 10px 100%, 0 calc(100% - 10px));
  }
  .msg-row.system .msg-bubble{
    background: none;
    color: var(--bark);
    font-family: var(--font-mono);
    font-size: 11px;
    letter-spacing: 0.5px;
    text-transform: uppercase;
    text-align:center;
    padding: 4px 0;
    border-top: 1px dashed rgba(107,90,70,0.4);
    border-bottom: 1px dashed rgba(107,90,70,0.4);
  }
  .order-tag{
    font-family: var(--font-mono);
    background: rgba(42,38,32,0.06);
    padding: 1px 6px;
    border-radius: 3px;
  }
  .typing{ display:flex; gap:4px; padding: 4px 2px; }
  .typing span{
    width:6px; height:6px; border-radius:50%;
    background: var(--bark);
    opacity:0.5;
    animation: bounce 1s infinite ease-in-out;
  }
  .typing span:nth-child(2){ animation-delay:0.15s; }
  .typing span:nth-child(3){ animation-delay:0.3s; }
  @keyframes bounce{ 0%,60%,100%{ transform: translateY(0); opacity:0.4;} 30%{ transform: translateY(-4px); opacity:1; } }

  /* ---- quick replies ---- */
  .quick-replies{
    display:flex; flex-wrap:wrap; gap:8px;
    padding: 10px 16px;
    background: var(--parchment);
    border-top: 1px solid rgba(42,38,32,0.08);
  }
  .chip{
    font-family: var(--font-body);
    font-size: 12.5px;
    font-weight:600;
    background: var(--white);
    border: 1.5px solid var(--ink);
    color: var(--ink);
    padding: 7px 12px 7px 10px;
    border-radius: 3px;
    cursor:pointer;
    display:flex; align-items:center; gap:6px;
  }
  .chip::before{
    content:"";
    width:0; height:0;
    border-top: 4px solid transparent;
    border-bottom: 4px solid transparent;
    border-left: 6px solid var(--blaze);
  }
  .chip:hover{ background: var(--ink); color: var(--parchment-hi); }
  .chip.urgent{ border-color: var(--blaze); }

  /* ---- input row ---- */
  .input-row{
    display:flex; gap:8px;
    padding: 12px 14px;
    background: var(--parchment-hi);
    border-top: 1px solid rgba(42,38,32,0.12);
  }
  .input-row input{
    flex:1;
    font-family: var(--font-body);
    font-size: 14px;
    padding: 10px 12px;
    border: 1.5px solid rgba(42,38,32,0.25);
    border-radius: 6px;
    background: var(--white);
    color: var(--ink);
  }
  .input-row input::placeholder{ color: rgba(42,38,32,0.4); }
  .input-row button{
    font-family: var(--font-display);
    letter-spacing: 1px;
    text-transform: uppercase;
    background: var(--blaze);
    color: var(--white);
    border:none;
    padding: 0 20px;
    border-radius: 6px;
    cursor:pointer;
    font-size: 15px;
  }
  .input-row button:hover{ background: var(--blaze-hi); }

  .messages::-webkit-scrollbar{ width:8px; }
  .messages::-webkit-scrollbar-thumb{ background: rgba(42,38,32,0.2); border-radius:4px; }
</style>
</head>
<body>

  <div class="storefront">
    <nav class="site-nav">
      <div class="brand">
        <div class="brand-mark" aria-hidden="true"></div>
        <div class="brand-name">North Star Outfitters</div>
      </div>
      <div class="nav-links">
        <a href="#" onclick="return false;">Trail</a>
        <a href="#" onclick="return false;">Camp</a>
        <a href="#" onclick="return false;">Apparel</a>
        <a href="#" onclick="return false;">Sale</a>
      </div>
    </nav>

    <header class="hero">
      <div class="hero-inner">
        <div class="hero-eyebrow">New for the season</div>
        <h1>Gear up.<br>Head out.</h1>
        <p>Everything you need for the trail, the summit, or the campsite next door — built for North American weather, tested past the parking lot.</p>
        <a href="#" class="hero-cta" onclick="return false;">Shop the collection</a>
      </div>
    </header>

    <section class="product-teaser">
      <div class="p-card">
        <div class="p-swatch swatch-1">
          <svg width="36" height="24" viewBox="0 0 36 24" fill="none"><path d="M2 20 L11 8 L16 14 L23 4 L34 20 Z" stroke="#EDE7D2" stroke-width="1.4"/></svg>
        </div>
        <div class="p-title">Ridgeline Trail Shoe</div>
        <div class="p-sub">$128.00</div>
      </div>
      <div class="p-card">
        <div class="p-swatch swatch-2">
          <svg width="30" height="24" viewBox="0 0 30 24" fill="none"><path d="M4 20 L15 4 L26 20 Z" stroke="#EDE7D2" stroke-width="1.4"/></svg>
        </div>
        <div class="p-title">Switchback 3-Season Tent</div>
        <div class="p-sub">$349.00</div>
      </div>
      <div class="p-card">
        <div class="p-swatch swatch-3">
          <svg width="26" height="26" viewBox="0 0 26 26" fill="none"><circle cx="13" cy="13" r="9" stroke="#EDE7D2" stroke-width="1.4"/></svg>
        </div>
        <div class="p-title">Basecamp Insulated Shell</div>
        <div class="p-sub">$210.00</div>
      </div>
    </section>
  </div>

  <!-- launcher bubble (shown when widget is closed) -->
  <button class="launcher" id="launcher" hidden onclick="openWidget()">
    <span class="launcher-dot" aria-hidden="true"></span>
    Chat with Scout
  </button>

  <!-- chat widget -->
  <div class="widget" id="widget">
    <div class="widget-header">
      <div class="avatar" aria-hidden="true">
        <svg viewBox="0 0 24 24" fill="none"><path d="M12 3 L20 19 L12 15 L4 19 Z" fill="#EDE7D2"/></svg>
      </div>
      <div class="header-text">
        <div class="header-title">Scout</div>
        <div class="header-sub"><span class="status-dot" aria-hidden="true"></span> North Star Outfitters · trail guide</div>
      </div>
      <div class="header-actions">
        <button class="icon-btn" title="Restart conversation" onclick="restartChat()" aria-label="Restart conversation">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 12a9 9 0 1 1-3-6.7"/><path d="M21 3v6h-6"/></svg>
        </button>
        <button class="icon-btn" title="Close chat" onclick="closeWidget()" aria-label="Close chat">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M6 6l12 12M18 6L6 18"/></svg>
        </button>
      </div>
    </div>

    <div class="blaze-trail" id="blazeTrail">
      <div class="blaze-step" data-key="order"><div class="blaze-mark"></div><div class="blaze-label">Order</div></div>
      <div class="blaze-step" data-key="returns"><div class="blaze-mark"></div><div class="blaze-label">Returns</div></div>
      <div class="blaze-step" data-key="gear"><div class="blaze-mark"></div><div class="blaze-label">Gear</div></div>
      <div class="blaze-step" data-key="agent"><div class="blaze-mark"></div><div class="blaze-label">Agent</div></div>
    </div>

    <div class="messages" id="messages"></div>
    <div class="quick-replies" id="quickReplies"></div>

    <form class="input-row" id="inputForm" autocomplete="off">
      <input id="userInput" type="text" placeholder="Type a message…" aria-label="Message Scout" />
      <button type="submit">Send</button>
    </form>
  </div>

<script>
(function(){

  // ---------------- mock data (per project spec) ----------------
  const ORDER_DATA = {
    '111': { status: 'shipped', text: (t) => `Good news — order ${t} has shipped and is on track to arrive tomorrow.` },
    '222': { status: 'processing', text: (t) => `Order ${t} is still in processing. It should ship within the next 24 hours.` },
    '333': { status: 'delivered', text: (t) => `Order ${t} shows as delivered.` }
  };

  const RETURN_POLICY = "You've got 30 days from delivery to send something back, as long as it's unused and still in its original packaging.";
  const RETURNS_LINK = "northstaroutfitters.com/returns";
  const SHIPPING_INFO = "Standard shipping runs 3–5 business days. Need it faster? Expedited shipping arrives in 1–2 business days.";

  const RECOMMENDATIONS = {
    hiking:   { day: "a pair of Ridgeline trail shoes and a 20L daypack — light enough that you won't notice them by mile four.",
                overnight: "real hiking boots, a 45L pack, and a 3-season sleeping bag for whenever you stop for the night.",
                multiday: "supportive hiking boots, a 60L expedition pack, and an ultralight tent that won't slow you down." },
    camping:  { day: "a packable camp table and chair set for wherever you set up base.",
                overnight: "our Switchback 3-season tent paired with an insulated sleeping pad.",
                multiday: "a family-size tent and a full camp kitchen kit — everything short of the marshmallows." },
    climbing: { day: "approach shoes and a chalk bag for getting to and up the rock.",
                overnight: "an alpine harness and a bivy sack for sleeping wherever the route leaves you.",
                multiday: "a full big-wall rack and a haul bag built for multi-day routes." },
    cold:     { day: "the Basecamp insulated shell — enough warmth without overheating on the move.",
                overnight: "a 0°F sleeping bag and insulated boots for when the temperature really drops.",
                multiday: "an expedition parka and a four-season tent rated for the worst the trip can throw at you." }
  };

  // ---------------- intent patterns ----------------
  const RE = {
    human:   /\b(human|agent|representative|live agent|real person|talk to (a )?(person|human|agent|someone|rep)|speak to (a )?(person|human|agent|someone|rep)|chat with (a )?(person|human|agent|someone|rep)|connect me|customer service)\b/i,
    order:   /\b(track(ing)?|orders?|packages?|shipments?|parcels?|where('?s| is) my (order|package|stuff)|status of my order|where is it|didn'?t arrive|never arrived|hasn'?t arrived|not arrived|hasn'?t shown up|haven'?t (received|gotten|got)|never (received|got)|missing (package|order)|lost (package|order)|package (is )?missing)\b/i,
    returns: /\b(returns?|exchange|refund|send (this|it) back|how do returns work|damaged?|broken|broke|defective|faulty|cracked|torn|doesn't work|not working|wrong (item|size|order)|missing (item|part)s?)\b/i,
    affirm:  /\b(yes|yep|yeah|yup|sure|sounds good|all good|it'?s fine|it is fine|it'?s good|it is good|fine|great|good|perfect|no problem|no issues?)\b/i,
    negative:/\b(no|nah|nope|not good|something'?s (off|wrong)|isn'?t right|there'?s a problem|issue)\b/i,
    rec:     /\b(recommend(ation)?s?|suggest(ion)?s?|looking for|need (some )?gear|help me find|gifts?|what should i (buy|get)|find (me )?(some )?gear|gear|hiking|hikes?|camping|camps?|climbing|climbs?)\b/i,
    ship:    /\b(shipping|shipped|ships|ship|delivery time|how (fast|long) (do you|does|will) (it|you|shipping) (ship|take)|when (will|does) it (ship|arrive|get shipped|be shipped))\b/i,
    greet:   /^\s*(hi|hello|hey|yo|sup|good (morning|afternoon|evening))\b/i,
    thanks:  /\b(thanks|thank you|appreciate it|cheers)\b/i
  };

  // separate from RE.order (which routes the message) — this flags when the phrasing
  // suggests genuine concern rather than a routine status check, so the response can
  // acknowledge it and offer a person even when the lookup itself succeeds
  const NEVER_ARRIVED_RE = /\b(didn'?t arrive|never arrived|hasn'?t arrived|not arrived|hasn'?t shown up|haven'?t (received|gotten|got)|never (received|got)|missing (package|order)|lost (package|order)|package (is )?missing)\b/i;

  // ---------------- state ----------------
  let state = {};
  function freshState(){
    return {
      stage: 'MAIN',        // MAIN | AWAIT_ORDER | AWAIT_REC1 | AWAIT_REC2 | HUMAN
      fallbackStreak: 0,
      visited: new Set(),
      rec: {},
      lastTopic: null,      // tracks the most recent flow, so short corrections (e.g. "wait 333 actually") can be understood in context
      orderConcern: false,  // true when the user expressed distress ("never arrived") rather than a neutral tracking request
      invalidOrderStreak: 0 // consecutive failed order-number lookups, so repeated misses escalate instead of looping forever
    };
  }

  const messagesEl = document.getElementById('messages');
  const chipsEl = document.getElementById('quickReplies');
  const form = document.getElementById('inputForm');
  const input = document.getElementById('userInput');

  // ---------------- rendering helpers ----------------
  function scrollToBottom(){ messagesEl.scrollTop = messagesEl.scrollHeight; }

  function addMessage(text, sender){
    const row = document.createElement('div');
    row.className = 'msg-row ' + sender;
    if (sender === 'system'){
      row.innerHTML = `<div class="msg-bubble">${text}</div>`;
    } else {
      const avatar = sender === 'bot' ? '<div class="msg-avatar" aria-hidden="true"></div>' : '';
      row.innerHTML = `${avatar}<div class="msg-bubble">${text}</div>`;
    }
    messagesEl.appendChild(row);
    scrollToBottom();
  }

  function botSay(text, delay){
    return new Promise(resolve => {
      const typingRow = document.createElement('div');
      typingRow.className = 'msg-row bot';
      typingRow.innerHTML = `<div class="msg-avatar" aria-hidden="true"></div><div class="msg-bubble"><div class="typing"><span></span><span></span><span></span></div></div>`;
      messagesEl.appendChild(typingRow);
      scrollToBottom();
      setTimeout(() => {
        typingRow.remove();
        addMessage(text, 'bot');
        resolve();
      }, delay || 500);
    });
  }

  function setChips(list){
    chipsEl.innerHTML = '';
    list.forEach(item => {
      const btn = document.createElement('button');
      btn.className = 'chip' + (item.urgent ? ' urgent' : '');
      btn.textContent = item.label;
      btn.onclick = () => {
        addMessage(item.label, 'user');
        chipsEl.innerHTML = '';
        handleInput(item.value !== undefined ? item.value : item.label, true);
      };
      chipsEl.appendChild(btn);
    });
  }

  function markBlaze(key, current){
    document.querySelectorAll('.blaze-step').forEach(el => {
      if (el.dataset.key === key){
        state.visited.add(key);
        el.classList.add('visited');
        el.classList.toggle('current', !!current);
      } else if (!current) {
        el.classList.remove('current');
      }
    });
  }
  function clearCurrentBlaze(){
    document.querySelectorAll('.blaze-step').forEach(el => el.classList.remove('current'));
  }

  const MAIN_CHIPS = [
    { label: 'Track my order', value: 'track my order' },
    { label: 'Returns & exchanges', value: 'return an item' },
    { label: 'Find gear for me', value: 'recommend some gear' },
    { label: 'Talk to a person', value: 'talk to a human' }
  ];

  // ---------------- flows ----------------
  async function showMainMenu(greetingFirst){
    state.stage = 'MAIN';
    clearCurrentBlaze();
    if (greetingFirst){
      await botSay("Anything else I can help with?", 550);
    }
    setChips(MAIN_CHIPS);
  }

  async function startOrderFlow(){
    state.stage = 'AWAIT_ORDER';
    state.lastTopic = 'order';
    state.invalidOrderStreak = 0;
    markBlaze('order', true);
    await botSay("Happy to check on that — what's your order number?", 550);
    chipsEl.innerHTML = '';
  }

  async function resolveOrder(raw){
    const concerned = state.orderConcern;
    state.orderConcern = false;
    state.lastTopic = 'order';
    const digits = (raw.match(/\d+/) || [])[0];
    if (!digits || !ORDER_DATA[digits]){
      state.invalidOrderStreak = (state.invalidOrderStreak || 0) + 1;
      if (state.invalidOrderStreak >= 2){
        state.invalidOrderStreak = 0;
        await botSay("Still not finding a match — let's get you a person who can dig into this directly.", 550);
        await startHandoff();
        return;
      }
      await botSay(`I couldn't find an order matching <span class="order-tag">${digits ? '#' + digits : raw}</span>. Mind double-checking the number, or I can connect you with a person who can dig deeper.`, 600);
      setChips([
        { label: 'Try another order number', value: '__retry_order__' },
        { label: 'Talk to a person', value: 'talk to a human' },
        { label: 'Back to main menu', value: '__menu__' }
      ]);
      return;
    }
    state.invalidOrderStreak = 0;
    const order = ORDER_DATA[digits];
    await botSay(order.text('<span class="order-tag">#' + digits + '</span>'), 650);
    if (order.status === 'delivered'){
      await botSay("Did it arrive in good shape, or is something off?", 500);
      setChips([
        { label: "It's all good", value: 'all good delivered' },
        { label: 'Something arrived damaged', value: 'return an item' },
        { label: 'Back to main menu', value: '__menu__' }
      ]);
      state.stage = 'AWAIT_DELIVERY_CHECK';
      return;
    }
    if (concerned){
      await botSay("If that doesn't match what you're seeing on your end, I can loop in a person to dig deeper — just say the word.", 500);
    }
    await showMainMenu(false);
  }

  async function startReturnsFlow(){
    state.stage = 'MAIN';
    state.lastTopic = 'returns';
    markBlaze('returns', true);
    await botSay(`Our return policy: ${RETURN_POLICY}`, 550);
    await botSay(`When you're ready, start a return here: <span class="order-tag">${RETURNS_LINK}</span>`, 500);
    setChips([
      { label: 'Start my return', value: '__start_return__' },
      { label: 'What about shipping times?', value: 'shipping info' },
      { label: 'Back to main menu', value: '__menu__' }
    ]);
  }

  function extractActivityFromText(text){
    const lower = text.toLowerCase();
    if (/\b(hiking|hikes?)\b/.test(lower)) return 'hiking';
    if (/\b(camping|camps?)\b/.test(lower)) return 'camping';
    if (/\b(climbing|climbs?)\b/.test(lower)) return 'climbing';
    if (/\b(cold|winter)\b/.test(lower)) return 'cold';
    return null;
  }

  function extractDurationFromText(text){
    const lower = text.toLowerCase();
    if (/\bmulti[- ]?day\b/.test(lower)) return 'multiday';
    if (/\bovernight\b/.test(lower)) return 'overnight';
    if (/\bweekend\b/.test(lower)) return 'overnight';
    if (/\b(a|an|\d+)\s*weeks?\b/.test(lower)) return 'multiday';
    const daysMatch = lower.match(/\b(\d+)\s*-?\s*days?\b/);
    if (daysMatch){
      const n = parseInt(daysMatch[1], 10);
      if (n <= 1) return 'day';
      if (n === 2) return 'overnight';
      return 'multiday';
    }
    if (/\bday\s*trips?\b/.test(lower)) return 'day';
    return null;
  }

  const ACTIVITY_LABEL = { hiking: 'hiking', camping: 'camping', climbing: 'climbing', cold: 'cold-weather travel' };
  const DURATION_LABEL = { day: 'a day trip', overnight: 'an overnight', multiday: 'a multi-day trip' };

  async function startRecFlow(triggerText){
    state.lastTopic = 'rec';
    markBlaze('gear', true);
    state.rec = {};

    const activity = triggerText ? extractActivityFromText(triggerText) : null;
    const duration = triggerText ? extractDurationFromText(triggerText) : null;

    if (activity && duration){
      state.stage = 'MAIN';
      const rec = RECOMMENDATIONS[activity][duration];
      await botSay(`Got it — ${ACTIVITY_LABEL[activity]}, ${DURATION_LABEL[duration]}. I'd point you toward ${rec}`, 700);
      await showMainMenu(false);
      return;
    }
    if (activity){
      state.rec.activity = activity;
      state.stage = 'AWAIT_REC2';
      await botSay(`Got it — ${ACTIVITY_LABEL[activity]}. What's the setting — day trips, an overnight, or a multi-day stretch?`, 550);
      setChips([
        { label: 'Day trips', value: 'day' },
        { label: 'Overnight', value: 'overnight' },
        { label: 'Multi-day', value: 'multiday' }
      ]);
      return;
    }

    state.stage = 'AWAIT_REC1';
    await botSay("Let's find you the right gear. What are you gearing up for?", 550);
    setChips([
      { label: 'Hiking', value: 'hiking' },
      { label: 'Camping', value: 'camping' },
      { label: 'Climbing', value: 'climbing' },
      { label: 'Cold weather', value: 'cold' }
    ]);
  }

  const ACTIVITY_MAP = { hiking:'hiking', hike:'hiking', camping:'camping', camp:'camping', climbing:'climbing', climb:'climbing', cold:'cold', winter:'cold' };
  const DURATION_MAP = { day:'day', 'day trip':'day', 'day trips':'day', overnight:'overnight', multiday:'multiday', 'multi-day':'multiday', 'multi day':'multiday' };

  async function handleRec1(raw){
    const key = ACTIVITY_MAP[raw.toLowerCase().trim()] || Object.keys(ACTIVITY_MAP).find(k => raw.toLowerCase().includes(k));
    if (!key){
      await botSay("I didn't catch an activity there — hiking, camping, climbing, or cold-weather travel?", 500);
      setChips([
        { label: 'Hiking', value: 'hiking' }, { label: 'Camping', value: 'camping' },
        { label: 'Climbing', value: 'climbing' }, { label: 'Cold weather', value: 'cold' }
      ]);
      return;
    }
    state.rec.activity = ACTIVITY_MAP[key] || key;
    state.stage = 'AWAIT_REC2';
    await botSay("Got it. And what's the setting — day trips, an overnight, or a multi-day stretch?", 500);
    setChips([
      { label: 'Day trips', value: 'day' },
      { label: 'Overnight', value: 'overnight' },
      { label: 'Multi-day', value: 'multiday' }
    ]);
  }

  async function handleRec2(raw){
    const key = DURATION_MAP[raw.toLowerCase().trim()] || Object.keys(DURATION_MAP).find(k => raw.toLowerCase().includes(k));
    const duration = key ? DURATION_MAP[key] : null;
    if (!duration){
      await botSay("Day trips, overnight, or multi-day — which fits best?", 500);
      setChips([
        { label: 'Day trips', value: 'day' }, { label: 'Overnight', value: 'overnight' }, { label: 'Multi-day', value: 'multiday' }
      ]);
      return;
    }
    const rec = RECOMMENDATIONS[state.rec.activity][duration];
    await botSay(`For that, I'd point you toward ${rec}`, 700);
    await showMainMenu(false);
  }

  async function handleDeliveryCheck(raw){
    const lower = raw.toLowerCase();
    if (RE.human.test(lower)){ await startHandoff(); return; }
    const correctionNumber = raw.match(/\b\d{2,6}\b/);
    if (correctionNumber){
      state.fallbackStreak = 0;
      markBlaze('order', true);
      await resolveOrder(raw);
      return;
    }
    if (NEVER_ARRIVED_RE.test(lower)){
      await botSay("That's not something I can sort out from here, but a person on our team can look into what happened with the delivery right away.", 550);
      await startHandoff();
      return;
    }
    if (RE.returns.test(lower) || RE.negative.test(lower)){
      await botSay("Sorry to hear that — let's get it sorted.", 450);
      await startReturnsFlow();
      return;
    }
    if (RE.affirm.test(lower)){
      await botSay("Glad to hear it!", 400);
      await showMainMenu(false);
      return;
    }
    await botSay("Just to confirm — did it arrive in good shape, or is something wrong with it?", 450);
    setChips([
      { label: "It's all good", value: 'all good delivered' },
      { label: 'Something arrived damaged', value: 'return an item' },
      { label: 'Back to main menu', value: '__menu__' }
    ]);
  }

  async function startHandoff(){
    state.stage = 'HUMAN';
    state.lastTopic = 'human';
    markBlaze('agent', true);
    await botSay("No problem — let me get you connected with a Trail Guide from our support team.", 500);
    await new Promise(r => setTimeout(r, 700));
    addMessage("— Connected to Jordan, Trail Guide —", 'system');
    await botSay("Hi, this is Jordan from North Star support. I've got your conversation so far and I'm happy to help from here.", 700);
    setChips([
      { label: 'Back to main menu', value: '__menu__' }
    ]);
  }

  async function handoffReply(){
    await botSay("Jordan: Let me look into that for you — one moment.", 550);
    setChips([{ label: 'Back to main menu', value: '__menu__' }]);
  }

  async function fallback(){
    state.fallbackStreak++;
    if (state.fallbackStreak >= 2){
      await botSay("Looks like I'm not getting this one right. Want me to connect you with a person instead?", 500);
      setChips([
        { label: 'Yes, connect me', value: 'talk to a human', urgent: true },
        { label: 'Show me the menu', value: '__menu__' }
      ]);
      state.stage = 'AWAIT_HANDOFF_CONFIRM';
      return;
    }
    await botSay("Hmm, I didn't quite catch that. Here's what I can help with:", 500);
    setChips(MAIN_CHIPS);
  }

  async function handleHandoffConfirm(raw){
    const lower = raw.toLowerCase();
    if (RE.human.test(lower) || RE.affirm.test(lower)){
      state.fallbackStreak = 0;
      await startHandoff();
      return;
    }
    if (RE.negative.test(lower)){
      state.fallbackStreak = 0;
      await showMainMenu(false);
      return;
    }
    await botSay("Just to confirm — connect you with a person, or would you rather see the main menu?", 450);
    setChips([
      { label: 'Yes, connect me', value: 'talk to a human', urgent: true },
      { label: 'Show me the menu', value: '__menu__' }
    ]);
  }

  // ---------------- router ----------------
  async function handleInput(raw, fromChip){
    const text = String(raw);
    const lower = text.toLowerCase();

    if (text === '__menu__'){ await showMainMenu(false); return; }
    if (text === '__retry_order__'){ await startOrderFlow(); return; }
    if (text === '__start_return__'){
      await botSay("You're all set — head to the link above whenever you're ready, and drop me a note if anything looks off once it's processed.", 550);
      await showMainMenu(false);
      return;
    }

    // context-specific stages take priority
    if (state.stage === 'AWAIT_ORDER'){
      if (RE.human.test(lower)) { state.fallbackStreak = 0; await startHandoff(); return; }
      if (RE.returns.test(lower)) { state.fallbackStreak = 0; await startReturnsFlow(); return; }
      if (RE.rec.test(lower)) { state.fallbackStreak = 0; await startRecFlow(text); return; }
      state.fallbackStreak = 0;
      await resolveOrder(text);
      return;
    }
    if (state.stage === 'AWAIT_REC1'){ await handleRec1(text); return; }
    if (state.stage === 'AWAIT_REC2'){ await handleRec2(text); return; }
    if (state.stage === 'AWAIT_DELIVERY_CHECK'){ await handleDeliveryCheck(text); return; }
    if (state.stage === 'AWAIT_HANDOFF_CONFIRM'){ await handleHandoffConfirm(text); return; }
    if (state.stage === 'HUMAN'){ await handoffReply(); return; }

    // a bare order number typed cold (e.g. "111" or "#222") — treat as a direct lookup
    if (/^#?\d{2,6}$/.test(text.trim())) {
      state.fallbackStreak = 0;
      markBlaze('order', true);
      await resolveOrder(text);
      return;
    }

    // general intent recognition
    // returns/damage language is checked ahead of generic order words, since a message like
    // "my package arrived damaged" contains both, and the damage complaint is the real intent
    if (RE.human.test(lower)) { state.fallbackStreak = 0; await startHandoff(); return; }
    if (RE.returns.test(lower)) { state.fallbackStreak = 0; await startReturnsFlow(); return; }
    if (RE.order.test(lower)) {
      state.fallbackStreak = 0;
      state.orderConcern = NEVER_ARRIVED_RE.test(lower);
      const inlineDigits = text.match(/\d{2,6}/);
      if (inlineDigits) { markBlaze('order', true); await resolveOrder(text); }
      else { await startOrderFlow(); }
      return;
    }
    if (RE.rec.test(lower)) { state.fallbackStreak = 0; await startRecFlow(text); return; }
    if (RE.ship.test(lower)) {
      state.fallbackStreak = 0;
      await botSay(SHIPPING_INFO, 500);
      await showMainMenu(false);
      return;
    }
    if (RE.greet.test(lower) && !fromChip) {
      state.fallbackStreak = 0;
      await botSay("Hey! What can I help you with today?", 450);
      setChips(MAIN_CHIPS);
      return;
    }
    if (RE.thanks.test(lower)) {
      state.fallbackStreak = 0;
      await botSay("Anytime! Anything else you need?", 450);
      setChips(MAIN_CHIPS);
      return;
    }

    // a short correction like "wait 333 actually" or "no, it's 111" right after an order
    // lookup — no keyword to match on, but the number plus recent context makes intent clear
    if (state.lastTopic === 'order') {
      const correctionNumber = text.match(/\b\d{2,6}\b/);
      if (correctionNumber) {
        state.fallbackStreak = 0;
        markBlaze('order', true);
        await resolveOrder(text);
        return;
      }
    }

    await fallback();
  }

  // ---------------- boot / controls ----------------
  async function bootConversation(){
    messagesEl.innerHTML = '';
    document.querySelectorAll('.blaze-step').forEach(el => el.classList.remove('visited','current'));
    state = freshState();
    await botSay("Hey there — I'm Scout, your trail guide from North Star Outfitters. I can help track an order, sort a return, find the right gear, or connect you with a real person.", 400);
    await botSay("What do you need today?", 500);
    setChips(MAIN_CHIPS);
  }

  window.restartChat = function(){ bootConversation(); };
  window.closeWidget = function(){
    document.getElementById('widget').hidden = true;
    document.getElementById('launcher').hidden = false;
  };
  window.openWidget = function(){
    document.getElementById('widget').hidden = false;
    document.getElementById('launcher').hidden = true;
  };

  form.addEventListener('submit', function(e){
    e.preventDefault();
    const val = input.value.trim();
    if (!val) return;
    addMessage(val, 'user');
    input.value = '';
    chipsEl.innerHTML = '';
    handleInput(val, false);
  });

  bootConversation();
})();
</script>
</body>
</html>
