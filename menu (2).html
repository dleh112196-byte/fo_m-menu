<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>메뉴판</title>
<link href="https://fonts.googleapis.com/css2?family=Noto+Serif+KR:wght@300;400;500;600&family=Noto+Sans+KR:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --gold: #C9A96E;
    --gold-light: #E8D5B0;
    --cream: #FAF7F2;
    --dark: #1A1612;
    --mid: #3D3530;
    --muted: #7A6E66;
    --border: rgba(201,169,110,0.25);
    --card-bg: #FFFFFF;
    --section-bg: #F5F0E8;
  }
  * { margin:0; padding:0; box-sizing:border-box; }
  body {
    background: var(--cream);
    color: var(--dark);
    font-family: 'Noto Sans KR', sans-serif;
    min-height: 100vh;
  }

  /* ADMIN TOGGLE */
  #admin-bar {
    position: fixed; bottom: 0; left: 0; right: 0;
    background: var(--dark); color: var(--gold);
    text-align: center; padding: 10px;
    font-size: 13px; cursor: pointer;
    z-index: 1000; display: none;
  }
  body.admin-mode #admin-bar { display: block; }

  /* HEADER */
  .site-header {
    background: #3A6B1A;
    padding: 32px 24px 28px;
    text-align: center;
  }
  .restaurant-name {
    font-family: 'Noto Serif KR', serif;
    font-size: clamp(32px, 9vw, 60px);
    font-weight: 300; color: #FFFFFF;
    letter-spacing: 6px; line-height: 1.2;
  }
  .gold-line {
    width: 60px; height: 1px;
    background: var(--gold); margin: 0 auto;
  }

  /* NAV */
  .category-nav {
    position: sticky; top: 0; z-index: 100;
    background: var(--dark);
    border-bottom: 1px solid var(--border);
    overflow-x: auto; white-space: nowrap;
    scrollbar-width: none;
  }
  .category-nav::-webkit-scrollbar { display: none; }
  .nav-inner {
    display: inline-flex; padding: 0 16px;
    gap: 0;
  }
  .nav-btn {
    background: none; border: none;
    color: var(--muted); font-family: 'Noto Sans KR';
    font-size: 13px; padding: 14px 18px;
    cursor: pointer; white-space: nowrap;
    border-bottom: 2px solid transparent;
    transition: all 0.2s;
    letter-spacing: 0.5px;
  }
  .nav-btn:hover, .nav-btn.active {
    color: var(--gold);
    border-bottom-color: var(--gold);
  }

  /* MENU CONTAINER */
  .menu-container { max-width: 680px; margin: 0 auto; padding: 0 16px 120px; }

  /* SECTION */
  .menu-section { padding-top: 48px; }
  .section-header {
    text-align: center; margin-bottom: 32px;
    padding-bottom: 24px;
    border-bottom: 1px solid var(--border);
  }
  .section-label {
    font-size: 10px; letter-spacing: 4px;
    color: var(--gold); text-transform: uppercase;
    display: block; margin-bottom: 8px;
  }
  .section-title {
    font-family: 'Noto Serif KR', serif;
    font-size: 22px; font-weight: 400;
    color: var(--dark);
  }

  /* MENU ITEM */
  .menu-item {
    display: flex; gap: 16px;
    padding: 20px 0;
    border-bottom: 1px solid rgba(0,0,0,0.06);
    position: relative;
  }
  .menu-item:last-child { border-bottom: none; }
  .item-image-wrap {
    width: 88px; height: 88px;
    flex-shrink: 0; border-radius: 8px;
    overflow: hidden;
    background: var(--section-bg);
    position: relative;
  }
  .item-image-wrap img {
    width: 100%; height: 100%; object-fit: cover;
  }
  .item-image-placeholder {
    width: 100%; height: 100%;
    display: flex; align-items: center; justify-content: center;
    font-size: 28px; color: var(--gold);
  }
  .item-info { flex: 1; min-width: 0; }
  .item-top {
    display: flex; justify-content: space-between;
    align-items: flex-start; gap: 8px;
    margin-bottom: 6px;
  }
  .item-name {
    font-family: 'Noto Serif KR', serif;
    font-size: 16px; font-weight: 500;
    color: var(--dark); line-height: 1.3;
    flex: 1;
  }
  .item-price {
    font-size: 15px; font-weight: 500;
    color: var(--gold); white-space: nowrap;
    font-family: 'Noto Serif KR';
    flex-shrink: 0;
  }
  .item-desc {
    font-size: 12.5px; color: var(--muted);
    line-height: 1.7; font-weight: 300;
  }

  /* ADMIN EDIT BUTTON */
  .edit-btn {
    display: none;
    position: absolute; top: 12px; right: 0;
    background: var(--gold); color: var(--dark);
    border: none; border-radius: 4px;
    font-size: 11px; padding: 3px 8px;
    cursor: pointer; font-family: 'Noto Sans KR';
    font-weight: 500;
  }
  body.admin-mode .edit-btn { display: block; }

  /* MODAL */
  .modal-overlay {
    display: none; position: fixed;
    inset: 0; background: rgba(0,0,0,0.7);
    z-index: 2000; align-items: center;
    justify-content: center; padding: 16px;
  }
  .modal-overlay.open { display: flex; }
  .modal {
    background: #fff; border-radius: 12px;
    padding: 24px; width: 100%; max-width: 480px;
    max-height: 90vh; overflow-y: auto;
  }
  .modal h3 {
    font-family: 'Noto Serif KR'; font-size: 18px;
    margin-bottom: 20px; color: var(--dark);
  }
  .form-group { margin-bottom: 16px; }
  .form-group label {
    display: block; font-size: 12px;
    color: var(--muted); margin-bottom: 6px;
    font-weight: 500; letter-spacing: 0.5px;
  }
  .form-group input,
  .form-group textarea {
    width: 100%; border: 1px solid #e0d8cc;
    border-radius: 8px; padding: 10px 12px;
    font-size: 14px; font-family: 'Noto Sans KR';
    color: var(--dark); resize: vertical;
    outline: none;
  }
  .form-group input:focus,
  .form-group textarea:focus { border-color: var(--gold); }
  .form-group textarea { min-height: 80px; }
  .modal-actions {
    display: flex; gap: 8px; margin-top: 20px;
    justify-content: flex-end;
  }
  .btn-save {
    background: var(--gold); color: var(--dark);
    border: none; border-radius: 8px;
    padding: 10px 20px; font-size: 14px;
    font-weight: 500; cursor: pointer;
    font-family: 'Noto Sans KR';
  }
  .btn-cancel {
    background: none; color: var(--muted);
    border: 1px solid #e0d8cc; border-radius: 8px;
    padding: 10px 20px; font-size: 14px;
    cursor: pointer; font-family: 'Noto Sans KR';
  }
  .btn-delete {
    background: none; color: #c0392b;
    border: 1px solid #f5c6c6; border-radius: 8px;
    padding: 10px 20px; font-size: 14px;
    cursor: pointer; font-family: 'Noto Sans KR';
    margin-right: auto;
  }
  .upload-area {
    border: 1.5px dashed #e0d8cc; border-radius: 8px;
    padding: 16px; text-align: center; cursor: pointer;
    color: var(--muted); font-size: 13px;
    margin-bottom: 8px;
  }
  .upload-area:hover { border-color: var(--gold); }
  #image-preview {
    width: 100%; border-radius: 8px;
    margin-top: 8px; display: none;
    max-height: 160px; object-fit: cover;
  }

  /* ADMIN ACCESS */
  .admin-access-btn {
    position: fixed; bottom: 16px; right: 16px;
    background: rgba(26,22,18,0.85);
    border: 1px solid var(--border);
    color: var(--gold); border-radius: 50%;
    width: 44px; height: 44px;
    font-size: 18px; cursor: pointer;
    display: flex; align-items: center;
    justify-content: center; z-index: 999;
    backdrop-filter: blur(8px);
  }

  .password-modal {
    display: none; position: fixed;
    inset: 0; background: rgba(0,0,0,0.7);
    z-index: 3000; align-items: center;
    justify-content: center; padding: 16px;
  }
  .password-modal.open { display: flex; }
  .password-box {
    background: var(--dark); border-radius: 12px;
    padding: 28px 24px; width: 100%; max-width: 320px;
    border: 1px solid var(--border); text-align: center;
  }
  .password-box h3 {
    color: var(--gold); font-family: 'Noto Serif KR';
    font-size: 16px; margin-bottom: 16px;
  }
  .password-box input {
    width: 100%; background: rgba(255,255,255,0.08);
    border: 1px solid var(--border); color: #fff;
    border-radius: 8px; padding: 10px 12px;
    font-size: 14px; text-align: center;
    letter-spacing: 4px; outline: none;
    font-family: 'Noto Sans KR';
    margin-bottom: 12px;
  }
  .password-box input:focus { border-color: var(--gold); }
  .btn-enter {
    width: 100%; background: var(--gold);
    color: var(--dark); border: none;
    border-radius: 8px; padding: 10px;
    font-size: 14px; font-weight: 500;
    cursor: pointer; font-family: 'Noto Sans KR';
  }
  .pw-error {
    color: #e74c3c; font-size: 12px;
    margin-top: 8px; display: none;
  }

  /* FOOTER */
  .footer {
    text-align: center; padding: 32px 24px;
    background: var(--dark);
    color: var(--muted); font-size: 12px;
    letter-spacing: 1px;
  }
  .footer .gold-line { margin: 0 auto 16px; }
