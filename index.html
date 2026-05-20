<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kizaru One Point On</title>
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }
body {
  width: 100%; min-height: 100vh;
  background: #090909;
  font-family: Arial, sans-serif;
  color: white;
  overflow: hidden;
}
.screen {
  position: absolute; width: 100%; min-height: 100vh;
  display: flex; flex-direction: column;
  align-items: center; justify-content: center;
  padding: 2rem; transition: all 0.8s ease;
}
.screen.hidden { opacity: 0; pointer-events: none; transform: translateX(-120%); }
.screen.fadeout { opacity: 0; pointer-events: none; }
#typingText {
  font-size: 28px; color: cyan;
  text-shadow: 0 0 20px cyan;
  margin-bottom: 30px; text-align: center;
}
.btn-cyan {
  padding: 12px 32px; border: none; border-radius: 14px;
  background: cyan; color: black; font-size: 17px; font-weight: bold;
  cursor: pointer; transition: transform 0.2s, opacity 0.4s;
}
.btn-cyan:hover { transform: scale(1.07); }
.btn-cyan:disabled { opacity: 0.35; cursor: not-allowed; transform: none; }
.fade-text { font-size: 24px; color: white; text-align: center; animation: fadeIn 1.5s forwards; }
@keyframes fadeIn { from { opacity:0; transform:translateY(20px); } to { opacity:1; transform:translateY(0); } }
.glow-title {
  font-size: 38px; color: cyan;
  text-shadow: 0 0 10px cyan, 0 0 30px cyan;
  margin-bottom: 24px; animation: glow 2s infinite alternate;
}
@keyframes glow {
  from { text-shadow: 0 0 10px cyan, 0 0 20px cyan; }
  to { text-shadow: 0 0 20px cyan, 0 0 50px cyan; }
}
#namaInput {
  width: 280px; padding: 13px; border-radius: 12px;
  font-size: 17px; text-align: center; outline: none;
  margin-bottom: 14px; background: #1a1a1a;
  color: white; border: 1.5px solid cyan;
}

/* MAIN APP */
#mainApp { display: none; flex-direction: column; width: 100%; height: 100vh; }

