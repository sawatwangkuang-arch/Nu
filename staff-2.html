<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>พนักงาน - ฮิปเตอร์สเต็ก</title>
<script type="module">
  import { initializeApp } from "https://www.gstatic.com/firebasejs/12.15.0/firebase-app.js";
  import { getFirestore, doc, getDoc, updateDoc, arrayUnion, collection, getDocs, orderBy, query } from "https://www.gstatic.com/firebasejs/12.15.0/firebase-firestore.js";

  const firebaseConfig = {
    apiKey: "AIzaSyCSjCe_m6m3fl58wGVygsE8_bDOSk2WfD0",
    authDomain: "panu-648a8.firebaseapp.com",
    projectId: "panu-648a8",
    storageBucket: "panu-648a8.firebasestorage.app",
    messagingSenderId: "1042503149018",
    appId: "1:1042503149018:web:a05888018fd56da4fb0ce3"
  };

  const app = initializeApp(firebaseConfig);
  const db = getFirestore(app);
  window._db = db;
  window._fn = { doc, getDoc, updateDoc, arrayUnion, collection, getDocs, orderBy, query };
</script>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Sarabun:wght@300;400;600;700&display=swap');
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body { font-family: 'Sarabun', sans-serif; background: #f5f5f5; color: #333; min-height: 100vh; }
  .header { background: linear-gradient(135deg, #1a1210, #c0392b); color: white; padding: 16px; text-align: center; }
  .header h1 { font-size: 20px; }
  .header p { font-size: 12px; opacity: 0.8; margin-top: 4px; }
  .tabs { display: flex; background: white; border-bottom: 2px solid #eee; }
  .tab { flex: 1; padding: 12px; text-align: center; cursor: pointer; font-size: 14px; font-weight: 600; color: #999; border-bottom: 3px solid transparent; }
  .tab.active { color: #c0392b; border-bottom-color: #c0392b; }
  .content { padding: 16px; }
  .panel { display: none; }
  .panel.active { display: block; }
  .card { background: white; border-radius: 12px; padding: 20px; margin-bottom: 16px; box-shadow: 0 2px 8px rgba(0,0,0,0.08); }
  .card h3 { font-size: 16px; margin-bottom: 16px; color: #333; }
  input[type=text] { width: 100%; padding: 12px; border: 2px solid #eee; border-radius: 10px; font-size: 14px; font-family: 'Sarabun', sans-serif; margin-bottom: 12px; }
  input[type=text]:focus { outline: none; border-color: #c0392b; }
  .btn { width: 100%; padding: 14px; border: none; border-radius: 10px; font-size: 15px; font-weight: 700; cursor: pointer; font-family: 'Sarabun', sans-serif; }
  .btn-red { background: #c0392b; color: white; }
  .btn-green { background: #27ae60; color: white; }
  .btn-gray { background: #95a5a6; color: white; margin-top: 8px; }
  .result-card { background: #f8f9fa; border-radius: 10px; padding: 16px; margin-top: 16px; display: none; }
  .result-card.show { display: block; }
  .customer-avatar { width: 60px; height: 60px; border-radius: 50%; background: #ddd; margin: 0 auto 12px; display: flex; align-items: center; justify-content: center; font-size: 30px; overflow: hidden; }
  .customer-avatar img { width: 100%; height: 100%; object-fit: cover; }
  .customer-name { font-size: 18px; font-weight: 700; text-align: center; color: #333; }
  .stamps-display { display: flex; justify-content: center; gap: 8px; margin: 16px 0; }
  .s { width: 40px; height: 40px; border-radius: 50%; border: 2px solid #ddd; display: flex; align-items: center; justify-content: center; font-size: 18px; }
  .s.on { border-color: #e67e22; background: rgba(230,126,34,0.1); }
  .stamp-info { text-align: center; font-size: 14px; color: #666; margin-bottom: 16px; }
  .stamp-info strong { color: #c0392b; font-size: 18px; }
  .customer-row { display: flex; align-items: center; gap: 12px; padding: 12px; background: #f8f9fa; border-radius: 10px; margin-bottom: 8px; cursor: pointer; }
  .cust-avatar { width: 44px; height: 44px; border-radius: 50%; background: #ddd; display: flex; align-items: center; justify-content: center; font-size: 22px; overflow: hidden; flex-shrink: 0; }
  .cust-avatar img { width: 100%; height: 100%; object-fit: cover; }
  .cust-info { flex: 1; }
  .cust-name { font-size: 14px; font-weight: 700; }
  .cust-sub { font-size: 12px; color: #999; margin-top: 2px; }
  .cust-stamps { font-size: 20px; font-weight: 700; color: #c0392b; }
  .badge { padding: 3px 8px; border-radius: 10px; font-size: 11px; font-weight: 700; }
  .badge-full { background: rgba(39,174,96,0.15); color: #27ae60; }
  .toast { position: fixed; top: 20px; left: 50%; transform: translateX(-50%); padding: 12px 24px; border-radius: 10px; font-size: 14px; font-weight: 600; color: white; z-index: 9999; animation: fadeIn 0.3s; }
  .toast.success { background: #27ae60; }
  .toast.error { background: #c0392b; }
  @keyframes fadeIn { from { opacity: 0; transform: translateX(-50%) translateY(-10px); } to { opacity: 1; transform: translateX(-50%) translateY(0); } }
  .scan-area { border: 3px dashed #ddd; border-radius: 12px; padding: 30px; text-align: center; margin-bottom: 12px; }
  .scan-icon { font-size: 48px; margin-bottom: 8px; }
  .scan-hint { font-size: 13px; color: #999; }
  #video-preview { width: 100%; border-radius: 8px; display: none; }
  .loading { text-align: center; padding: 30px; color: #999; }
</style>
</head>
<body>

<div class="header">
  <h1>🥩 ระบบพนักงาน</h1>
  <p>ฮิปเตอร์สเต็ก ร้อยเอ็ด</p>
</div>

<div class="tabs">
  <div class="tab active" onclick="switchTab('scan')">📷 ให้แสตมป์</div>
  <div class="tab" onclick="switchTab('customers')">👥 ลูกค้าทั้งหมด</div>
</div>

<div class="content">
  <!-- SCAN TAB -->
  <div class="panel active" id="panel-scan">
    <div class="card">
      <h3>📷 สแกน QR หรือกรอก LINE ID</h3>
      <div class="scan-area" id="scan-area" onclick="startCamera()">
        <video id="video-preview" autoplay playsinline></video>
        <div id="scan-placeholder">
          <div class="scan-icon">📱</div>
          <div class="scan-hint">กดเพื่อเปิดกล้องสแกน QR</div>
        </div>
      </div>
      <p style="text-align:center;color:#999;font-size:13px;margin-bottom:12px">— หรือ —</p>
      <input type="text" id="uid-input" placeholder="กรอก LINE User ID ของลูกค้า">
      <button class="btn btn-red" onclick="searchCustomer()">🔍 ค้นหาลูกค้า</button>

      <div class="result-card" id="result-card">
        <div class="customer-avatar" id="cust-avatar-result">👤</div>
        <div class="customer-name" id="cust-name-result">-</div>
        <div class="stamps-display" id="stamps-display-result"></div>
        <div class="stamp-info">สะสมแล้ว <strong id="stamp-num-result">0</strong> / 5 ดวง</div>
        <button class="btn btn-green" onclick="addStamp()">🔥 ให้แสตมป์ +1</button>
        <button class="btn btn-gray" onclick="clearResult()">ยกเลิก</button>
      </div>
    </div>
  </div>

  <!-- CUSTOMERS TAB -->
  <div class="panel" id="panel-customers">
    <div class="card">
      <h3>👥 ลูกค้าทั้งหมด</h3>
      <div id="customers-list"><div class="loading">กำลังโหลด...</div></div>
    </div>
  </div>
</div>

<script>
  let currentCustomerId = null;
  let currentCustomerData = null;
  let cameraStream = null;

  function switchTab(tab) {
    document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
    document.querySelectorAll('.panel').forEach(p => p.classList.remove('active'));
    event.target.classList.add('active');
    document.getElementById('panel-' + tab).classList.add('active');
    if (tab === 'customers') loadCustomers();
  }

  function showToast(msg, type = 'success') {
    const t = document.createElement('div');
    t.className = 'toast ' + type;
    t.textContent = msg;
    document.body.appendChild(t);
    setTimeout(() => t.remove(), 3000);
  }

  function renderResultStamps(stamps) {
    const grid = document.getElementById('stamps-display-result');
    grid.innerHTML = '';
    for (let i = 0; i < 5; i++) {
      const s = document.createElement('div');
      s.className = 's' + (i < stamps ? ' on' : '');
      s.textContent = i < stamps ? '🔥' : '○';
      grid.appendChild(s);
    }
    document.getElementById('stamp-num-result').textContent = stamps;
  }

  async function searchCustomer(uid) {
    const inputUid = uid || document.getElementById('uid-input').value.trim();
    if (!inputUid) { showToast('กรุณากรอก LINE ID', 'error'); return; }
    try {
      const db = window._db;
      const { doc, getDoc } = window._fn;
      const ref = doc(db, 'customers', inputUid);
      const snap = await getDoc(ref);
      if (!snap.exists()) { showToast('ไม่พบลูกค้านี้ในระบบ', 'error'); return; }
      currentCustomerId = inputUid;
      currentCustomerData = snap.data();
      document.getElementById('cust-name-result').textContent = currentCustomerData.name || 'ไม่ระบุชื่อ';
      if (currentCustomerData.pictureUrl) {
        document.getElementById('cust-avatar-result').innerHTML = `<img src="${currentCustomerData.pictureUrl}">`;
      } else {
        document.getElementById('cust-avatar-result').textContent = '👤';
      }
      renderResultStamps(currentCustomerData.stamps || 0);
      document.getElementById('result-card').classList.add('show');
    } catch(e) {
      showToast('เกิดข้อผิดพลาด: ' + e.message, 'error');
    }
  }

  async function addStamp() {
    if (!currentCustomerId || !currentCustomerData) return;
    if (currentCustomerData.stamps >= 5) { showToast('ลูกค้าครบ 5 ดวงแล้ว ให้แลกก่อน', 'error'); return; }
    try {
      const db = window._db;
      const { doc, updateDoc, arrayUnion } = window._fn;
      const newStamps = (currentCustomerData.stamps || 0) + 1;
      const ref = doc(db, 'customers', currentCustomerId);
      await updateDoc(ref, {
        stamps: newStamps,
        history: arrayUnion({ type: 'stamp', date: new Date().toISOString() })
      });
      currentCustomerData.stamps = newStamps;
      renderResultStamps(newStamps);
      showToast('✅ ให้แสตมป์สำเร็จ! (' + newStamps + '/5)');
      if (newStamps >= 5) showToast('🎉 ลูกค้าครบ 5 ดวงแล้ว!', 'success');
    } catch(e) {
      showToast('เกิดข้อผิดพลาด', 'error');
    }
  }

  function clearResult() {
    currentCustomerId = null;
    currentCustomerData = null;
    document.getElementById('result-card').classList.remove('show');
    document.getElementById('uid-input').value = '';
  }

  async function loadCustomers() {
    try {
      const db = window._db;
      const { collection, getDocs } = window._fn;
      const snap = await getDocs(collection(db, 'customers'));
      const customers = [];
      snap.forEach(d => customers.push({ id: d.id, ...d.data() }));
      customers.sort((a, b) => (b.stamps || 0) - (a.stamps || 0));
      const list = document.getElementById('customers-list');
      if (customers.length === 0) {
        list.innerHTML = '<p style="text-align:center;color:#999;padding:20px">ยังไม่มีลูกค้า</p>';
        return;
      }
      list.innerHTML = customers.map(c => `
        <div class="customer-row" onclick="selectCustomer('${c.id}')">
          <div class="cust-avatar">${c.pictureUrl ? `<img src="${c.pictureUrl}">` : '👤'}</div>
          <div class="cust-info">
            <div class="cust-name">${c.name || 'ไม่ระบุชื่อ'}</div>
            <div class="cust-sub">แลกแล้ว ${c.redeemCount || 0} ครั้ง</div>
          </div>
          <div>
            <div class="cust-stamps">${c.stamps || 0}/5</div>
            ${(c.stamps || 0) >= 5 ? '<div class="badge badge-full">ครบแล้ว!</div>' : ''}
          </div>
        </div>
      `).join('');
    } catch(e) {
      document.getElementById('customers-list').innerHTML = '<p style="color:red;text-align:center">โหลดไม่ได้: ' + e.message + '</p>';
    }
  }

  function selectCustomer(uid) {
    switchTab('scan');
    document.querySelector('.tab').classList.add('active');
    document.getElementById('uid-input').value = uid;
    searchCustomer(uid);
  }

  async function startCamera() {
    try {
      const stream = await navigator.mediaDevices.getUserMedia({ video: { facingMode: 'environment' } });
      const video = document.getElementById('video-preview');
      video.srcObject = stream;
      video.style.display = 'block';
      document.getElementById('scan-placeholder').style.display = 'none';
      cameraStream = stream;
      showToast('เปิดกล้องแล้ว กรุณาใช้ QR Scanner app สแกน แล้วกรอก ID', 'success');
    } catch(e) {
      showToast('ไม่สามารถเปิดกล้องได้ กรุณากรอก ID แทน', 'error');
    }
  }
</script>
</body>
</html>