</style>
</head>
<body>

<!-- HEADER -->
<header class="site-header">
  <h1 class="restaurant-name">fo_m</h1>
</header>

<!-- CATEGORY NAV -->
<nav class="category-nav">
  <div class="nav-inner" id="nav-inner"></div>
</nav>

<!-- MENU -->
<main class="menu-container" id="menu-container"></main>

<!-- FOOTER -->
<footer class="footer">
  <div class="gold-line"></div>
  <p>모든 요리는 당일 신선한 재료로 준비됩니다</p>
</footer>

<!-- ADMIN ACCESS BUTTON -->
<button class="admin-access-btn" id="admin-access-btn" title="관리자">⚙</button>

<!-- ADMIN BAR -->
<div id="admin-bar" onclick="exitAdmin()">관리자 모드 활성화 중 — 메뉴를 탭하여 수정 | 종료하려면 클릭</div>

<!-- PASSWORD MODAL -->
<div class="password-modal" id="pw-modal">
  <div class="password-box">
    <h3>관리자 접근</h3>
    <input type="password" id="pw-input" placeholder="비밀번호" maxlength="20">
    <button class="btn-enter" onclick="checkPassword()">확인</button>
    <p class="pw-error" id="pw-error">비밀번호가 틀렸습니다</p>
    <button style="background:none;border:none;color:var(--muted);font-size:12px;margin-top:12px;cursor:pointer;font-family:'Noto Sans KR'" onclick="closePwModal()">취소</button>
  </div>