/* TOP BAR */
.topbar {
  background: #0a0a0a; border-bottom: 1px solid #1a1a1a;
  padding: 12px 20px; display: flex; align-items: center; gap: 12px; flex-shrink: 0;
}
.topbar-logo {
  width: 38px; height: 38px; border-radius: 50%;
  background: linear-gradient(135deg, cyan, #003040);
  display: flex; align-items: center; justify-content: center;
  font-weight: bold; font-size: 14px; color: #000;
}
.topbar-name { font-size: 18px; font-weight: bold; color: cyan; text-shadow: 0 0 10px rgba(0,255,255,0.4); }
.topbar-sub { font-size: 11px; color: #555; }
.topbar-user { margin-left: auto; display: flex; align-items: center; gap: 8px; }
.topbar-avatar {
  width: 32px; height: 32px; border-radius: 50%;
  background: #005f6b; display: flex; align-items: center;
  justify-content: center; font-size: 12px; font-weight: bold; color: cyan;
}
.topbar-uname { font-size: 13px; color: #aaa; }
.logout-btn {
  background: none; border: 1px solid #333; border-radius: 8px;
  color: #666; font-size: 11px; padding: 4px 10px; cursor: pointer;
}
.logout-btn:hover { border-color: #f55; color: #f55; }

/* CONTENT */
.content { display: flex; flex: 1; overflow: hidden; }

/* VOTE AREA */
.vote-area {
  flex: 1; display: flex; flex-direction: column;
  align-items: center; justify-content: center;
  padding: 2rem 1.5rem; overflow-y: auto;
}
.vote-title { font-size: 28px; color: cyan; text-shadow: 0 0 15px cyan; margin-bottom: 4px; animation: glow 2s infinite alternate; }
.vote-sub { font-size: 13px; color: #777; margin-bottom: 10px; }
.greet { font-size: 14px; color: #aaa; margin-bottom: 18px; }
.greet span { color: cyan; font-weight: bold; }
.vote-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 14px; width: 100%; max-width: 380px; margin-bottom: 16px; }
.vote-card {
  background: #111; border: 1.5px solid #333; border-radius: 14px;
  padding: 16px 10px; display: flex; flex-direction: column;
  align-items: center; gap: 8px; cursor: pointer; transition: all 0.22s; position: relative;
}
.vote-card:hover:not(.dis) { border-color: cyan; transform: scale(1.05); }
.vote-card.voted-here { border-color: lime; background: #0a1f0a; box-shadow: 0 0 16px rgba(0,255,100,0.2); }
.vote-card.dis { opacity: 0.45; cursor: not-allowed; }
.role-icon { font-size: 30px; }
.role-name { font-size: 13px; font-weight: bold; }
.role-count { font-size: 18px; font-weight: bold; }
.role-lbl { font-size: 11px; color: #666; }
.vbadge {
  position: absolute; top: -8px; right: -8px;
  background: lime; color: black; font-size: 10px; font-weight: bold;
  border-radius: 50%; width: 20px; height: 20px;
  display: flex; align-items: center; justify-content: center;
}
.voted-msg { font-size: 13px; color: lime; min-height: 18px; text-align: center; }

/* CHAT PANEL */
.chat-panel {
  width: 290px; min-width: 270px;
  background: #0e0e0e; border-left: 1px solid #1a1a1a;
  display: flex; flex-direction: column;
}
.chat-header {
  padding: 12px 16px; border-bottom: 1px solid #1a1a1a;
  display: flex; align-items: center; gap: 8px;
}
.chat-hname { font-size: 14px; font-weight: bold; color: cyan; }
.online-dot { width: 7px; height: 7px; border-radius: 50%; background: lime; margin-left: auto; }
.chat-msgs {
  flex: 1; overflow-y: auto; padding: 12px;
  display: flex; flex-direction: column; gap: 10px;
  scrollbar-width: thin; scrollbar-color: #222 transparent;
}
.msg { display: flex; flex-direction: column; max-width: 90%; }
.msg.mine { align-self: flex-end; align-items: flex-end; }
.msg.other { align-self: flex-start; align-items: flex-start; }
.msg-sender { font-size: 10px; color: #555; margin-bottom: 2px; }
.msg.mine .msg-sender { color: #0aa; }
.msg-bubble { padding: 7px 11px; border-radius: 13px; font-size: 13px; line-height: 1.5; word-break: break-word; }
.msg.mine .msg-bubble { background: #005f6b; color: #e0ffff; border-bottom-right-radius: 3px; }
.msg.other .msg-bubble { background: #1a1a1a; color: #ddd; border-bottom-left-radius: 3px; }
.msg-time { font-size: 10px; color: #444; margin-top: 2px; }
.sys-msg { text-align: center; font-size: 11px; color: #555; padding: 4px 0; }
.chat-input-row {
  padding: 10px 12px; border-top: 1px solid #1a1a1a;
  display: flex; gap: 8px; align-items: center;
}
.chat-input-row input {
  flex: 1; background: #1a1a1a; border: 1px solid #2a2a2a;
  border-radius: 20px; padding: 8px 13px; color: white; font-size: 13px; outline: none;
}
.chat-input-row input:focus { border-color: cyan; }
.chat-send {
  width: 32px; height: 32px; border-radius: 50%;
  background: cyan; border: none; cursor: pointer;
  font-size: 14px; flex-shrink: 0; transition: transform 0.15s;
}
.chat-send:hover { transform: scale(1.1); }
</style>
</head>
<body>

<div id="app">
  <div class="screen" id="s1">
    <div id="typingText"></div>
    <button class="btn-cyan" id="cont1" style="opacity:0" onclick="goS2()">Continue</button>
  </div>
  <div class="screen hidden" id="s2">
    <div class="fade-text">Terimakasih Telah Menjoin Kizaru One Point On</div>
  </div>
  <div class="screen hidden" id="s3">
    <div class="glow-title">LOGIN</div>
    <input type="text" id="namaInput" placeholder="Masukkan Nama"
      oninput="checkNama()"
      onkeydown="if(event.key==='Enter')doLogin()" />
    <button class="btn-cyan" id="loginBtn" disabled onclick="doLogin()">Continue</button>
  </div>
</div>

<div id="mainApp">
  <div class="topbar">
    <div class="topbar-logo">K</div>
    <div>
      <div class="topbar-name">⚡ KNOX Chat Group</div>
      <div class="topbar-sub">Kizaru One Point On</div>
    </div>
    <div class="topbar-user">
      <div class="topbar-avatar" id="topAvatar"></div>
      <div class="topbar-uname" id="topName"></div>
      <button class="logout-btn" onclick="doLogout()">Logout</button>
    </div>
  </div>
  <div class="content">
    <div class="vote-area">
      <div class="vote-title">VOTE ROLE</div>
      <div class="vote-sub" id="vsub">Pilih 1 role untukmu — tidak bisa diubah</div>
      <div class="greet" id="greet"></div>
      <div class="vote-grid" id="vgrid"></div>
      <div class="voted-msg" id="vmsg"></div>
    </div>
    <div class="chat-panel">
      <div class="chat-header">
        <span style="font-size:16px;">#</span>
        <span class="chat-hname">knox-general</span>
        <div class="online-dot"></div>
      </div>
      <div class="chat-msgs" id="chatMsgs">
        <div class="sys-msg">Menghubungkan ke server...</div>
      </div>
      <div class="chat-input-row">
        <input type="text" id="chatInput" placeholder="Ketik pesan..."
          onkeydown="if(event.key==='Enter')sendMsg()" />
        <button class="chat-send" onclick="sendMsg()">&#9658;</button>
      </div>
    </div>
  </div>
</div>

<!-- FIREBASE SDK -->
<script src="https://www.gstatic.com/firebasejs/9.22.2/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/9.22.2/firebase-database-compat.js"></script>

<script>
// =====================
// FIREBASE CONFIG
// =====================
var firebaseConfig = {
  apiKey: "AIzaSyB27AFZBoMgq1K9Yweb6g9gDOgU-r280M8",
  authDomain: "kizaru-html.firebaseapp.com",
  databaseURL: "https://kizaru-html-default-rtdb.asia-southeast1.firebasedatabase.app",
  projectId: "kizaru-html",
  storageBucket: "kizaru-html.firebasestorage.app",
  messagingSenderId: "908867741214",
  appId: "1:908867741214:web:b5232294692ea019bbf00f"
};
firebase.initializeApp(firebaseConfig);
var db = firebase.database();

// =====================
// ROLES
// =====================
var roles = [
  { id:'support', icon:'🛡️', name:'Support', color:'#0af' },
  { id:'spy',     icon:'🕵️', name:'Spy',     color:'#f0a' },
  { id:'knight',  icon:'⚔️', name:'Knight',  color:'#fa0' },
  { id:'builder', icon:'🏗️', name:'Builder', color:'#0fa' }
];

var userName = '';
var userVote = null;

// =====================
// LOCAL SESSION SAVE
// =====================
function saveSession() {
  localStorage.setItem('knox_session', JSON.stringify({ name: userName, vote: userVote }));
}
function loadSession() {
  try { var s = localStorage.getItem('knox_session'); return s ? JSON.parse(s) : null; }
  catch(e) { return null; }
}
function clearSession() { localStorage.removeItem('knox_session'); }

// =====================
// TIME
// =====================
function getTime() {
  var d = new Date();
  return d.getHours().toString().padStart(2,'0') + ':' + d.getMinutes().toString().padStart(2,'0');
}

// =====================
// TYPING
// =====================
var welcomeText = "Selamat datang Di Pengambilan Role.";
var ti = 0;
function ketik() {
  if (ti < welcomeText.length) {
    document.getElementById('typingText').innerHTML += welcomeText.charAt(ti++);
    setTimeout(ketik, 70);
  } else {
    document.getElementById('cont1').style.opacity = '1';
  }
}

// =====================
// INIT
// =====================
function init() {
  ketik();
  var s = loadSession();
  if (s && s.name) {
    userName = s.name;
    userVote = s.vote || null;
    enterMain(true);
  }
}
init();

// =====================
// SCREEN FLOW
// =====================
function goS2() {
  showScreen('s1','s2');
  setTimeout(function() {
    document.getElementById('s2').classList.add('fadeout');
    setTimeout(function() { showScreen('s2','s3'); }, 800);
  }, 3000);
}
function showScreen(a, b) {
  document.getElementById(a).classList.add('hidden');
  document.getElementById(a).classList.remove('fadeout');
  document.getElementById(b).classList.remove('hidden','fadeout');
}
function checkNama() {
  document.getElementById('loginBtn').disabled = document.getElementById('namaInput').value.trim().length === 0;
}
function doLogin() {
  var nama = document.getElementById('namaInput').value.trim();
  if (!nama) return;
  userName = nama;
  db.ref('users/' + userName).once('value', function(snap) {
    var data = snap.val();
    if (data && data.vote) {
      userVote = data.vote;
      enterMain(true);
    } else {
      userVote = null;
      enterMain(false);
    }
  });
}

// =====================
// MAIN APP
// =====================
function enterMain(isReturn) {
  document.getElementById('app').style.display = 'none';
  document.getElementById('mainApp').style.display = 'flex';
  document.getElementById('topName').textContent = userName;
  document.getElementById('topAvatar').textContent = userName.charAt(0).toUpperCase();
  document.getElementById('greet').innerHTML = isReturn
    ? '👋 Selamat Kembali, <span>' + userName + '</span>!'
    : 'Halo, <span>' + userName + '</span>! Pilih role kamu:';
  saveSession();
  listenVotes();
  listenChat();
}

function doLogout() {
  clearSession();
  location.reload();
}

// =====================
// VOTE - REALTIME
// =====================
function listenVotes() {
  db.ref('votes').on('value', function(snap) {
    var votes = snap.val() || { support:0, spy:0, knight:0, builder:0 };
    renderVotes(votes);
  });
}

function renderVotes(votes) {
  var grid = document.getElementById('vgrid');
  grid.innerHTML = '';
  roles.forEach(function(r) {
    var c = document.createElement('div');
    c.className = 'vote-card' +
      (userVote === r.id ? ' voted-here' : '') +
      (userVote && userVote !== r.id ? ' dis' : '');
    if (!userVote) {
      (function(rid) { c.onclick = function() { castVote(rid); }; })(r.id);
    }
    c.innerHTML =
      (userVote === r.id ? '<div class="vbadge">✓</div>' : '') +
      '<div class="role-icon">' + r.icon + '</div>' +
      '<div class="role-name" style="color:' + r.color + '">' + r.name + '</div>' +
      '<div class="role-count">' + (votes[r.id] || 0) + '</div>' +
      '<div class="role-lbl">votes</div>';
    grid.appendChild(c);
  });
  if (userVote) {
    var p = roles.find(function(r) { return r.id === userVote; });
    document.getElementById('vmsg').textContent = '✅ Role kamu: ' + p.name + ' — tidak bisa diubah.';
    document.getElementById('vsub').textContent = 'Hasil vote saat ini:';
  }
}

function castVote(id) {
  if (userVote) return;
  userVote = id;
  saveSession();
  db.ref('users/' + userName).set({ vote: id });
  db.ref('votes/' + id).transaction(function(val) { return (val || 0) + 1; });
  var p = roles.find(function(r) { return r.id === id; });
  postSysMsg('🎯 ' + userName + ' memilih role ' + p.icon + ' ' + p.name + '!');
}

// =====================
// CHAT - REALTIME
// =====================
function listenChat() {
  var box = document.getElementById('chatMsgs');
  box.innerHTML = '';
  db.ref('chat').limitToLast(100).on('child_added', function(snap) {
    var m = snap.val();
    appendMsgEl(m);
    box.scrollTop = box.scrollHeight;
  });
}

function appendMsgEl(m) {
  var box = document.getElementById('chatMsgs');
  if (m.sender === '__system__') {
    var d = document.createElement('div');
    d.className = 'sys-msg';
    d.textContent = m.text;
    box.appendChild(d);
    return;
  }
  var isMe = (m.sender === userName);
  var div = document.createElement('div');
  div.className = 'msg ' + (isMe ? 'mine' : 'other');
  div.innerHTML =
    '<div class="msg-sender">' + m.sender + '</div>' +
    '<div class="msg-bubble">' + m.text + '</div>' +
    '<div class="msg-time">' + m.time + '</div>';
  box.appendChild(div);
}

function postSysMsg(text) {
  db.ref('chat').push({ sender: '__system__', text: text, time: getTime() });
}

function sendMsg() {
  var inp = document.getElementById('chatInput');
  var txt = inp.value.trim();
  if (!txt) return;
  inp.value = '';
  db.ref('chat').push({ sender: userName, text: txt, time: getTime() });
}
</script>
</body>
</html>
