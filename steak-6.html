<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ฮิปเตอร์สเต็ก ร้อยเอ็ด</title>
<!-- LINE SDK -->
<script src="https://static.line-scdn.net/liff/edge/versions/2.22.3/sdk.js"></script>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Sarabun:wght@300;400;600;700&display=swap');

  :root {
    --coal: #1a1210;
    --ember: #c0392b;
    --amber: #e67e22;
    --cream: #fdf6ee;
    --bone: #f0e6d3;
    --smoke: #7f6a5c;
    --gold: #d4a84b;
    --success: #27ae60;
    --warning: #f39c12;
  }

  * { margin: 0; padding: 0; box-sizing: border-box; }

  body {
    font-family: 'Sarabun', sans-serif;
    background: linear-gradient(135deg, #0f0a08 0%, #1a1210 100%);
    color: var(--cream);
    min-height: 100vh;
    max-width: 430px;
    margin: 0 auto;
    position: relative;
  }

  /* Loading State */
  .loading-screen {
    position: fixed;
    inset: 0;
    background: linear-gradient(135deg, #0f0a08 0%, #1a1210 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 20px;
    z-index: 2000;
  }
  .loading-screen.hidden {
    display: none;
  }
  .spinner {
    width: 40px;
    height: 40px;
    border: 4px solid rgba(212,168,75,0.2);
    border-top-color: var(--gold);
    border-radius: 50%;
    animation: spin 1s linear infinite;
  }
  @keyframes spin {
    to { transform: rotate(360deg); }
  }
  .loading-text {
    color: var(--gold);
    font-size: 14px;
  }

  /* Header */
  .header {
    background: linear-gradient(160deg, rgba(45,26,20,0.95) 0%, rgba(26,18,16,0.95) 100%);
    backdrop-filter: blur(10px);
    padding: 24px 20px 16px;
    border-bottom: 2px solid var(--ember);
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 8px 32px rgba(0,0,0,0.3);
  }
  .header-top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 12px;
  }
  .logo {
    font-family: 'Playfair Display', serif;
    font-size: 20px;
    font-weight: 900;
    color: var(--gold);
    letter-spacing: 1px;
    line-height: 1.1;
  }
  .logo span { 
    display: block; 
    font-size: 11px; 
    color: var(--smoke); 
    font-family: 'Sarabun', sans-serif; 
    font-weight: 300; 
    letter-spacing: 3px; 
    text-transform: uppercase; 
  }
  .header-right {
    display: flex;
    gap: 12px;
    align-items: center;
  }
  .badge-stamps {
    background: linear-gradient(135deg, var(--ember), #a02820);
    color: white;
    font-size: 12px;
    font-weight: 700;
    padding: 6px 12px;
    border-radius: 20px;
    box-shadow: 0 4px 15px rgba(192,57,43,0.3);
    transition: all 0.3s ease;
  }
  .badge-stamps:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(192,57,43,0.4);
  }
  .profile-btn {
    background: rgba(212,168,75,0.15);
    border: 1px solid var(--gold);
    color: var(--gold);
    width: 36px;
    height: 36px;
    border-radius: 50%;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 18px;
    transition: all 0.3s ease;
  }
  .profile-btn:hover {
    background: rgba(212,168,75,0.25);
    transform: scale(1.05);
  }
  .close-btn {
    background: rgba(192,57,43,0.2);
    border: 1px solid var(--ember);
    color: var(--ember);
    width: 32px;
    height: 32px;
    border-radius: 50%;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 16px;
    transition: all 0.3s ease;
  }
  .close-btn:hover {
    background: rgba(192,57,43,0.3);
  }

  /* Nav tabs */
  .nav {
    display: flex;
    background: rgba(15,10,8,0.8);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(45,26,20,0.5);
  }
  .nav-btn {
    flex: 1;
    background: none;
    border: none;
    color: var(--smoke);
    padding: 12px 4px;
    font-family: 'Sarabun', sans-serif;
    font-size: 12px;
    font-weight: 600;
    cursor: pointer;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 3px;
    transition: all 0.3s ease;
    border-bottom: 3px solid transparent;
    position: relative;
  }
  .nav-btn.active { 
    color: var(--gold); 
    border-bottom-color: var(--gold);
  }
  .nav-btn:hover:not(.active) {
    color: var(--amber);
  }
  .nav-btn .icon { font-size: 18px; }

  /* Page sections */
  .page { 
    display: none; 
    padding: 20px; 
    animation: fadeIn 0.3s ease;
  }
  .page.active { display: block; }
  
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(10px); }
    to { opacity: 1; transform: translateY(0); }
  }

  /* Stamp card */
  .stamp-card {
    background: linear-gradient(135deg, rgba(45,26,20,0.6), rgba(26,18,16,0.6));
    backdrop-filter: blur(10px);
    border: 1px solid rgba(212,168,75,0.2);
    border-radius: 20px;
    padding: 24px;
    margin-bottom: 20px;
    position: relative;
    overflow: hidden;
    box-shadow: 0 8px 32px rgba(0,0,0,0.2);
  }
  .stamp-card::before {
    content: '🥩';
    position: absolute;
    right: -10px;
    top: -10px;
    font-size: 80px;
    opacity: 0.06;
  }
  .stamp-card h3 { 
    font-size: 13px; 
    color: var(--smoke); 
    margin-bottom: 14px; 
    letter-spacing: 2px; 
    text-transform: uppercase; 
  }
  .stamps-grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 10px;
    margin-bottom: 16px;
  }
  .stamp {
    aspect-ratio: 1;
    border-radius: 50%;
    border: 2px solid rgba(61,34,24,0.8);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 18px;
    background: rgba(15,10,8,0.6);
    transition: all 0.3s ease;
    cursor: pointer;
  }
  .stamp:hover {
    transform: scale(1.1);
  }
  .stamp.filled {
    border-color: var(--amber);
    background: radial-gradient(circle, rgba(230,126,34,0.4), rgba(45,21,8,0.6));
    box-shadow: 0 0 15px rgba(230,126,34,0.4);
  }
  .stamp.filled::after { content: '🔥'; font-size: 18px; }
  .stamp:not(.filled)::after { content: '○'; color: rgba(61,34,24,0.8); font-size: 22px; }

  .progress-bar {
    height: 6px;
    background: rgba(45,26,20,0.8);
    border-radius: 6px;
    overflow: hidden;
    margin-bottom: 12px;
  }
  .progress-fill {
    height: 100%;
    background: linear-gradient(90deg, var(--ember), var(--amber));
    border-radius: 6px;
    transition: width 0.5s ease;
    box-shadow: 0 0 10px rgba(230,126,34,0.3);
  }
  .progress-label {
    display: flex;
    justify-content: space-between;
    font-size: 12px;
    color: var(--smoke);
  }
  .progress-label strong { color: var(--amber); }

  /* QR Section */
  .qr-section {
    background: linear-gradient(135deg, rgba(253,246,238,0.95), rgba(240,230,211,0.95));
    backdrop-filter: blur(10px);
    border-radius: 20px;
    padding: 24px;
    text-align: center;
    margin-bottom: 20px;
    color: var(--coal);
    box-shadow: 0 8px 32px rgba(0,0,0,0.2);
  }
  .qr-section h3 { 
    font-family: 'Playfair Display', serif; 
    font-size: 16px; 
    color: var(--coal); 
    margin-bottom: 6px; 
  }
  .qr-section p { 
    font-size: 12px; 
    color: var(--smoke); 
    margin-bottom: 16px; 
  }
  .qr-box {
    width: 160px;
    height: 160px;
    margin: 0 auto 16px;
    background: white;
    border-radius: 16px;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 8px 32px rgba(0,0,0,0.15);
    position: relative;
    overflow: hidden;
  }
  .qr-inner {
    display: grid;
    grid-template-columns: repeat(7, 1fr);
    gap: 2px;
    padding: 12px;
    width: 100%;
    height: 100%;
  }
  .qr-pixel {
    border-radius: 1px;
    background: var(--coal);
  }
  .qr-logo {
    position: absolute;
    width: 36px;
    height: 36px;
    background: linear-gradient(135deg, var(--ember), #a02820);
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 18px;
    border: 2px solid white;
    box-shadow: 0 4px 12px rgba(0,0,0,0.2);
  }
  .scan-btn {
    background: linear-gradient(135deg, var(--ember), #a02820);
    color: white;
    border: none;
    padding: 12px 28px;
    border-radius: 30px;
    font-family: 'Sarabun', sans-serif;
    font-size: 14px;
    font-weight: 700;
    cursor: pointer;
    display: inline-flex;
    align-items: center;
    gap: 8px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(192,57,43,0.3);
  }
  .scan-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(192,57,43,0.4);
  }
  .scan-btn:active { transform: scale(0.96); }

  /* Discount badge */
  .discount-ready {
    background: linear-gradient(135deg, var(--gold), var(--amber));
    border-radius: 16px;
    padding: 20px;
    text-align: center;
    margin-bottom: 20px;
    animation: pulse 2s infinite;
    box-shadow: 0 8px 32px rgba(212,168,75,0.3);
  }
  @keyframes pulse { 
    0%,100% { box-shadow: 0 8px 32px rgba(212,168,75,0.3); } 
    50% { box-shadow: 0 8px 32px rgba(212,168,75,0.5); } 
  }
  .discount-ready h3 { color: var(--coal); font-size: 18px; font-weight: 700; }
  .discount-ready p { color: #5d3a00; font-size: 13px; margin-top: 4px; }

  /* Menu Filter */
  .menu-filter {
    display: flex;
    gap: 8px;
    margin-bottom: 20px;
    overflow-x: auto;
    padding-bottom: 8px;
  }
  .filter-btn {
    background: rgba(45,26,20,0.6);
    border: 1px solid rgba(212,168,75,0.2);
    color: var(--smoke);
    padding: 8px 16px;
    border-radius: 20px;
    font-size: 12px;
    font-weight: 600;
    cursor: pointer;
    white-space: nowrap;
    transition: all 0.3s ease;
  }
  .filter-btn:hover,
  .filter-btn.active {
    background: linear-gradient(135deg, var(--amber), #d68910);
    color: white;
    border-color: var(--amber);
  }

  /* Menu */
  .menu-category {
    margin-bottom: 24px;
  }
  .cat-title {
    font-family: 'Playfair Display', serif;
    font-size: 18px;
    color: var(--gold);
    margin-bottom: 12px;
    padding-bottom: 8px;
    border-bottom: 1px solid rgba(45,26,20,0.5);
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .menu-item {
    display: flex;
    align-items: center;
    gap: 14px;
    padding: 14px 0;
    border-bottom: 1px solid rgba(31,19,16,0.5);
    transition: all 0.3s ease;
    cursor: pointer;
  }
  .menu-item:hover {
    transform: translateX(4px);
  }
  .menu-emoji {
    font-size: 36px;
    width: 52px;
    height: 52px;
    background: rgba(45,26,20,0.6);
    border-radius: 12px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    transition: all 0.3s ease;
  }
  .menu-item:hover .menu-emoji {
    background: rgba(212,168,75,0.2);
    transform: scale(1.1);
  }
  .menu-info { flex: 1; }
  .menu-name { font-size: 15px; font-weight: 600; color: var(--cream); }
  .menu-desc { font-size: 11px; color: var(--smoke); margin-top: 2px; line-height: 1.4; }
  .menu-price {
    font-family: 'Playfair Display', serif;
    font-size: 16px;
    font-weight: 700;
    color: var(--amber);
    white-space: nowrap;
  }
  .menu-price span { 
    display: block; 
    font-size: 10px; 
    color: var(--smoke); 
    font-family: 'Sarabun', sans-serif; 
    text-align: right; 
  }

  /* History */
  .history-item {
    background: rgba(31,19,16,0.6);
    backdrop-filter: blur(10px);
    border-radius: 12px;
    padding: 14px;
    margin-bottom: 10px;
    display: flex;
    align-items: center;
    gap: 12px;
    transition: all 0.3s ease;
  }
  .history-item:hover {
    background: rgba(45,26,20,0.8);
    transform: translateX(4px);
  }
  .hist-icon {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: rgba(45,26,20,0.8);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 18px;
    flex-shrink: 0;
  }
  .hist-info { flex: 1; }
  .hist-title { font-size: 14px; font-weight: 600; }
  .hist-date { font-size: 11px; color: var(--smoke); margin-top: 2px; }
  .hist-badge {
    font-size: 12px;
    font-weight: 700;
    padding: 4px 10px;
    border-radius: 20px;
    background: rgba(45,26,20,0.8);
    color: var(--amber);
  }
  .hist-badge.discount { 
    background: rgba(192,57,43,0.2); 
    color: var(--ember); 
  }

  /* Promotions */
  .promo-card {
    background: linear-gradient(135deg, rgba(45,26,20,0.6), rgba(26,18,16,0.6));
    backdrop-filter: blur(10px);
    border: 1px solid rgba(212,168,75,0.2);
    border-radius: 16px;
    padding: 20px;
    margin-bottom: 14px;
    display: flex;
    gap: 14px;
    align-items: flex-start;
    transition: all 0.3s ease;
  }
  .promo-card:hover {
    border-color: rgba(212,168,75,0.4);
    transform: translateY(-4px);
    box-shadow: 0 8px 32px rgba(0,0,0,0.2);
  }
  .promo-icon { font-size: 36px; flex-shrink: 0; }
  .promo-title { font-weight: 700; font-size: 15px; color: var(--gold); margin-bottom: 4px; }
  .promo-desc { font-size: 12px; color: var(--smoke); line-height: 1.5; }
  .promo-tag {
    display: inline-block;
    margin-top: 8px;
    background: rgba(192,57,43,0.2);
    color: var(--ember);
    font-size: 11px;
    font-weight: 700;
    padding: 3px 10px;
    border-radius: 20px;
  }

  /* Profile Page */
  .profile-card {
    background: linear-gradient(135deg, rgba(45,26,20,0.6), rgba(26,18,16,0.6));
    backdrop-filter: blur(10px);
    border: 1px solid rgba(212,168,75,0.2);
    border-radius: 20px;
    padding: 24px;
    margin-bottom: 20px;
    text-align: center;
    box-shadow: 0 8px 32px rgba(0,0,0,0.2);
  }
  .profile-avatar {
    width: 80px;
    height: 80px;
    border-radius: 50%;
    background: linear-gradient(135deg, var(--amber), var(--gold));
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 40px;
    margin: 0 auto 16px;
    box-shadow: 0 4px 15px rgba(212,168,75,0.3);
    overflow: hidden;
  }
  .profile-avatar img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .profile-name {
    font-family: 'Playfair Display', serif;
    font-size: 18px;
    color: var(--gold);
    margin-bottom: 4px;
  }
  .profile-email {
    font-size: 12px;
    color: var(--smoke);
    margin-bottom: 16px;
  }
  .profile-form {
    display: flex;
    flex-direction: column;
    gap: 12px;
  }
  .form-group {
    display: flex;
    flex-direction: column;
    gap: 6px;
  }
  .form-group label {
    font-size: 12px;
    color: var(--smoke);
    font-weight: 600;
    text-align: left;
  }
  .form-group input {
    background: rgba(15,10,8,0.6);
    border: 1px solid rgba(212,168,75,0.2);
    color: var(--cream);
    padding: 10px 12px;
    border-radius: 8px;
    font-family: 'Sarabun', sans-serif;
    font-size: 14px;
    transition: all 0.3s ease;
  }
  .form-group input:focus {
    outline: none;
    border-color: var(--gold);
    background: rgba(15,10,8,0.8);
    box-shadow: 0 0 10px rgba(212,168,75,0.2);
  }
  .save-btn {
    background: linear-gradient(135deg, var(--success), #1e8449);
    color: white;
    border: none;
    padding: 12px;
    border-radius: 8px;
    font-family: 'Sarabun', sans-serif;
    font-size: 14px;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.3s ease;
    margin-top: 8px;
  }
  .save-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 15px rgba(39,174,96,0.3);
  }

  /* Modal for scan */
  .modal-overlay {
    display: none;
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.85);
    backdrop-filter: blur(5px);
    z-index: 999;
    align-items: center;
    justify-content: center;
    animation: fadeIn 0.3s ease;
  }
  .modal-overlay.show { display: flex; }
  .modal {
    background: linear-gradient(135deg, rgba(31,19,16,0.95), rgba(26,18,16,0.95));
    backdrop-filter: blur(10px);
    border: 1px solid rgba(212,168,75,0.3);
    border-radius: 24px;
    padding: 28px 24px;
    width: 320px;
    text-align: center;
    box-shadow: 0 20px 60px rgba(0,0,0,0.4);
  }
  .modal h3 { 
    font-family: 'Playfair Display', serif; 
    font-size: 22px; 
    color: var(--gold); 
    margin-bottom: 8px; 
  }
  .modal p { 
    color: var(--smoke); 
    font-size: 13px; 
    margin-bottom: 20px; 
    line-height: 1.6; 
  }
  .modal-btns { 
    display: flex; 
    gap: 10px; 
  }
  .modal-btn {
    flex: 1;
    padding: 12px;
    border-radius: 30px;
    border: none;
    font-family: 'Sarabun', sans-serif;
    font-size: 14px;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.3s ease;
  }
  .modal-btn.primary { 
    background: linear-gradient(135deg, var(--ember), #a02820);
    color: white;
  }
  .modal-btn.primary:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 15px rgba(192,57,43,0.3);
  }
  .modal-btn.secondary { 
    background: rgba(45,26,20,0.8); 
    color: var(--smoke);
  }
  .modal-btn.secondary:hover {
    background: rgba(45,26,20,1);
  }
  .stamp-anim { 
    font-size: 48px; 
    margin: 16px 0; 
    animation: bounce 0.5s ease; 
  }
  @keyframes bounce { 
    0%,100% { transform: scale(1); } 
    50% { transform: scale(1.3); } 
  }

  /* Toast Notification */
  .toast-container {
    position: fixed;
    bottom: 20px;
    right: 20px;
    z-index: 1000;
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .toast {
    background: linear-gradient(135deg, rgba(39,174,96,0.9), rgba(30,132,73,0.9));
    backdrop-filter: blur(10px);
    color: white;
    padding: 14px 16px;
    border-radius: 12px;
    box-shadow: 0 8px 32px rgba(0,0,0,0.3);
    display: flex;
    align-items: center;
    gap: 10px;
    animation: slideIn 0.3s ease;
    min-width: 280px;
  }
  .toast.error {
    background: linear-gradient(135deg, rgba(192,57,43,0.9), rgba(160,40,32,0.9));
  }
  .toast.warning {
    background: linear-gradient(135deg, rgba(243,156,18,0.9), rgba(230,126,34,0.9));
  }
  @keyframes slideIn {
    from { 
      transform: translateX(400px);
      opacity: 0;
    }
    to { 
      transform: translateX(0);
      opacity: 1;
    }
  }
  @keyframes slideOut {
    from { 
      transform: translateX(0);
      opacity: 1;
    }
    to { 
      transform: translateX(400px);
      opacity: 0;
    }
  }
  .toast.hide {
    animation: slideOut 0.3s ease forwards;
  }

  /* Responsive */
  @media (max-width: 480px) {
    body { max-width: 100%; }
    .header { padding: 16px 16px 12px; }
    .logo { font-size: 18px; }
    .badge-stamps { font-size: 11px; padding: 5px 10px; }
    .modal { width: 90%; }
  }
</style>
</head>
<body>

<!-- Loading Screen -->
<div class="loading-screen" id="loading-screen">
  <div class="spinner"></div>
  <div class="loading-text">กำลังเชื่อมต่อ...</div>
</div>

<!-- Header -->
<div class="header">
  <div class="header-top">
    <div class="logo">
      ฮิปเตอร์สเต็ก
      <span>Hipster Steak · Roi Et</span>
    </div>
    <div class="header-right">
      <div class="badge-stamps" id="header-stamps">🔥 3/5 ดวง</div>
      <button class="profile-btn" onclick="showPage('profile')" title="โปรไฟล์">👤</button>
      <button class="close-btn" onclick="closeLIFF()" title="ปิด">✕</button>
    </div>
  </div>
</div>

<!-- Nav -->
<div class="nav">
  <button class="nav-btn active" onclick="showPage('home')" id="nav-home">
    <span class="icon">🏠</span>สะสมแสตมป์
  </button>
  <button class="nav-btn" onclick="showPage('menu')" id="nav-menu">
    <span class="icon">🥩</span>เมนู
  </button>
  <button class="nav-btn" onclick="showPage('history')" id="nav-history">
    <span class="icon">📋</span>ประวัติ
  </button>
  <button class="nav-btn" onclick="showPage('promo')" id="nav-promo">
    <span class="icon">🎉</span>โปรโมชั่น
  </button>
</div>

<!-- HOME PAGE -->
<div class="page active" id="page-home">

  <div id="discount-banner" style="display:none" class="discount-ready">
    <h3>🎉 ครบ 5 ดวงแล้ว!</h3>
    <p>คุณได้รับสิทธิ์ลด 10% สำหรับมื้อถัดไป</p>
  </div>

  <div class="stamp-card">
    <h3>บัตรสะสมแสตมป์</h3>
    <div class="stamps-grid" id="stamps-grid">
    </div>
    <div class="progress-bar">
      <div class="progress-fill" id="progress-fill" style="width:60%"></div>
    </div>
    <div class="progress-label">
      <span>สะสมแล้ว <strong id="stamp-count">3</strong> ดวง</span>
      <span>เป้าหมาย <strong>5 ดวง</strong></span>
    </div>
  </div>

  <div class="qr-section">
    <h3>สแกน QR Code เพื่อรับแสตมป์</h3>
    <p>แสดงหน้านี้ให้พนักงานสแกน ทุกการสั่งอาหาร 1 ครั้ง = 1 ดวง</p>
    <div class="qr-box">
      <canvas id="qr-canvas" width="160" height="160"></canvas>
      <div class="qr-logo">🥩</div>
    </div>
    <button class="scan-btn" onclick="simulateScan()">
      📷 รับแสตมป์ (จำลองการสแกน)
    </button>
  </div>
</div>

<!-- MENU PAGE -->
<div class="page" id="page-menu">
  <div class="menu-filter">
    <button class="filter-btn active" onclick="filterMenu('all')">ทั้งหมด</button>
    <button class="filter-btn" onclick="filterMenu('steak')">🥩 สเต็ก</button>
    <button class="filter-btn" onclick="filterMenu('chicken')">🍗 ไก่และหมู</button>
    <button class="filter-btn" onclick="filterMenu('side')">🥗 เครื่องเคียง</button>
  </div>

  <div class="menu-category" data-category="steak">
    <div class="cat-title">🥩 สเต็ก</div>
    <div class="menu-item">
      <div class="menu-emoji">🥩</div>
      <div class="menu-info">
        <div class="menu-name">ริบอาย สเต็ก</div>
        <div class="menu-desc">เนื้อออสเตรเลีย เกรด A ย่างถ่านหอมกลิ่นไม้</div>
      </div>
      <div class="menu-price">299฿<span>250g</span></div>
    </div>
    <div class="menu-item">
      <div class="menu-emoji">🥩</div>
      <div class="menu-info">
        <div class="menu-name">ซีร่อยน์ สเต็ก</div>
        <div class="menu-desc">เนื้อนุ่ม ไขมันน้อย เหมาะสำหรับคนรักสุขภาพ</div>
      </div>
      <div class="menu-price">249฿<span>200g</span></div>
    </div>
    <div class="menu-item">
      <div class="menu-emoji">🥩</div>
      <div class="menu-info">
        <div class="menu-name">เทนเดอร์ล่อยน์ สเต็ก</div>
        <div class="menu-desc">เนื้อสันในนุ่มเนียน สมบูรณ์แบบทุกคำ</div>
      </div>
      <div class="menu-price">349฿<span>200g</span></div>
    </div>
    <div class="menu-item">
      <div class="menu-emoji">🍖</div>
      <div class="menu-info">
        <div class="menu-name">ทีโบน สเต็ก</div>
        <div class="menu-desc">สองเนื้อในชิ้นเดียว ซีร่อยน์ + เทนเดอร์ล่อยน์</div>
      </div>
      <div class="menu-price">399฿<span>350g</span></div>
    </div>
  </div>

  <div class="menu-category" data-category="chicken">
    <div class="cat-title">🍗 ไก่และหมู</div>
    <div class="menu-item">
      <div class="menu-emoji">🍗</div>
      <div class="menu-info">
        <div class="menu-name">ไก่ย่างสมุนไพร</div>
        <div class="menu-desc">ไก่หมักสมุนไพรไทย อบถ่านกรอบนอก นุ่มในสุด</div>
      </div>
      <div class="menu-price">189฿<span>350g</span></div>
    </div>
    <div class="menu-item">
      <div class="menu-emoji">🍖</div>
      <div class="menu-info">
        <div class="menu-name">หมูย่างเกาหลี</div>
        <div class="menu-desc">หมูสามชั้นหมักซอสเกาหลี ย่างสดใหม่ต่อหน้า</div>
      </div>
      <div class="menu-price">229฿<span>300g</span></div>
    </div>
    <div class="menu-item">
      <div class="menu-emoji">🍗</div>
      <div class="menu-info">
        <div class="menu-name">ไก่ครึ่งตัว</div>
        <div class="menu-desc">ไก่ย่างสดใหม่ เสิร์ฟพร้อมซอสพิเศษ</div>
      </div>
      <div class="menu-price">299฿<span>600g</span></div>
    </div>
  </div>

  <div class="menu-category" data-category="side">
    <div class="cat-title">🥗 เครื่องเคียง & เครื่องดื่ม</div>
    <div class="menu-item">
      <div class="menu-emoji">🍟</div>
      <div class="menu-info">
        <div class="menu-name">เฟรนช์ฟรายส์ทรัฟเฟิล</div>
        <div class="menu-desc">มันฝรั่งกรอบราดน้ำมันทรัฟเฟิล โรยพาร์เมซาน</div>
      </div>
      <div class="menu-price">79฿</div>
    </div>
    <div class="menu-item">
      <div class="menu-emoji">🥗</div>
      <div class="menu-info">
        <div class="menu-name">สลัดผักรวม</div>
        <div class="menu-desc">ผักสดน้ำสลัดซีซาร์โฮมเมด</div>
      </div>
      <div class="menu-price">59฿</div>
    </div>
    <div class="menu-item">
      <div class="menu-emoji">🧃</div>
      <div class="menu-info">
        <div class="menu-name">น้ำผลไม้สด</div>
        <div class="menu-desc">ส้ม / มะม่วง / สับปะรด / มะพร้าว</div>
      </div>
      <div class="menu-price">59฿</div>
    </div>
    <div class="menu-item">
      <div class="menu-emoji">☕</div>
      <div class="menu-info">
        <div class="menu-name">กาแฟฮิปเตอร์</div>
        <div class="menu-desc">เมล็ดคั่วพิเศษจากดอยช้าง เสิร์ฟร้อน/เย็น</div>
      </div>
      <div class="menu-price">69฿</div>
    </div>
  </div>
</div>

<!-- HISTORY PAGE -->
<div class="page" id="page-history">
  <div id="history-list">
    <div class="history-item">
      <div class="hist-icon">🔥</div>
      <div class="hist-info">
        <div class="hist-title">รับแสตมป์</div>
        <div class="hist-date">19 มิ.ย. 2569 · 19:32</div>
      </div>
      <div class="hist-badge">+1 ดวง</div>
    </div>
    <div class="history-item">
      <div class="hist-icon">🔥</div>
      <div class="hist-info">
        <div class="hist-title">รับแสตมป์</div>
        <div class="hist-date">15 มิ.ย. 2569 · 12:14</div>
      </div>
      <div class="hist-badge">+1 ดวง</div>
    </div>
    <div class="history-item">
      <div class="hist-icon">🎉</div>
      <div class="hist-info">
        <div class="hist-title">ใช้ส่วนลด 10%</div>
        <div class="hist-date">10 มิ.ย. 2569 · 18:55</div>
      </div>
      <div class="hist-badge discount">ใช้แล้ว</div>
    </div>
    <div class="history-item">
      <div class="hist-icon">🔥</div>
      <div class="hist-info">
        <div class="hist-title">รับแสตมป์</div>
        <div class="hist-date">5 มิ.ย. 2569 · 20:10</div>
      </div>
      <div class="hist-badge">+1 ดวง</div>
    </div>
  </div>
</div>

<!-- PROMO PAGE -->
<div class="page" id="page-promo">
  <div class="promo-card">
    <div class="promo-icon">🔥</div>
    <div>
      <div class="promo-title">สะสม 5 ดวง รับลด 10%</div>
      <div class="promo-desc">สั่งอาหารทุก 1 ครั้ง รับ 1 แสตมป์ เมื่อครบ 5 ดวง รับส่วนลดทันที 10% จากยอดบิลทั้งหมด</div>
      <span class="promo-tag">ตลอดทั้งปี</span>
    </div>
  </div>
  <div class="promo-card">
    <div class="promo-icon">🎂</div>
    <div>
      <div class="promo-title">วันเกิดพิเศษ</div>
      <div class="promo-desc">รับส่วนลด 20% และของหวานฟรี 1 จาน ในเดือนวันเกิดของคุณ แจ้งพนักงานพร้อมบัตรประชาชน</div>
      <span class="promo-tag">เดือนเกิดเท่านั้น</span>
    </div>
  </div>
  <div class="promo-card">
    <div class="promo-icon">👫</div>
    <div>
      <div class="promo-title">มื้อค่ำสำหรับคู่รัก</div>
      <div class="promo-desc">สั่งสเต็ก 2 จาน แถมเครื่องดื่มฟรี 2 แก้ว ทุกวันศุกร์-เสาร์ เวลา 17:00–21:00</div>
      <span class="promo-tag">ศุกร์–เสาร์</span>
    </div>
  </div>
  <div class="promo-card">
    <div class="promo-icon">📣</div>
    <div>
      <div class="promo-title">ชวนเพื่อนมาทาน</div>
      <div class="promo-desc">พาเพื่อนใหม่มาทานครั้งแรก รับแสตมป์โบนัส 1 ดวงทันที ไม่จำกัดจำนวนครั้ง</div>
      <span class="promo-tag">ตลอดทั้งปี</span>
    </div>
  </div>
  <div style="text-align:center; margin-top: 20px;">
    <p style="color: var(--smoke); font-size: 12px;">📍 ฮิปเตอร์สเต็ก ร้อยเอ็ด<br>เปิดทุกวัน 11:00–22:00 น.<br>☎️ 043-XXX-XXXX</p>
  </div>
</div>

<!-- PROFILE PAGE -->
<div class="page" id="page-profile">
  <div class="profile-card">
    <div class="profile-avatar" id="profile-avatar">👤</div>
    <div class="profile-name" id="profile-name-display">สมาชิกฮิปเตอร์</div>
    <div class="profile-email" id="profile-email-display">member@hipstersteak.com</div>
  </div>

  <div class="stamp-card">
    <h3>สถิติการสะสมแสตมป์</h3>
    <div style="text-align: center; margin: 16px 0;">
      <div style="font-size: 32px; color: var(--gold); font-weight: 700; margin-bottom: 8px;" id="total-stamps">3</div>
      <div style="font-size: 12px; color: var(--smoke);">ดวงแสตมป์ทั้งหมด</div>
    </div>
    <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-top: 16px;">
      <div style="background: rgba(15,10,8,0.6); padding: 12px; border-radius: 8px; text-align: center;">
        <div style="font-size: 18px; color: var(--amber); font-weight: 700;" id="lifetime-stamps">3</div>
        <div style="font-size: 11px; color: var(--smoke); margin-top: 4px;">ตลอดอายุ</div>
      </div>
      <div style="background: rgba(15,10,8,0.6); padding: 12px; border-radius: 8px; text-align: center;">
        <div style="font-size: 18px; color: var(--amber); font-weight: 700;" id="used-stamps">1</div>
        <div style="font-size: 11px; color: var(--smoke); margin-top: 4px;">ใช้แล้ว</div>
      </div>
    </div>
  </div>

  <div class="profile-card">
    <h3 style="text-align: left; margin-bottom: 16px;">ข้อมูลส่วนตัว</h3>
    <div class="profile-form">
      <div class="form-group">
        <label>ชื่อ-นามสกุล</label>
        <input type="text" id="input-name" placeholder="กรุณากรอกชื่อ-นามสกุล">
      </div>
      <div class="form-group">
        <label>อีเมล</label>
        <input type="email" id="input-email" placeholder="กรุณากรอกอีเมล">
      </div>
      <div class="form-group">
        <label>เบอร์โทรศัพท์</label>
        <input type="tel" id="input-phone" placeholder="กรุณากรอกเบอร์โทรศัพท์">
      </div>
      <button class="save-btn" onclick="saveProfile()">💾 บันทึกข้อมูล</button>
    </div>
  </div>
</div>

<!-- Modal -->
<div class="modal-overlay" id="scan-modal">
  <div class="modal">
    <div class="stamp-anim" id="modal-icon">🔥</div>
    <h3 id="modal-title">รับแสตมป์สำเร็จ!</h3>
    <p id="modal-msg">คุณได้รับ 1 ดวง ขอบคุณที่มาอุดหนุนนะคะ 🙏</p>
    <div class="modal-btns">
      <button class="modal-btn secondary" onclick="closeModal()">ปิด</button>
      <button class="modal-btn primary" onclick="closeModal()">ยอดเยี่ยม!</button>
    </div>
  </div>
</div>

<!-- Toast Container -->
<div class="toast-container" id="toast-container"></div>

<script>
  // ==================== LINE LIFF CONFIGURATION ====================
  // ⚠️ สำคัญ: ให้ใส่ LIFF ID ของคุณตรงนี้ (ได้จากการสมัคร LINE Developers)
  const LIFF_ID = '2010457043-0yiKBN1p'; // เช่น: '1234567890-abcdefgh'

  // ==================== DATA MANAGEMENT ====================
  const STORAGE_KEY = 'hipster_steak_data';
  const MAX_STAMPS = 5;

  let appData = {
    stamps: 3,
    usedStamps: 1,
    profile: {
      name: 'สมาชิกฮิปเตอร์',
      email: 'member@hipstersteak.com',
      phone: '',
      pictureUrl: null
    },
    history: [
      { title: 'รับแสตมป์', icon: '🔥', badge: '+1 ดวง', badgeClass: '', date: new Date(Date.now() - 5*24*60*60*1000) },
      { title: 'รับแสตมป์', icon: '🔥', badge: '+1 ดวง', badgeClass: '', date: new Date(Date.now() - 9*24*60*60*1000) },
      { title: 'ใช้ส่วนลด 10%', icon: '🎉', badge: 'ใช้แล้ว', badgeClass: 'discount', date: new Date(Date.now() - 14*24*60*60*1000) },
      { title: 'รับแสตมป์', icon: '🔥', badge: '+1 ดวง', badgeClass: '', date: new Date(Date.now() - 19*24*60*60*1000) }
    ]
  };

  // Load data from localStorage
  function loadData() {
    const saved = localStorage.getItem(STORAGE_KEY);
    if (saved) {
      try {
        const parsed = JSON.parse(saved);
        appData = { ...appData, ...parsed };
        // Parse dates back to Date objects
        appData.history = appData.history.map(item => ({
          ...item,
          date: new Date(item.date)
        }));
      } catch (e) {
        console.error('Failed to load data:', e);
      }
    }
  }

  // Save data to localStorage
  function saveData() {
    try {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(appData));
    } catch (e) {
      console.error('Failed to save data:', e);
      showToast('ไม่สามารถบันทึกข้อมูล', 'error');
    }
  }

  // ==================== LINE LIFF INITIALIZATION ====================
  async function initLIFF() {
    try {
      await liff.init({ liffId: LIFF_ID });
      
      if (!liff.isLoggedIn()) {
        liff.login();
        return;
      }

      // Get user profile from LINE
      const profile = await liff.getProfile();
      
      // Update app data with LINE profile
      appData.profile.name = profile.displayName || appData.profile.name;
      appData.profile.email = profile.userId || appData.profile.email;
      appData.profile.pictureUrl = profile.pictureUrl;

      // Save and display
      saveData();
      updateProfileDisplay();
      
      // Hide loading screen
      document.getElementById('loading-screen').classList.add('hidden');
      
      showToast(`✅ ยินดีต้อนรับ ${profile.displayName}!`, 'success');
    } catch (error) {
      console.error('LIFF initialization error:', error);
      document.getElementById('loading-screen').classList.add('hidden');
      showToast('⚠️ ไม่สามารถเชื่อมต่อกับ LINE ได้', 'error');
    }
  }

  function closeLIFF() {
    if (liff.isInClient()) {
      liff.closeWindow();
    } else {
      showToast('⚠️ กรุณาเปิดแอปนี้จาก LINE เท่านั้น', 'warning');
    }
  }

  // ==================== UI FUNCTIONS ====================
  function renderStamps() {
    const grid = document.getElementById('stamps-grid');
    grid.innerHTML = '';
    for (let i = 0; i < MAX_STAMPS; i++) {
      const el = document.createElement('div');
      el.className = 'stamp' + (i < appData.stamps ? ' filled' : '');
      grid.appendChild(el);
    }
    const pct = (appData.stamps / MAX_STAMPS) * 100;
    document.getElementById('progress-fill').style.width = pct + '%';
    document.getElementById('stamp-count').textContent = appData.stamps;
    document.getElementById('header-stamps').textContent = `🔥 ${appData.stamps}/${MAX_STAMPS} ดวง`;

    const banner = document.getElementById('discount-banner');
    if (appData.stamps >= MAX_STAMPS) {
      banner.style.display = 'block';
    } else {
      banner.style.display = 'none';
    }
  }

  function renderHistory() {
    const list = document.getElementById('history-list');
    list.innerHTML = '';
    appData.history.forEach(item => {
      const el = document.createElement('div');
      el.className = 'history-item';
      const dateStr = item.date.toLocaleString('th-TH', { day:'numeric', month:'short', year:'numeric', hour:'2-digit', minute:'2-digit' });
      el.innerHTML = `
        <div class="hist-icon">${item.icon}</div>
        <div class="hist-info">
          <div class="hist-title">${item.title}</div>
          <div class="hist-date">${dateStr}</div>
        </div>
        <div class="hist-badge ${item.badgeClass}">${item.badge}</div>
      `;
      list.appendChild(el);
    });
  }

  function updateProfileDisplay() {
    document.getElementById('profile-name-display').textContent = appData.profile.name;
    document.getElementById('profile-email-display').textContent = appData.profile.email;
    document.getElementById('input-name').value = appData.profile.name;
    document.getElementById('input-email').value = appData.profile.email;
    document.getElementById('input-phone').value = appData.profile.phone;
    document.getElementById('total-stamps').textContent = appData.stamps + appData.usedStamps;
    document.getElementById('lifetime-stamps').textContent = appData.stamps + appData.usedStamps;
    document.getElementById('used-stamps').textContent = appData.usedStamps;

    // Update avatar
    const avatarEl = document.getElementById('profile-avatar');
    if (appData.profile.pictureUrl) {
      avatarEl.innerHTML = `<img src="${appData.profile.pictureUrl}" alt="Profile">`;
    } else {
      avatarEl.textContent = '👤';
    }
  }

  function simulateScan() {
    if (appData.stamps >= MAX_STAMPS) {
      // use discount
      document.getElementById('modal-icon').textContent = '🎉';
      document.getElementById('modal-title').textContent = 'ใช้ส่วนลด 10%!';
      document.getElementById('modal-msg').textContent = 'ส่วนลด 10% ถูกใช้แล้ว แสตมป์จะเริ่มนับใหม่';
      document.getElementById('scan-modal').classList.add('show');
      addHistory('ใช้ส่วนลด 10%', '🎉', 'ใช้แล้ว', 'discount');
      appData.usedStamps += appData.stamps;
      appData.stamps = 0;
      showToast('✨ ใช้ส่วนลด 10% สำเร็จ!', 'success');
      setTimeout(renderStamps, 300);
    } else {
      appData.stamps++;
      document.getElementById('modal-icon').textContent = '🔥';
      if (appData.stamps >= MAX_STAMPS) {
        document.getElementById('modal-title').textContent = 'ครบ 5 ดวงแล้ว! 🎊';
        document.getElementById('modal-msg').textContent = 'คุณได้รับสิทธิ์ลด 10% มื้อถัดไปสแกนอีกครั้งเพื่อใช้สิทธิ์';
        showToast('🎉 ครบ 5 ดวงแล้ว! สามารถใช้ส่วนลดได้', 'success');
      } else {
        document.getElementById('modal-title').textContent = 'รับแสตมป์สำเร็จ!';
        document.getElementById('modal-msg').textContent = `คุณได้รับ 1 ดวง รวม ${appData.stamps}/${MAX_STAMPS} ดวง ขอบคุณที่มาอุดหนุนนะคะ 🙏`;
        showToast(`✅ รับแสตมป์สำเร็จ (${appData.stamps}/${MAX_STAMPS})`, 'success');
      }
      document.getElementById('scan-modal').classList.add('show');
      addHistory('รับแสตมป์', '🔥', '+1 ดวง', '');
      renderStamps();
    }
    saveData();
  }

  function addHistory(title, icon, badge, badgeClass) {
    appData.history.unshift({
      title: title,
      icon: icon,
      badge: badge,
      badgeClass: badgeClass,
      date: new Date()
    });
    renderHistory();
    saveData();
  }

  function closeModal() {
    document.getElementById('scan-modal').classList.remove('show');
  }

  function showPage(id) {
    document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
    document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
    document.getElementById('page-' + id).classList.add('active');
    document.getElementById('nav-' + id).classList.add('active');
    
    if (id === 'profile') {
      updateProfileDisplay();
    }
  }

  function filterMenu(category) {
    // Update filter buttons
    document.querySelectorAll('.filter-btn').forEach(btn => btn.classList.remove('active'));
    event.target.classList.add('active');

    // Show/hide categories
    document.querySelectorAll('.menu-category').forEach(cat => {
      if (category === 'all' || cat.dataset.category === category) {
        cat.style.display = 'block';
      } else {
        cat.style.display = 'none';
      }
    });
  }

  function saveProfile() {
    const name = document.getElementById('input-name').value.trim();
    const email = document.getElementById('input-email').value.trim();
    const phone = document.getElementById('input-phone').value.trim();

    if (!name) {
      showToast('⚠️ กรุณากรอกชื่อ-นามสกุล', 'warning');
      return;
    }
    if (!email) {
      showToast('⚠️ กรุณากรอกอีเมล', 'warning');
      return;
    }

    appData.profile = { ...appData.profile, name, email, phone };
    updateProfileDisplay();
    saveData();
    showToast('✅ บันทึกข้อมูลสำเร็จ!', 'success');
  }

  function showToast(message, type = 'success') {
    const container = document.getElementById('toast-container');
    const toast = document.createElement('div');
    toast.className = `toast ${type}`;
    toast.innerHTML = `<span>${message}</span>`;
    container.appendChild(toast);

    setTimeout(() => {
      toast.classList.add('hide');
      setTimeout(() => toast.remove(), 300);
    }, 3000);
  }

  // ==================== QR CODE ====================
  function drawQR() {
    const canvas = document.getElementById('qr-canvas');
    const ctx = canvas.getContext('2d');
    const size = 160;
    const cell = size / 15;
    ctx.fillStyle = 'white';
    ctx.fillRect(0, 0, size, size);

    const pattern = [
      [1,1,1,1,1,1,1,0,0,0,1,1,1,1,1],
      [1,0,0,0,0,0,1,0,1,0,1,0,0,0,1],
      [1,0,1,1,1,0,1,0,0,1,1,0,1,0,1],
      [1,0,1,1,1,0,1,1,0,0,0,0,1,0,1],
      [1,0,1,1,1,0,1,0,1,1,1,0,1,0,1],
      [1,0,0,0,0,0,1,0,0,1,0,0,0,0,1],
      [1,1,1,1,1,1,1,0,1,0,1,1,1,1,1],
      [0,0,0,0,0,0,0,0,1,0,0,0,0,0,0],
      [1,0,1,0,1,1,1,1,1,0,1,0,1,0,1],
      [0,1,0,0,1,0,0,1,0,1,0,1,0,1,0],
      [1,1,1,1,1,1,1,0,1,1,1,0,1,1,1],
      [0,0,0,1,0,0,0,0,0,1,0,1,0,0,0],
      [1,1,0,1,1,0,1,1,0,0,1,0,1,1,0],
      [0,0,0,0,0,0,0,0,1,1,0,1,0,0,1],
      [1,1,1,0,1,1,1,0,1,0,1,0,1,1,1],
    ];

    ctx.fillStyle = '#1a1210';
    pattern.forEach((row, r) => {
      row.forEach((cell_val, c) => {
        if (cell_val) {
          ctx.fillRect(c * cell, r * cell, cell - 1, cell - 1);
        }
      });
    });
  }

  // ==================== INITIALIZATION ====================
  loadData();
  drawQR();
  renderStamps();
  renderHistory();
  updateProfileDisplay();
  
  // Initialize LIFF
  // Add timeout fallback
  const liffTimeout = setTimeout(() => {
    document.getElementById("loading-screen").classList.add("hidden");
  }, 5000);
  initLIFF().finally(() => clearTimeout(liffTimeout));
</script>
</body>
</html>