</div>

<!-- EDIT MODAL -->
<div class="modal-overlay" id="edit-modal">
  <div class="modal">
    <h3>메뉴 수정</h3>
    <div class="form-group">
      <label>메뉴 이름</label>
      <input type="text" id="edit-name">
    </div>
    <div class="form-group">
      <label>가격 (만원, 숫자만)</label>
      <input type="text" id="edit-price" placeholder="예: 35">
    </div>
    <div class="form-group">
      <label>설명</label>
      <textarea id="edit-desc"></textarea>
    </div>
    <div class="form-group">
      <label>사진</label>
      <div class="upload-area" onclick="document.getElementById('edit-img-input').click()">
        📷 사진을 탭하여 업로드
      </div>
      <input type="file" id="edit-img-input" accept="image/*" style="display:none">
      <img id="image-preview" alt="preview">
    </div>
    <div class="modal-actions">
      <button class="btn-delete" onclick="deleteItem()">삭제</button>
      <button class="btn-cancel" onclick="closeModal()">취소</button>
      <button class="btn-save" onclick="saveItem()">저장</button>
    </div>
  </div>
</div>

<script>
const ADMIN_PW = '1234';

const DEFAULT_DATA = {
  restaurantName: '레스토랑',
  restaurantSub: 'Seasonal Italian Cuisine',
  categories: [
    {
      id: 'pasta', label: '파스타', items: [
        { id: 'p1', name: '잣소스 와 생트러플 파스타', price: '35', desc: '잣, 연두부로 만든 소스와 생트러플을 곁들인 카펠리니 면', img: '' },
        { id: 'p2', name: '호래기, 쑥버터소스 칼라마라타', price: '28', desc: '쑥버터소스와 호래기프라이, 제철조개, 어란을 곁들인 칼라마라타 파스타', img: '' },
        { id: 'p3', name: '수제판체타와 봄나물장 파스타', price: '26', desc: '치즈, 버터, 마늘로 만든 소스와 수제 판체타, 달래장을 곁들인 먹물 스파게티면', img: '' },
        { id: 'p4', name: '어란 파스타', price: '24', desc: '초리조, 페코리노치즈, 썬드라이토마토, 쥬키니, 세이지레몬버터, 어란으로 맛을 낸 파스타', img: '' },
        { id: 'p5', name: '크림 파스타 or 뇨끼 (+0.2)', price: '22', desc: '고르곤졸라 치즈 소스의 감자 뇨끼', img: '' },
        { id: 'p6', name: '봉골레', price: '22', desc: '제철 조개와 화이트와인으로 맛을 낸 봉골레 파스타', img: '' },
        { id: 'p7', name: '볼로냐식 토마토 라구 파스타 or 뇨끼 (+0.2)', price: '22', desc: '페코리노 치즈로 맛을 낸 볼로냐식 토마토 라구 파스타', img: '' },
      ]
    },
    {
      id: 'seafood', label: '해산물', items: [
        { id: 's1', name: '북해도산 관자 요리', price: '30', desc: '라임, 코코넛소스와 땅콩치즈소스, 루꼴라, 골든키위를 곁들인 북해도산 관자 요리', img: '' },
        { id: 's2', name: '새우 요리 (감보네스)', price: '24', desc: '오렌지 꼬냑소스, 자연산 홍새우', img: '' },
        { id: 's3', name: '문어 요리', price: '27', desc: '당근퓨레, 땅콩, 알배추구이를 곁들인 문어 요리', img: '' },
      ]
    },
    {
      id: 'meat', label: '육류', items: [
        { id: 'm1', name: '살치살 스테이크', price: '43', desc: '감자 메쉬, 포트와인 소스, 참기름 파우더 살치살 스테이크', img: '' },
        { id: 'm2', name: '돼지 항정살 스테이크', price: '35', desc: '사과폼 소스를 곁들인 국내산 돼지 항정살 스테이크', img: '' },
      ]
    },
    {
      id: 'salad', label: '샐러드 & 사이드', items: [
        { id: 'a1', name: '딸기 와 대저토마토 제철 샐러드', price: '', desc: '스트라챠치즈와 비네그렛 드레싱, 딸기, 대저토마토 제철 과일을 활용한 요리', img: '' },
        { id: 'a2', name: '시저 샐러드', price: '14', desc: '시저 드레싱으로 맛을 낸 샐러드', img: '' },
        { id: 'a3', name: '까로짜와 가지 프라이', price: '24', desc: '빵에 두 가지 치즈와 엔초비, 블랙올리브를 채워 말아서 만든 요리와 가지프라이', img: '' },
        { id: 'a4', name: '라자냐', price: '27', desc: '감자와 가지를 구워 겹겹이 쌓은 그리스식 라자냐', img: '' },
        { id: 'a5', name: '프렌치 프라이', price: '10', desc: '', img: '' },
      ]
    }
  ]
};

