<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>Justice</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,500;0,600;0,700;1,500&family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#1C2541;
    --ink-soft:#2E3A5C;
    --paper:#F3EFE6;
    --paper-dim:#EAE4D5;
    --card:#FBF9F4;
    --brass:#A8763E;
    --brass-soft:#C99B5F;
    --seal:#7A2E2E;
    --seal-soft:#9A4646;
    --sage:#4B6455;
    --sage-soft:#6C8A76;
    --slate:#33363D;
    --slate-dim:#6B6E76;
    --line:#D8D0BE;
    --radius:14px;
    --shadow: 0 2px 10px rgba(28,37,65,0.08);
  }
  *{box-sizing:border-box;}
  body{margin:0;background:#dcd5c4;font-family:'Inter',sans-serif;color:var(--slate);}
  .display{font-family:'Lora',serif;}
  .mono{font-family:'JetBrains Mono',monospace;}

  #app-frame{
    max-width:430px;
    margin:0 auto;
    min-height:100vh;
    background:var(--paper);
    position:relative;
    display:flex;
    flex-direction:column;
    overflow-x:hidden;
  }

  /* Top bar */
  .topbar{
    padding:22px 20px 16px;
    background:var(--ink);
    color:var(--paper);
    position:relative;
  }
  .topbar::after{
    content:"";
    position:absolute; left:0; right:0; bottom:-8px; height:8px;
    background:linear-gradient(180deg, rgba(0,0,0,0.12), transparent);
  }
  .brand-row{display:flex; align-items:center; justify-content:space-between;}
  .brand{font-family:'Lora',serif; font-weight:700; font-size:22px; letter-spacing:0.3px; display:flex; align-items:center; gap:8px;}
  .brand .mark{color:var(--brass-soft); font-size:20px;}
  .topbar-sub{font-size:12.5px; color:#B9C0D6; margin-top:4px; font-weight:500;}
  .topbar-sub .mono{color:var(--brass-soft);}

  /* Screen container */
  .screen{ flex:1; padding:20px 18px 100px; display:none; }
  .screen.active{ display:block; animation:fadeIn .25s ease; }
  @keyframes fadeIn{ from{opacity:0; transform:translateY(4px);} to{opacity:1; transform:none;} }

  .section-label{
    font-size:11px; text-transform:uppercase; letter-spacing:1.4px; font-weight:700;
    color:var(--brass); margin:0 0 10px 2px;
  }

  /* Cards */
  .card{
    background:var(--card); border:1px solid var(--line); border-radius:var(--radius);
    padding:16px; margin-bottom:12px; box-shadow:var(--shadow);
  }
  .empty-card{
    border:1.5px dashed var(--line); border-radius:var(--radius); padding:28px 18px;
    text-align:center; color:var(--slate-dim); font-size:14px; background:transparent;
  }

  /* Docket entry (case card) */
  .docket{
    background:var(--card); border:1px solid var(--line); border-radius:var(--radius);
    padding:16px; margin-bottom:12px; box-shadow:var(--shadow); position:relative; overflow:hidden;
  }
  .docket-head{display:flex; justify-content:space-between; align-items:flex-start; gap:10px;}
  .docket-id{font-size:11.5px; color:var(--slate-dim); letter-spacing:0.5px;}
  .docket-cat{font-family:'Lora',serif; font-weight:600; font-size:16.5px; color:var(--ink); margin:3px 0 6px;}
  .docket-desc{font-size:13.5px; color:var(--slate); line-height:1.5; margin-bottom:10px;}
  .docket-meta{display:flex; gap:14px; font-size:12px; color:var(--slate-dim); margin-bottom:10px; flex-wrap:wrap;}
  .docket-meta span{display:flex; align-items:center; gap:4px;}

  .status-chip{
    font-size:10.5px; font-weight:700; letter-spacing:0.6px; text-transform:uppercase;
    padding:4px 9px; border-radius:20px; white-space:nowrap;
  }
  .status-filed{ background:#EFE7D8; color:var(--brass); border:1px solid #DCC9A3; }
  .status-matched{ background:#E4EBE5; color:var(--sage); border:1px solid #BFD1C2; }

  /* Seal stamp */
  .seal{
    position:absolute; top:14px; right:14px; width:52px; height:52px; border-radius:50%;
    border:2.5px solid var(--seal); color:var(--seal); display:flex; align-items:center; justify-content:center;
    font-family:'Lora',serif; font-weight:700; font-size:9px; text-transform:uppercase; letter-spacing:0.5px;
    transform:rotate(-14deg) scale(0); opacity:0; text-align:center; line-height:1.1; padding:2px;
    animation:stamp .5s cubic-bezier(.34,1.56,.64,1) forwards; animation-delay:.15s;
    background:rgba(122,46,46,0.04);
  }
  @keyframes stamp{ to{ transform:rotate(-14deg) scale(1); opacity:0.92; } }

  /* Buttons */
  .btn{
    display:inline-flex; align-items:center; justify-content:center; gap:6px;
    font-family:'Inter',sans-serif; font-weight:600; font-size:14px; letter-spacing:0.1px;
    padding:12px 18px; border-radius:10px; border:none; cursor:pointer; transition:transform .12s ease, opacity .12s ease;
    width:100%;
  }
  .btn:active{ transform:scale(0.98); }
  .btn-primary{ background:var(--ink); color:var(--paper); }
  .btn-brass{ background:var(--brass); color:#fff; }
  .btn-outline{ background:transparent; color:var(--ink); border:1.5px solid var(--ink); }
  .btn-ghost{ background:transparent; color:var(--seal); font-size:13px; padding:8px; width:auto; }
  .btn:disabled{ opacity:0.55; cursor:default; }
  .btn-sm{ width:auto; padding:9px 14px; font-size:13px; }

  /* Forms */
  label{ font-size:12.5px; font-weight:600; color:var(--ink-soft); margin-bottom:6px; display:block; }
  input, select, textarea{
    width:100%; font-family:'Inter',sans-serif; font-size:14.5px; color:var(--slate);
    background:#fff; border:1.5px solid var(--line); border-radius:10px; padding:11px 12px;
    margin-bottom:16px; outline:none;
  }
  input:focus, select:focus, textarea:focus{ border-color:var(--brass); }
  textarea{ resize:vertical; min-height:90px; font-family:'Inter',sans-serif; }

  .chip-select{ display:flex; flex-wrap:wrap; gap:8px; margin-bottom:16px; }
  .chip-opt{
    padding:8px 13px; border-radius:20px; border:1.5px solid var(--line); font-size:13px; font-weight:500;
    cursor:pointer; background:#fff; color:var(--slate);
  }
  .chip-opt.selected{ background:var(--ink); color:var(--paper); border-color:var(--ink); }

  /* Onboarding */
  .onboard-hero{ text-align:center; padding:38px 10px 24px; }
  .onboard-mark{ font-size:38px; color:var(--brass); margin-bottom:6px; }
  .onboard-title{ font-family:'Lora',serif; font-weight:700; font-size:26px; color:var(--ink); margin-bottom:6px; }
  .onboard-tag{ font-size:13.5px; color:var(--slate-dim); line-height:1.5; padding:0 12px; }
  .role-row{ display:flex; gap:12px; margin:22px 0; }
  .role-card{
    flex:1; border:1.5px solid var(--line); border-radius:var(--radius); padding:18px 12px; text-align:center;
    background:var(--card); cursor:pointer;
  }
  .role-card.selected{ border-color:var(--brass); background:#FBF3E4; }
  .role-icon{ font-size:24px; margin-bottom:8px; }
  .role-name{ font-weight:700; font-size:14px; color:var(--ink); margin-bottom:3px; }
  .role-desc{ font-size:11.5px; color:var(--slate-dim); }

  /* Bottom nav */
  .bottomnav{
    position:fixed; bottom:0; left:50%; transform:translateX(-50%);
    width:100%; max-width:430px; background:var(--card); border-top:1px solid var(--line);
    display:flex; padding:10px 8px calc(10px + env(safe-area-inset-bottom));
    box-shadow:0 -4px 14px rgba(28,37,65,0.06); z-index:20;
  }
  .navbtn{
    flex:1; background:none; border:none; display:flex; flex-direction:column; align-items:center; gap:3px;
    color:var(--slate-dim); font-size:10.5px; font-weight:600; cursor:pointer; padding:6px 4px;
  }
  .navbtn.active{ color:var(--ink); }
  .navbtn .ic{ font-size:19px; }

  .fab{
    position:fixed; bottom:78px; left:50%; transform:translateX(calc(-50% + 155px));
    width:54px; height:54px; border-radius:50%; background:var(--seal); color:#fff; border:none;
    font-size:26px; box-shadow:0 4px 14px rgba(122,46,46,0.35); cursor:pointer; z-index:25;
    display:flex; align-items:center; justify-content:center;
  }

  .toast{
    position:fixed; bottom:96px; left:50%; transform:translateX(-50%);
    background:var(--ink); color:var(--paper); padding:11px 18px; border-radius:10px; font-size:13px;
    z-index:60; box-shadow:0 4px 16px rgba(0,0,0,0.2); opacity:0; pointer-events:none; transition:opacity .25s ease;
    max-width:340px; text-align:center;
  }
  .toast.show{ opacity:1; }

  .lawyer-row{
    display:flex; justify-content:space-between; align-items:center; padding:10px 0;
    border-bottom:1px solid var(--line);
  }
  .lawyer-row:last-child{ border-bottom:none; }
  .lawyer-name{ font-weight:600; font-size:14px; color:var(--ink); }
  .lawyer-sub{ font-size:12px; color:var(--slate-dim); }

  .backrow{ display:flex; align-items:center; gap:8px; margin-bottom:16px; cursor:pointer; color:var(--slate-dim); font-size:13px; font-weight:600; }

  .header-row{ display:flex; justify-content:space-between; align-items:center; margin-bottom:16px; }
  .profile-field{ display:flex; justify-content:space-between; padding:12px 0; border-bottom:1px solid var(--line); font-size:14px; }
  .profile-field:last-child{ border-bottom:none; }
  .profile-field .k{ color:var(--slate-dim); }
  .profile-field .v{ font-weight:600; color:var(--ink); }

  .filter-row{ display:flex; gap:8px; margin-bottom:16px; }
  .filter-btn{
    flex:1; padding:9px; border-radius:9px; border:1.5px solid var(--line); background:var(--card);
    font-size:12.5px; font-weight:600; color:var(--slate-dim); cursor:pointer;
  }
  .filter-btn.active{ background:var(--ink); color:var(--paper); border-color:var(--ink); }

  .spinner{
    width:22px; height:22px; border-radius:50%; border:2.5px solid var(--line); border-top-color:var(--brass);
    animation:spin .7s linear infinite; margin:30px auto;
  }
  @keyframes spin{ to{ transform:rotate(360deg); } }
</style>
</head>
<body>
<div id="app-frame">

  <!-- ONBOARDING -->
  <div class="screen active" id="screen-onboard">
    <div class="onboard-hero">
      <div class="onboard-mark">&#9878;</div>
      <div class="onboard-title">Justice</div>
      <div class="onboard-tag">File a case. Get matched with a lawyer.<br>No fees to search, no waiting rooms.</div>
    </div>
    <div class="role-row">
      <div class="role-card" id="role-client" onclick="selectRole('client')">
        <div class="role-icon">&#128100;</div>
        <div class="role-name">I need a lawyer</div>
        <div class="role-desc">File a case, review matches</div>
      </div>
      <div class="role-card" id="role-lawyer" onclick="selectRole('lawyer')">
        <div class="role-icon">&#9878;</div>
        <div class="role-name">I'm a lawyer</div>
        <div class="role-desc">Browse open cases</div>
      </div>
    </div>
    <div id="onboard-fields" style="display:none;">
      <label>Your name</label>
      <input type="text" id="ob-name" placeholder="e.g. Arbaaz Ahmed">
      <div id="ob-lawyer-fields" style="display:none;">
        <label>Practice area</label>
        <div class="chip-select" id="ob-specialty-chips"></div>
        <label>Based in</label>
        <input type="text" id="ob-location" placeholder="e.g. Tinsukia, Assam">
      </div>
      <div id="ob-client-fields" style="display:none;">
        <label>Location</label>
        <input type="text" id="ob-location-client" placeholder="e.g. Tinsukia, Assam">
      </div>
      <button class="btn btn-primary" id="ob-continue" onclick="completeOnboarding()">Enter Justice</button>
    </div>
  </div>

  <!-- CLIENT HOME -->
  <div class="screen" id="screen-client-home">
    <div class="topbar">
      <div class="brand-row">
        <div class="brand"><span class="mark">&#9878;</span>Justice</div>
      </div>
      <div class="topbar-sub">Welcome back, <span id="ch-name" class="mono"></span></div>
    </div>
    <div style="padding:18px 18px 100px;">
      <div class="section-label">My Filed Cases</div>
      <div id="client-case-list"><div class="spinner"></div></div>
    </div>
  </div>

  <!-- NEW CASE FORM -->
  <div class="screen" id="screen-new-case">
    <div style="padding-top:20px;">
      <div class="backrow" onclick="goTo('client-home')">&#8592; Back</div>
      <div class="section-label">File a New Case</div>
      <label>What kind of matter is this?</label>
      <div class="chip-select" id="nc-category-chips"></div>
      <label>Describe your situation</label>
      <textarea id="nc-desc" placeholder="Give the key facts — what happened, who's involved, what you need help with."></textarea>
      <label>How urgent is this?</label>
      <div class="chip-select" id="nc-urgency-chips"></div>
      <button class="btn btn-brass" onclick="submitCase()">File Case</button>
    </div>
  </div>

  <!-- CASE CONFIRMATION -->
  <div class="screen" id="screen-case-filed">
    <div style="padding-top:60px; text-align:center;">
      <div style="font-size:44px; margin-bottom:6px;">&#128220;</div>
      <div class="display" style="font-size:20px; font-weight:700; color:var(--ink); margin-bottom:8px;">Case Filed</div>
      <div class="mono" style="font-size:15px; color:var(--brass); font-weight:600; margin-bottom:14px;" id="filed-case-id"></div>
      <div style="font-size:13.5px; color:var(--slate-dim); padding:0 30px; margin-bottom:26px;">
        Your case is now on the docket. Lawyers matching your practice area will be notified and can express interest.
      </div>
      <button class="btn btn-primary" onclick="goTo('client-home')">View My Cases</button>
    </div>
  </div>

  <!-- CASE DETAIL (client view) -->
  <div class="screen" id="screen-case-detail">
    <div style="padding-top:20px;">
      <div class="backrow" onclick="goTo('client-home')">&#8592; Back to my cases</div>
      <div id="case-detail-content"></div>
    </div>
  </div>

  <!-- LAWYER HOME (docket) -->
  <div class="screen" id="screen-lawyer-home">
    <div class="topbar">
      <div class="brand-row">
        <div class="brand"><span class="mark">&#9878;</span>Justice</div>
      </div>
      <div class="topbar-sub">Docket for <span id="lh-name" class="mono"></span></div>
    </div>
    <div style="padding:18px 18px 100px;">
      <div class="filter-row">
        <button class="filter-btn active" id="filter-my-specialty" onclick="setLawyerFilter('mine')">My Specialty</button>
        <button class="filter-btn" id="filter-all" onclick="setLawyerFilter('all')">All Cases</button>
      </div>
      <div class="section-label">Open Cases</div>
      <div id="lawyer-case-list"><div class="spinner"></div></div>
    </div>
  </div>

  <!-- PROFILE -->
  <div class="screen" id="screen-profile">
    <div class="topbar">
      <div class="brand-row"><div class="brand"><span class="mark">&#9878;</span>Justice</div></div>
      <div class="topbar-sub">Your profile</div>
    </div>
    <div style="padding:18px;">
      <div class="card" id="profile-card"></div>
      <button class="btn btn-ghost" onclick="resetIdentity()">Switch role / start over</button>
    </div>
  </div>

  <!-- Bottom nav -->
  <div class="bottomnav" id="bottomnav" style="display:none;">
    <button class="navbtn active" id="nav-home" onclick="onNavHome()"><span class="ic">&#8962;</span>Home</button>
    <button class="navbtn" id="nav-profile" onclick="goTo('profile')"><span class="ic">&#9776;</span>Profile</button>
  </div>
  <button class="fab" id="fab-new-case" style="display:none;" onclick="goTo('new-case')">+</button>

  <div class="toast" id="toast"></div>
</div>

<script>
const CATEGORIES = ["Family Law","Property & Land","Criminal Defense","Business & Contracts","Consumer Rights","Other"];
const URGENCY = ["Standard","Time-sensitive","Urgent"];

let identity = null;
let selectedRole = null;
let currentCaseId = null;
let lawyerFilterMode = 'mine';
let newCaseCategory = null;
let newCaseUrgency = null;

function showToast(msg){
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  setTimeout(()=> t.classList.remove('show'), 2200);
}

function goTo(screenKey){
  document.querySelectorAll('.screen').forEach(s => s.classList.remove('active'));
  document.getElementById('screen-' + screenKey).classList.add('active');
  document.querySelectorAll('.navbtn').forEach(b => b.classList.remove('active'));
  if(screenKey === 'client-home' || screenKey === 'lawyer-home'){
    document.getElementById('nav-home').classList.add('active');
    document.getElementById('bottomnav').style.display = 'flex';
  } else if(screenKey === 'profile'){
    document.getElementById('nav-profile').classList.add('active');
    document.getElementById('bottomnav').style.display = 'flex';
  } else {
    document.getElementById('bottomnav').style.display = 'none';
  }
  document.getElementById('fab-new-case').style.display = (screenKey === 'client-home' && identity && identity.role === 'client') ? 'flex' : 'none';

  if(screenKey === 'client-home') renderClientCases();
  if(screenKey === 'lawyer-home') renderLawyerDocket();
  if(screenKey === 'profile') renderProfile();
}

function onNavHome(){
  goTo(identity.role === 'client' ? 'client-home' : 'lawyer-home');
}

function selectRole(role){
  selectedRole = role;
  document.getElementById('role-client').classList.toggle('selected', role === 'client');
  document.getElementById('role-lawyer').classList.toggle('selected', role === 'lawyer');
  document.getElementById('onboard-fields').style.display = 'block';
  document.getElementById('ob-lawyer-fields').style.display = role === 'lawyer' ? 'block' : 'none';
  document.getElementById('ob-client-fields').style.display = role === 'client' ? 'block' : 'none';
  if(role === 'lawyer' && document.getElementById('ob-specialty-chips').children.length === 0){
    buildChips('ob-specialty-chips', CATEGORIES, (val) => { obSpecialty = val; });
  }
}
let obSpecialty = null;
function buildChips(containerId, options, onSelect){
  const el = document.getElementById(containerId);
  el.innerHTML = '';
  options.forEach(opt => {
    const chip = document.createElement('div');
    chip.className = 'chip-opt';
    chip.textContent = opt;
    chip.onclick = () => {
      el.querySelectorAll('.chip-opt').forEach(c => c.classList.remove('selected'));
      chip.classList.add('selected');
      onSelect(opt);
    };
    el.appendChild(chip);
  });
}

async function completeOnboarding(){
  const name = document.getElementById('ob-name').value.trim();
  if(!selectedRole){ showToast('Choose a role first'); return; }
  if(!name){ showToast('Enter your name'); return; }
  let location = '';
  if(selectedRole === 'lawyer'){
    if(!obSpecialty){ showToast('Choose a practice area'); return; }
    location = document.getElementById('ob-location').value.trim();
  } else {
    location = document.getElementById('ob-location-client').value.trim();
  }
  identity = {
    id: 'u-' + crypto.randomUUID().slice(0,8),
    role: selectedRole,
    name: name,
    specialty: selectedRole === 'lawyer' ? obSpecialty : null,
    location: location || 'Not specified',
    joinedAt: Date.now()
  };
  try{
    await window.storage.set('identity', JSON.stringify(identity), false);
  }catch(e){ console.error('Storage error saving identity', e); }
  enterApp();
}

function enterApp(){
  if(identity.role === 'client'){
    document.getElementById('ch-name').textContent = identity.name;
    goTo('client-home');
  } else {
    document.getElementById('lh-name').textContent = identity.name + ' \u2014 ' + identity.specialty;
    goTo('lawyer-home');
  }
}

async function loadIdentity(){
  try{
    const res = await window.storage.get('identity', false);
    if(res && res.value){
      identity = JSON.parse(res.value);
      enterApp();
    }
  }catch(e){
    // no identity yet, stay on onboarding
  }
}

async function resetIdentity(){
  try{ await window.storage.delete('identity', false); }catch(e){}
  identity = null; selectedRole = null; obSpecialty = null;
  document.getElementById('ob-name').value = '';
  document.getElementById('onboard-fields').style.display = 'none';
  document.getElementById('role-client').classList.remove('selected');
  document.getElementById('role-lawyer').classList.remove('selected');
  goTo('onboard');
}

// ---- New Case ----
document.addEventListener('DOMContentLoaded', () => {
  buildChips('nc-category-chips', CATEGORIES, (v) => newCaseCategory = v);
  buildChips('nc-urgency-chips', URGENCY, (v) => newCaseUrgency = v);
  loadIdentity();
});

async function submitCase(){
  const desc = document.getElementById('nc-desc').value.trim();
  if(!newCaseCategory){ showToast('Select a case category'); return; }
  if(!desc || desc.length < 8){ showToast('Add a bit more detail'); return; }
  if(!newCaseUrgency){ showToast('Select urgency'); return; }

  const id = 'JN-2026-' + String(Date.now()).slice(-4);
  const caseObj = {
    id: id,
    category: newCaseCategory,
    description: desc,
    urgency: newCaseUrgency,
    location: identity.location,
    clientId: identity.id,
    clientName: identity.name,
    status: 'filed',
    createdAt: Date.now(),
    interestedLawyers: []
  };
  try{
    const result = await window.storage.set('case:' + id, JSON.stringify(caseObj), true);
    if(!result){ showToast('Could not file case — try again'); return; }
  }catch(e){
    console.error('Storage error filing case', e);
    showToast('Could not file case — try again');
    return;
  }
  document.getElementById('filed-case-id').textContent = id;
  document.getElementById('nc-desc').value = '';
  newCaseCategory = null; newCaseUrgency = null;
  document.querySelectorAll('#nc-category-chips .chip-opt, #nc-urgency-chips .chip-opt').forEach(c => c.classList.remove('selected'));
  goTo('case-filed');
}

// ---- Client: list own cases ----
async function fetchAllCases(){
  try{
    const listRes = await window.storage.list('case:', true);
    if(!listRes || !listRes.keys) return [];
    const cases = [];
    for(const key of listRes.keys){
      try{
        const r = await window.storage.get(key, true);
        if(r && r.value) cases.push(JSON.parse(r.value));
      }catch(e){ /* skip missing */ }
    }
    return cases.sort((a,b) => b.createdAt - a.createdAt);
  }catch(e){
    console.error('Error listing cases', e);
    return [];
  }
}

async function renderClientCases(){
  const container = document.getElementById('client-case-list');
  container.innerHTML = '<div class="spinner"></div>';
  const all = await fetchAllCases();
  const mine = all.filter(c => c.clientId === identity.id);
  if(mine.length === 0){
    container.innerHTML = '<div class="empty-card">No cases filed yet.<br>Tap the + button to file your first case.</div>';
    return;
  }
  container.innerHTML = '';
  mine.forEach(c => {
    const matched = c.interestedLawyers && c.interestedLawyers.length > 0;
    const div = document.createElement('div');
    div.className = 'docket';
    div.onclick = () => openCaseDetail(c.id);
    div.innerHTML = `
      ${matched ? `<div class="seal">${c.interestedLawyers.length} LAWYER${c.interestedLawyers.length>1?'S':''}<br>MATCHED</div>` : ''}
      <div class="docket-head">
        <div class="docket-id mono">${c.id}</div>
      </div>
      <div class="docket-cat">${c.category}</div>
      <div class="docket-desc">${escapeHtml(c.description).slice(0,110)}${c.description.length>110?'…':''}</div>
      <div class="docket-meta">
        <span>&#128205; ${escapeHtml(c.location)}</span>
        <span>&#9201; ${c.urgency}</span>
      </div>
      <span class="status-chip ${matched ? 'status-matched' : 'status-filed'}">${matched ? 'Matched' : 'Awaiting Match'}</span>
    `;
    container.appendChild(div);
  });
}

async function openCaseDetail(caseId){
  currentCaseId = caseId;
  const content = document.getElementById('case-detail-content');
  content.innerHTML = '<div class="spinner"></div>';
  goTo('case-detail');
  try{
    const r = await window.storage.get('case:' + caseId, true);
    const c = JSON.parse(r.value);
    const lawyers = c.interestedLawyers || [];
    content.innerHTML = `
      <div class="docket" style="margin-bottom:18px;">
        <div class="docket-id mono">${c.id}</div>
        <div class="docket-cat">${c.category}</div>
        <div class="docket-desc">${escapeHtml(c.description)}</div>
        <div class="docket-meta">
          <span>&#128205; ${escapeHtml(c.location)}</span>
          <span>&#9201; ${c.urgency}</span>
        </div>
      </div>
      <div class="section-label">Interested Lawyers</div>
      ${lawyers.length === 0
        ? '<div class="empty-card">No lawyers have responded yet. Cases are usually reviewed within a day.</div>'
        : lawyers.map(l => `
          <div class="card">
            <div class="lawyer-row" style="border:none; padding:0;">
              <div>
                <div class="lawyer-name">${escapeHtml(l.name)}</div>
                <div class="lawyer-sub">${escapeHtml(l.specialty)} &middot; ${escapeHtml(l.location)}</div>
              </div>
              <button class="btn btn-outline btn-sm" onclick="showToast('In the full version, this opens a direct message thread.')">Contact</button>
            </div>
          </div>
        `).join('')
      }
    `;
  }catch(e){
    console.error(e);
    content.innerHTML = '<div class="empty-card">Could not load this case.</div>';
  }
}

// ---- Lawyer: docket ----
function setLawyerFilter(mode){
  lawyerFilterMode = mode;
  document.getElementById('filter-my-specialty').classList.toggle('active', mode === 'mine');
  document.getElementById('filter-all').classList.toggle('active', mode === 'all');
  renderLawyerDocket();
}

async function renderLawyerDocket(){
  const container = document.getElementById('lawyer-case-list');
  container.innerHTML = '<div class="spinner"></div>';
  const all = await fetchAllCases();
  const filtered = lawyerFilterMode === 'mine'
    ? all.filter(c => c.category === identity.specialty)
    : all;
  if(filtered.length === 0){
    container.innerHTML = '<div class="empty-card">No open cases right now. Check back soon, or switch to "All Cases".</div>';
    return;
  }
  container.innerHTML = '';
  filtered.forEach(c => {
    const alreadyIn = (c.interestedLawyers || []).some(l => l.lawyerId === identity.id);
    const div = document.createElement('div');
    div.className = 'docket';
    div.innerHTML = `
      <div class="docket-head">
        <div class="docket-id mono">${c.id}</div>
        <span class="status-chip ${c.interestedLawyers.length ? 'status-matched' : 'status-filed'}">${c.interestedLawyers.length} interested</span>
      </div>
      <div class="docket-cat">${c.category}</div>
      <div class="docket-desc">${escapeHtml(c.description)}</div>
      <div class="docket-meta">
        <span>&#128205; ${escapeHtml(c.location)}</span>
        <span>&#9201; ${c.urgency}</span>
      </div>
      <button class="btn ${alreadyIn ? 'btn-outline' : 'btn-brass'} btn-sm" ${alreadyIn ? 'disabled' : ''} onclick="expressInterest('${c.id}', this)">
        ${alreadyIn ? 'Interest Sent' : 'Express Interest'}
      </button>
    `;
    container.appendChild(div);
  });
}

async function expressInterest(caseId, btn){
  btn.disabled = true;
  btn.textContent = 'Sending…';
  try{
    const r = await window.storage.get('case:' + caseId, true);
    const c = JSON.parse(r.value);
    if(!c.interestedLawyers.some(l => l.lawyerId === identity.id)){
      c.interestedLawyers.push({
        lawyerId: identity.id,
        name: identity.name,
        specialty: identity.specialty,
        location: identity.location
      });
      c.status = 'matched';
    }
    await window.storage.set('case:' + caseId, JSON.stringify(c), true);
    showToast('Interest sent to ' + c.clientName);
    renderLawyerDocket();
  }catch(e){
    console.error(e);
    showToast('Could not send interest — try again');
    btn.disabled = false;
    btn.textContent = 'Express Interest';
  }
}

// ---- Profile ----
function renderProfile(){
  const card = document.getElementById('profile-card');
  if(identity.role === 'client'){
    card.innerHTML = `
      <div class="profile-field"><span class="k">Name</span><span class="v">${escapeHtml(identity.name)}</span></div>
      <div class="profile-field"><span class="k">Role</span><span class="v">Client</span></div>
      <div class="profile-field"><span class="k">Location</span><span class="v">${escapeHtml(identity.location)}</span></div>
    `;
  } else {
    card.innerHTML = `
      <div class="profile-field"><span class="k">Name</span><span class="v">${escapeHtml(identity.name)}</span></div>
      <div class="profile-field"><span class="k">Role</span><span class="v">Lawyer</span></div>
      <div class="profile-field"><span class="k">Practice area</span><span class="v">${escapeHtml(identity.specialty)}</span></div>
      <div class="profile-field"><span class="k">Location</span><span class="v">${escapeHtml(identity.location)}</span></div>
    `;
  }
}

function escapeHtml(str){
  const d = document.createElement('div');
  d.textContent = str || '';
  return d.innerHTML;
}
</script>
</body>
</html>