let menuData = JSON.parse(localStorage.getItem('menuData')) || DEFAULT_DATA;
let editingId = null;
let isAdmin = false;
let pendingImgData = null;

function save() { localStorage.setItem('menuData', JSON.stringify(menuData)); }

function render() {
  const nav = document.getElementById('nav-inner');
  const container = document.getElementById('menu-container');
  nav.innerHTML = '';
  container.innerHTML = '';

  menuData.categories.forEach((cat, ci) => {
    const btn = document.createElement('button');
    btn.className = 'nav-btn' + (ci === 0 ? ' active' : '');
    btn.textContent = cat.label;
    btn.onclick = () => {
      document.querySelectorAll('.nav-btn').forEach(b => b.classList.remove('active'));
      btn.classList.add('active');
      document.getElementById('sec-' + cat.id).scrollIntoView({ behavior: 'smooth', block: 'start' });
    };
    nav.appendChild(btn);

    const section = document.createElement('section');
    section.className = 'menu-section';
    section.id = 'sec-' + cat.id;
    section.innerHTML = `
      <div class="section-header">
        <span class="section-label">Menu</span>
        <h2 class="section-title">${cat.label}</h2>
      </div>
    `;

    cat.items.forEach(item => {
      const el = document.createElement('div');
      el.className = 'menu-item';
      el.innerHTML = `
        <div class="item-image-wrap">
          ${item.img
            ? `<img src="${item.img}" alt="${item.name}">`
            : `<div class="item-image-placeholder">🍽</div>`}
        </div>
        <div class="item-info">
          <div class="item-top">
            <span class="item-name">${item.name}</span>
            ${item.price ? `<span class="item-price">${item.price}.</span>` : ''}
          </div>
          ${item.desc ? `<p class="item-desc">${item.desc}</p>` : ''}
        </div>
        <button class="edit-btn" onclick="openEdit('${cat.id}','${item.id}')">수정</button>
      `;
      section.appendChild(el);
    });

    container.appendChild(section);
  });
}

function openEdit(catId, itemId) {
  const cat = menuData.categories.find(c => c.id === catId);
  const item = cat.items.find(i => i.id === itemId);
  editingId = { catId, itemId };
  pendingImgData = null;
  document.getElementById('edit-name').value = item.name;
  document.getElementById('edit-price').value = item.price;
  document.getElementById('edit-desc').value = item.desc;
  const prev = document.getElementById('image-preview');
  if (item.img) { prev.src = item.img; prev.style.display = 'block'; }
  else { prev.style.display = 'none'; }
  document.getElementById('edit-modal').classList.add('open');
}

function closeModal() {
  document.getElementById('edit-modal').classList.remove('open');
  editingId = null; pendingImgData = null;
}

function saveItem() {
  if (!editingId) return;
  const cat = menuData.categories.find(c => c.id === editingId.catId);
  const item = cat.items.find(i => i.id === editingId.itemId);
  item.name = document.getElementById('edit-name').value;
  item.price = document.getElementById('edit-price').value;
  item.desc = document.getElementById('edit-desc').value;
  if (pendingImgData) item.img = pendingImgData;
  save(); render(); closeModal();
}

function deleteItem() {
  if (!editingId || !confirm('이 메뉴를 삭제하시겠습니까?')) return;
  const cat = menuData.categories.find(c => c.id === editingId.catId);
  cat.items = cat.items.filter(i => i.id !== editingId.itemId);
  save(); render(); closeModal();
}

document.getElementById('edit-img-input').addEventListener('change', e => {
  const file = e.target.files[0];
  if (!file) return;
  const reader = new FileReader();
  reader.onload = ev => {
    pendingImgData = ev.target.result;
    const prev = document.getElementById('image-preview');
    prev.src = pendingImgData; prev.style.display = 'block';
  };
  reader.readAsDataURL(file);
});

document.getElementById('admin-access-btn').onclick = () => {
  if (isAdmin) { exitAdmin(); return; }
  document.getElementById('pw-modal').classList.add('open');
  document.getElementById('pw-input').value = '';
  document.getElementById('pw-error').style.display = 'none';
  setTimeout(() => document.getElementById('pw-input').focus(), 100);
};

document.getElementById('pw-input').addEventListener('keydown', e => {
  if (e.key === 'Enter') checkPassword();
});

function checkPassword() {
  const val = document.getElementById('pw-input').value;
  if (val === ADMIN_PW) {
    isAdmin = true;
    document.body.classList.add('admin-mode');
    closePwModal();
  } else {
    document.getElementById('pw-error').style.display = 'block';
  }
}

function closePwModal() {
  document.getElementById('pw-modal').classList.remove('open');
}

function exitAdmin() {
  isAdmin = false;
  document.body.classList.remove('admin-mode');
}

document.getElementById('edit-modal').addEventListener('click', e => {
  if (e.target === document.getElementById('edit-modal')) closeModal();
});

document.getElementById('pw-modal').addEventListener('click', e => {
  if (e.target === document.getElementById('pw-modal')) closePwModal();
});

// Intersection observer for nav highlight
const observer = new IntersectionObserver(entries => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      const id = entry.target.id.replace('sec-', '');
      document.querySelectorAll('.nav-btn').forEach((btn, i) => {
        btn.classList.toggle('active', menuData.categories[i]?.id === id);
      });
    }
  });
}, { rootMargin: '-40% 0px -50% 0px' });

render();

setTimeout(() => {
  document.querySelectorAll('.menu-section').forEach(s => observer.observe(s));
}, 100);
</script>
</body>
</html>
