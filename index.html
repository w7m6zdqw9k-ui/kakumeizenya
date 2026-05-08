<!DOCTYPE html>

<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="theme-color" content="#4f46e5">
<title>家計やりくり</title>
<style>
* { box-sizing: border-box; -webkit-tap-highlight-color: transparent; }
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Hiragino Sans", "Yu Gothic", sans-serif;
  background: #f3f4f6;
  margin: 0;
  padding: 0;
  color: #1f2937;
  padding-bottom: 40px;
  -webkit-font-smoothing: antialiased;
}
.app { max-width: 600px; margin: 0 auto; }

.header {
background: linear-gradient(135deg, #4f46e5 0%, #7c3aed 100%);
color: white;
padding: 16px 16px 12px;
position: sticky;
top: 0;
z-index: 50;
box-shadow: 0 2px 8px rgba(0,0,0,0.08);
}
.header-top { display: flex; justify-content: space-between; align-items: center; margin-bottom: 6px; }
.header h1 { margin: 0; font-size: 18px; font-weight: 600; }
.menu-btn {
background: rgba(255,255,255,0.2); color: white; border: none;
width: 32px; height: 32px; border-radius: 8px; font-size: 18px; cursor: pointer;
display: flex; align-items: center; justify-content: center;
}
.month-nav { display: flex; align-items: center; gap: 10px; }
.month-display { font-size: 14px; font-weight: 500; }
.month-nav button {
background: rgba(255,255,255,0.2); color: white; border: none;
width: 28px; height: 28px; border-radius: 8px; font-size: 14px; cursor: pointer;
display: flex; align-items: center; justify-content: center;
}
.today-btn {
margin-left: auto !important;
width: auto !important;
padding: 4px 10px !important;
font-size: 11px !important;
}

.summary-card {
background: white;
margin: 12px;
padding: 16px;
border-radius: 14px;
box-shadow: 0 1px 3px rgba(0,0,0,0.05);
}
.summary-row { display: flex; justify-content: space-between; align-items: baseline; margin: 6px 0; }
.summary-label { font-size: 13px; color: #6b7280; }
.summary-value { font-size: 18px; font-weight: 600; font-variant-numeric: tabular-nums; }
.summary-value.income { color: #059669; }
.summary-value.payment { color: #dc2626; }
.summary-value.remain { color: #4f46e5; font-size: 22px; }
.divider { border-top: 1px solid #e5e7eb; margin: 10px 0; }

.progress-container {
background: #e5e7eb;
border-radius: 8px;
height: 8px;
overflow: hidden;
margin: 8px 0 4px;
}
.progress-bar {
height: 100%;
background: linear-gradient(90deg, #10b981, #059669);
transition: width 0.3s ease;
}
.progress-bar.warning { background: linear-gradient(90deg, #f59e0b, #d97706); }
.progress-bar.danger { background: linear-gradient(90deg, #ef4444, #dc2626); }
.progress-text { font-size: 11px; color: #6b7280; text-align: right; }

.tabs {
display: flex;
background: white;
margin: 0 12px;
border-radius: 12px;
padding: 4px;
box-shadow: 0 1px 3px rgba(0,0,0,0.05);
margin-bottom: 12px;
}
.tab {
flex: 1;
padding: 10px 4px;
text-align: center;
font-size: 13px;
font-weight: 500;
color: #6b7280;
border-radius: 8px;
cursor: pointer;
transition: all 0.2s;
}
.tab.active {
background: #4f46e5;
color: white;
}

.section { margin: 0 12px 12px; }
.section-header {
display: flex;
justify-content: space-between;
align-items: center;
margin-bottom: 8px;
padding: 0 4px;
flex-wrap: wrap;
gap: 6px;
}
.section-title { font-size: 14px; font-weight: 600; color: #374151; }
.section-actions { display: flex; gap: 6px; }
.section-action {
font-size: 12px; color: #4f46e5; background: white;
border: 1px solid #c7d2fe; cursor: pointer; padding: 4px 10px;
border-radius: 6px; font-family: inherit;
}
.section-action.active { background: #4f46e5; color: white; }

.card {
background: white;
border-radius: 12px;
padding: 12px;
margin-bottom: 8px;
box-shadow: 0 1px 3px rgba(0,0,0,0.05);
transition: opacity 0.2s, border 0.2s;
}
.card.paid { background: #f0fdf4; border: 1px solid #bbf7d0; }
.card.dragging { opacity: 0.5; }
.card.drag-over { border-top: 3px solid #4f46e5; }

.card-row {
display: flex;
align-items: center;
gap: 8px;
margin-bottom: 6px;
}
.card-row:last-child { margin-bottom: 0; }

input[type=“text”], input[type=“number”], textarea {
padding: 10px 12px;
font-size: 15px;
border: 1px solid #e5e7eb;
border-radius: 8px;
background: #f9fafb;
width: 100%;
-webkit-appearance: none;
appearance: none;
font-family: inherit;
}
input[type=“number”] { font-variant-numeric: tabular-nums; }
input:focus, textarea:focus { outline: none; border-color: #4f46e5; background: white; }

textarea {
resize: vertical;
min-height: 38px;
font-size: 13px;
line-height: 1.4;
}

.input-name { flex: 1; min-width: 0; }
.input-amount { width: 110px; text-align: right; }
.input-amount-display { width: 110px; text-align: right; font-variant-numeric: tabular-nums; }

.drag-handle {
width: 28px; height: 28px;
display: flex; align-items: center; justify-content: center;
color: #9ca3af; cursor: grab;
flex-shrink: 0;
font-size: 16px;
user-select: none;
touch-action: none;
}
.drag-handle:active { cursor: grabbing; }
.priority-num {
width: 26px; height: 26px;
background: #ede9fe; color: #6d28d9;
border-radius: 6px;
display: flex; align-items: center; justify-content: center;
font-size: 12px; font-weight: 600;
flex-shrink: 0;
}

.btn {
padding: 10px 14px;
font-size: 14px;
font-weight: 500;
border: none;
border-radius: 8px;
cursor: pointer;
transition: all 0.15s;
font-family: inherit;
white-space: nowrap;
}
.btn:active { transform: scale(0.96); }
.btn-primary { background: #4f46e5; color: white; }
.btn-success { background: #10b981; color: white; }
.btn-danger { background: #ef4444; color: white; }
.btn-ghost { background: #f3f4f6; color: #374151; }
.btn-icon { width: 36px; height: 36px; padding: 0; display: flex; align-items: center; justify-content: center; }
.btn-add {
width: 100%;
background: white;
border: 2px dashed #d1d5db;
color: #6b7280;
padding: 12px;
margin-top: 4px;
}

.checkbox {
width: 26px;
height: 26px;
border: 2px solid #d1d5db;
border-radius: 6px;
display: flex;
align-items: center;
justify-content: center;
cursor: pointer;
transition: all 0.15s;
flex-shrink: 0;
background: white;
}
.checkbox.checked {
background: #10b981;
border-color: #10b981;
}
.checkbox.checked::after {
content: “✓”;
color: white;
font-size: 16px;
font-weight: bold;
}

.note-toggle {
font-size: 11px;
color: #6b7280;
background: none;
border: none;
cursor: pointer;
padding: 4px 0;
font-family: inherit;
}
.note-area {
display: none;
margin-top: 6px;
}
.note-area.show { display: block; }

.allocation-card {
background: white;
border-radius: 12px;
padding: 14px;
margin-bottom: 8px;
box-shadow: 0 1px 3px rgba(0,0,0,0.05);
border-left: 4px solid #10b981;
}
.allocation-card.shortage { border-left-color: #ef4444; }
.allocation-card.partial { border-left-color: #f59e0b; }
.allocation-card.paid-card { border-left-color: #3b82f6; opacity: 0.7; }
.allocation-name {
font-size: 15px;
font-weight: 600;
display: flex;
justify-content: space-between;
align-items: center;
margin-bottom: 8px;
gap: 8px;
}
.priority-badge {
background: #ede9fe;
color: #6d28d9;
font-size: 11px;
padding: 3px 8px;
border-radius: 10px;
font-weight: 500;
white-space: nowrap;
}
.allocation-detail {
font-size: 13px;
color: #6b7280;
display: flex;
justify-content: space-between;
margin: 4px 0;
}
.allocation-note {
font-size: 12px;
color: #6b7280;
background: #f9fafb;
padding: 6px 8px;
border-radius: 6px;
margin-top: 6px;
white-space: pre-wrap;
line-height: 1.4;
}
.amount-positive { color: #059669; font-weight: 500; }
.amount-negative { color: #dc2626; font-weight: 600; }
.status-badge {
display: inline-block;
font-size: 11px;
padding: 4px 10px;
border-radius: 10px;
font-weight: 500;
margin-top: 6px;
}
.status-ok { background: #d1fae5; color: #065f46; }
.status-shortage { background: #fee2e2; color: #991b1b; }
.status-paid { background: #dbeafe; color: #1e40af; }

.history-item {
display: flex;
justify-content: space-between;
align-items: center;
padding: 10px 12px;
background: white;
border-radius: 8px;
margin-bottom: 6px;
box-shadow: 0 1px 2px rgba(0,0,0,0.04);
font-size: 14px;
}
.history-meta { color: #6b7280; font-size: 12px; margin-top: 2px; }
.history-amount { font-weight: 600; color: #059669; font-variant-numeric: tabular-nums; }
.history-delete {
background: none; border: none; color: #ef4444;
cursor: pointer; padding: 4px 8px; font-size: 18px;
}

.empty-state {
text-align: center;
padding: 30px 20px;
color: #9ca3af;
font-size: 13px;
background: white;
border-radius: 12px;
}
.empty-icon { font-size: 32px; margin-bottom: 8px; }

.modal-overlay {
position: fixed; inset: 0;
background: rgba(0,0,0,0.5);
display: none; align-items: center; justify-content: center;
z-index: 100; padding: 20px;
}
.modal-overlay.show { display: flex; }
.modal {
background: white;
border-radius: 16px;
padding: 20px;
width: 100%;
max-width: 380px;
animation: slideUp 0.25s ease;
max-height: 90vh;
overflow-y: auto;
}
@keyframes slideUp {
from { transform: translateY(20px); opacity: 0; }
to { transform: translateY(0); opacity: 1; }
}
.modal h3 { margin: 0 0 12px; font-size: 16px; }
.modal p { margin: 0 0 16px; font-size: 14px; color: #6b7280; line-height: 1.5; white-space: pre-wrap; }
.modal-actions { display: flex; gap: 8px; }
.modal-actions .btn { flex: 1; }

.menu-item {
display: flex; align-items: center; gap: 12px;
padding: 14px 12px;
border-radius: 8px;
cursor: pointer;
font-size: 15px;
transition: background 0.15s;
}
.menu-item:hover, .menu-item:active { background: #f3f4f6; }
.menu-item .icon { font-size: 20px; }
.menu-divider { border-top: 1px solid #e5e7eb; margin: 8px 0; }

.archive-month {
background: white;
border-radius: 12px;
padding: 14px;
margin-bottom: 8px;
box-shadow: 0 1px 3px rgba(0,0,0,0.05);
cursor: pointer;
}
.archive-title { font-weight: 600; margin-bottom: 8px; font-size: 15px; }
.archive-stat { font-size: 12px; color: #6b7280; display: flex; justify-content: space-between; margin: 3px 0; }
.archive-stat b { color: #1f2937; font-variant-numeric: tabular-nums; }

.toast {
position: fixed;
bottom: 30px;
left: 50%;
transform: translateX(-50%) translateY(100px);
background: #1f2937;
color: white;
padding: 10px 20px;
border-radius: 24px;
font-size: 14px;
z-index: 200;
opacity: 0;
transition: all 0.3s ease;
pointer-events: none;
white-space: nowrap;
max-width: 90vw;
}
.toast.show { transform: translateX(-50%) translateY(0); opacity: 1; }

.help-text {
font-size: 11px;
color: #9ca3af;
margin-top: 4px;
padding: 0 4px;
margin-bottom: 6px;
}
</style>

</head>
<body>

<div class="app">
  <div class="header">
    <div class="header-top">
      <h1>💰 家計やりくり</h1>
      <button class="menu-btn" onclick="openMenu()" title="メニュー">☰</button>
    </div>
    <div class="month-nav">
      <button onclick="changeMonth(-1)">◀</button>
      <span class="month-display" id="monthDisplay">2026年5月</span>
      <button onclick="changeMonth(1)">▶</button>
      <button class="today-btn" onclick="goToCurrentMonth()">今月へ</button>
    </div>
  </div>

  <div class="summary-card">
    <div class="summary-row">
      <span class="summary-label">💵 今月の入金</span>
      <span class="summary-value income"><span id="monthIncome">0</span>円</span>
    </div>
    <div class="summary-row">
      <span class="summary-label">💳 未払い合計</span>
      <span class="summary-value payment"><span id="paymentTotal">0</span>円</span>
    </div>
    <div class="summary-row" id="paidPaymentRow" style="display:none">
      <span class="summary-label" style="color:#059669">✓ 支払い済み</span>
      <span class="summary-value" style="color:#059669;font-size:15px">－<span id="paidPaymentAmt">0</span>円</span>
    </div>
    <div class="progress-container">
      <div class="progress-bar" id="progressBar" style="width:0%"></div>
    </div>
    <div class="progress-text" id="progressText">支払いカバー率 0%</div>
    <div class="divider"></div>
    <div class="summary-row">
      <span class="summary-label">📊 残り（余り）</span>
      <span class="summary-value remain"><span id="remain">0</span>円</span>
    </div>
  </div>

  <div class="tabs">
    <div class="tab active" onclick="switchTab('income')">収入</div>
    <div class="tab" onclick="switchTab('payment')">支払い</div>
    <div class="tab" onclick="switchTab('allocation')">振り分け</div>
    <div class="tab" onclick="switchTab('history')">履歴</div>
  </div>

  <div id="tab-income" class="tab-content">
    <div class="section">
      <div class="section-header">
        <span class="section-title">収入元</span>
      </div>
      <div class="help-text">給料・副業など、繰り返し使う収入元を登録します。「入金」ボタンで履歴に記録されます。</div>
      <div id="incomeList"></div>
      <button class="btn btn-add" onclick="addIncome()">＋ 収入元を追加</button>
    </div>

```
<div class="section">
  <div class="section-header">
    <span class="section-title">入金履歴（今月）</span>
    <button class="section-action" onclick="resetMonthIncome()">クリア</button>
  </div>
  <div id="incomeHistoryList"></div>
</div>
```

  </div>

  <div id="tab-payment" class="tab-content" style="display:none">
    <div class="section">
      <div class="section-header">
        <span class="section-title">今月の支払い</span>
        <div class="section-actions">
          <button class="section-action" id="reorderBtn" onclick="toggleReorderMode()">並べ替え</button>
          <button class="section-action" onclick="copyFromLastMonth()">先月をコピー</button>
        </div>
      </div>
      <div class="help-text" id="paymentHelpText">優先順位は上から順（番号で表示）。チェックで支払い完了。</div>
      <div id="paymentList"></div>
      <button class="btn btn-add" onclick="addPayment()">＋ 支払いを追加</button>
    </div>
  </div>

  <div id="tab-allocation" class="tab-content" style="display:none">
    <div class="section">
      <div class="section-header">
        <span class="section-title">振り分け結果</span>
      </div>
      <div class="help-text">優先順位の高い順に入金額を割り当てます。支払い済みは別枠で表示されます。</div>
      <div id="allocation"></div>
    </div>
  </div>

  <div id="tab-history" class="tab-content" style="display:none">
    <div class="section">
      <div class="section-header">
        <span class="section-title">過去の月（記録あり）</span>
      </div>
      <div id="archiveList"></div>
    </div>
  </div>
</div>

<div class="modal-overlay" id="modal">
  <div class="modal">
    <h3 id="modalTitle">確認</h3>
    <p id="modalMessage">本当に実行しますか？</p>
    <div class="modal-actions">
      <button class="btn btn-ghost" onclick="closeModal()">キャンセル</button>
      <button class="btn btn-primary" id="modalConfirm">OK</button>
    </div>
  </div>
</div>

<div class="modal-overlay" id="menuModal">
  <div class="modal">
    <h3>メニュー</h3>
    <div class="menu-item" onclick="exportData()">
      <span class="icon">📤</span>
      <div>
        <div>データをエクスポート</div>
        <div style="font-size:11px;color:#9ca3af">バックアップ用JSONファイル</div>
      </div>
    </div>
    <div class="menu-item" onclick="document.getElementById('importFile').click()">
      <span class="icon">📥</span>
      <div>
        <div>データをインポート</div>
        <div style="font-size:11px;color:#9ca3af">JSONファイルから復元</div>
      </div>
    </div>
    <input type="file" id="importFile" accept=".json,application/json" style="display:none" onchange="importData(event)">
    <div class="menu-divider"></div>
    <div class="menu-item" onclick="deleteAllData()" style="color:#dc2626">
      <span class="icon">⚠️</span>
      <div>
        <div>全データを削除</div>
        <div style="font-size:11px;color:#9ca3af">取り消しできません</div>
      </div>
    </div>
    <div class="modal-actions" style="margin-top:12px">
      <button class="btn btn-ghost" onclick="closeMenu()">閉じる</button>
    </div>
  </div>
</div>

<div class="toast" id="toast"></div>

<script>
let data = {
  currentMonth: getCurrentMonthKey(),
  incomeTemplates: [],
  months: {}
};

let currentTab = 'income';
let reorderMode = false;
let openNotes = {};

function getCurrentMonthKey() {
  const d = new Date();
  return `${d.getFullYear()}-${String(d.getMonth() + 1).padStart(2, '0')}`;
}

function formatMonthDisplay(key) {
  const [y, m] = key.split('-');
  return `${y}年${parseInt(m)}月`;
}

function yen(num) { return Number(num || 0).toLocaleString(); }

function formatAmountInput(el) {
  // フォーカスが外れたらカンマ表示
  const raw = el.value.replace(/,/g, '');
  const num = Number(raw);
  if (!isNaN(num) && raw !== '') {
    el.value = num.toLocaleString();
  }
}
function unformatAmountInput(el) {
  // フォーカス時はカンマ除去して数字入力モードに
  el.value = el.value.replace(/,/g, '');
}
function getAmountValue(el) {
  return el.value.replace(/,/g, '');
}

function escapeHtml(str) {
  return String(str || '')
    .replace(/&/g, '&amp;')
    .replace(/</g, '&lt;')
    .replace(/>/g, '&gt;')
    .replace(/"/g, '&quot;')
    .replace(/'/g, '&#039;');
}

function formatDate(iso) {
  const d = new Date(iso);
  return `${d.getMonth() + 1}/${d.getDate()} ${String(d.getHours()).padStart(2, '0')}:${String(d.getMinutes()).padStart(2, '0')}`;
}

function showToast(msg) {
  const t = document.getElementById('toast');
  t.innerText = msg;
  t.classList.add('show');
  setTimeout(() => t.classList.remove('show'), 2000);
}

function showModal(title, message, onConfirm) {
  document.getElementById('modalTitle').innerText = title;
  document.getElementById('modalMessage').innerText = message;
  const btn = document.getElementById('modalConfirm');
  btn.onclick = () => { onConfirm(); closeModal(); };
  document.getElementById('modal').classList.add('show');
}

function closeModal() {
  document.getElementById('modal').classList.remove('show');
}

function openMenu() {
  document.getElementById('menuModal').classList.add('show');
}

function closeMenu() {
  document.getElementById('menuModal').classList.remove('show');
}

function save() {
  try {
    localStorage.setItem('budgetAppData_v3', JSON.stringify(data));
  } catch (e) {
    showToast('保存エラー：容量不足の可能性');
  }
}

function load() {
  let saved = localStorage.getItem('budgetAppData_v3');
  if (!saved) saved = localStorage.getItem('budgetAppData_v2');
  if (saved) {
    try {
      data = JSON.parse(saved);
    } catch (e) {
      console.error('データ読込エラー', e);
    }
  }
  if (!data.currentMonth) data.currentMonth = getCurrentMonthKey();
  if (!data.months) data.months = {};
  if (!data.months[data.currentMonth]) {
    data.months[data.currentMonth] = { payments: [], history: [] };
  }
  if (!data.incomeTemplates) data.incomeTemplates = [];

  Object.values(data.months).forEach(m => {
    if (!m.payments) m.payments = [];
    if (!m.history) m.history = [];
    if (!m.recordedTemplates) m.recordedTemplates = [];
    m.payments.forEach(p => {
      if (p.note === undefined) p.note = '';
    });
  });
}

function getMonthData() {
  if (!data.months[data.currentMonth]) {
    data.months[data.currentMonth] = { payments: [], history: [], recordedTemplates: [] };
  }
  if (!data.months[data.currentMonth].recordedTemplates) {
    data.months[data.currentMonth].recordedTemplates = [];
  }
  return data.months[data.currentMonth];
}

function changeMonth(diff) {
  const [y, m] = data.currentMonth.split('-').map(Number);
  const d = new Date(y, m - 1 + diff, 1);
  data.currentMonth = `${d.getFullYear()}-${String(d.getMonth() + 1).padStart(2, '0')}`;
  if (!data.months[data.currentMonth]) {
    data.months[data.currentMonth] = { payments: [], history: [] };
  }
  reorderMode = false;
  openNotes = {};
  save();
  render();
}

function goToCurrentMonth() {
  data.currentMonth = getCurrentMonthKey();
  if (!data.months[data.currentMonth]) {
    data.months[data.currentMonth] = { payments: [], history: [] };
  }
  reorderMode = false;
  openNotes = {};
  save();
  render();
}

function switchTab(tab) {
  currentTab = tab;
  const tabs = ['income', 'payment', 'allocation', 'history'];
  document.querySelectorAll('.tab').forEach((t, i) => {
    t.classList.toggle('active', tabs[i] === tab);
  });
  document.querySelectorAll('.tab-content').forEach(c => c.style.display = 'none');
  document.getElementById(`tab-${tab}`).style.display = 'block';
}

function addIncome() {
  data.incomeTemplates.push({ name: '', amount: '' });
  save(); render();
}

function updateIncomeTemplate(i, key, value) {
  if (!data.incomeTemplates[i]) return;
  data.incomeTemplates[i][key] = value;
  save();
}

function deleteIncomeTemplate(i) {
  showModal('削除確認', '収入元を削除しますか？\n（入金履歴は残ります）', () => {
    data.incomeTemplates.splice(i, 1);
    save(); render();
  });
}

function recordIncome(i) {
  const t = data.incomeTemplates[i];
  const amount = Number(t.amount || 0);
  if (amount <= 0) { showToast('金額を入力してください'); return; }
  const md = getMonthData();
  md.history.push({
    name: t.name || '収入',
    amount: amount,
    date: new Date().toISOString()
  });
  // 入金済みフラグをセット
  if (!md.recordedTemplates.includes(i)) {
    md.recordedTemplates.push(i);
  }
  save(); render();
  showToast(`${yen(amount)}円を記録しました`);
}

function deleteHistoryItem(idx) {
  showModal('削除確認', 'この入金記録を削除しますか？\n削除するとその方の入金ボタンも元に戻ります。', () => {
    const md = getMonthData();
    const deletedName = md.history[idx]?.name;
    md.history.splice(idx, 1);

    // 同じ名前の収入元のインデックスを探してフラグを解除
    if (deletedName) {
      data.incomeTemplates.forEach((t, i) => {
        const tName = t.name || '収入';
        if (tName === deletedName) {
          // まだ履歴に同じ名前が残っていなければフラグ解除
          const stillExists = md.history.some(h => h.name === tName);
          if (!stillExists) {
            md.recordedTemplates = md.recordedTemplates.filter(r => r !== i);
          }
        }
      });
    }
    save(); render();
  });
}

function resetMonthIncome() {
  const cnt = getMonthData().history.length;
  if (cnt === 0) { showToast('履歴はありません'); return; }
  showModal('クリア確認', `今月の入金履歴${cnt}件をすべて削除しますか？\n（この操作は取り消せません）`, () => {
    const md2 = getMonthData();
    md2.history = [];
    md2.recordedTemplates = [];
    save(); render();
    showToast('入金履歴をクリアしました');
  });
}

function addPayment() {
  getMonthData().payments.push({
    name: '', amount: '', note: '', paid: false
  });
  save(); render();
}

function updatePayment(i, key, value) {
  const md = getMonthData();
  if (!md.payments[i]) return;
  md.payments[i][key] = value;
  save();
  if (key !== 'note') calculate();
}

function deletePayment(i) {
  showModal('削除確認', 'この支払いを削除しますか？', () => {
    getMonthData().payments.splice(i, 1);
    delete openNotes[i];
    save(); render();
  });
}

function togglePaid(i) {
  const p = getMonthData().payments[i];
  if (!p) return;
  p.paid = !p.paid;
  save(); render();
  if (p.paid) showToast('✓ 支払い完了');
}

function toggleNote(i) {
  openNotes[i] = !openNotes[i];
  render();
}

function toggleReorderMode() {
  reorderMode = !reorderMode;
  render();
}

function copyFromLastMonth() {
  const [y, m] = data.currentMonth.split('-').map(Number);
  const lastDate = new Date(y, m - 2, 1);
  const lastKey = `${lastDate.getFullYear()}-${String(lastDate.getMonth() + 1).padStart(2, '0')}`;
  const lastData = data.months[lastKey];

  if (!lastData || !lastData.payments || lastData.payments.length === 0) {
    showToast('先月のデータがありません');
    return;
  }

  const md = getMonthData();
  const existingCount = md.payments.length;

  showModal(
    'コピー確認',
    `${formatMonthDisplay(lastKey)}の支払い${lastData.payments.length}件を${existingCount > 0 ? '追加で' : ''}コピーしますか？\n（メモも引継ぎ、支払い済みフラグはリセットされます）`,
    () => {
      lastData.payments.forEach(p => {
        md.payments.push({
          name: p.name,
          amount: p.amount,
          note: p.note || '',
          paid: false
        });
      });
      save(); render();
      showToast(`${lastData.payments.length}件をコピーしました`);
    }
  );
}

// ドラッグ＆ドロップ（PC）
let dragSrcIdx = null;

function onDragStart(e, idx) {
  dragSrcIdx = idx;
  e.target.classList.add('dragging');
  e.dataTransfer.effectAllowed = 'move';
  try { e.dataTransfer.setData('text/plain', String(idx)); } catch(_){}
}

function onDragEnd(e) {
  e.target.classList.remove('dragging');
  document.querySelectorAll('.card.drag-over').forEach(el => el.classList.remove('drag-over'));
  dragSrcIdx = null;
}

function onDragOver(e, idx) {
  e.preventDefault();
  e.dataTransfer.dropEffect = 'move';
  document.querySelectorAll('.card.drag-over').forEach(el => el.classList.remove('drag-over'));
  if (dragSrcIdx !== null && dragSrcIdx !== idx) {
    e.currentTarget.classList.add('drag-over');
  }
}

function onDrop(e, dstIdx) {
  e.preventDefault();
  if (dragSrcIdx === null || dragSrcIdx === dstIdx) return;
  const md = getMonthData();
  const item = md.payments.splice(dragSrcIdx, 1)[0];
  md.payments.splice(dstIdx, 0, item);
  openNotes = {};
  save(); render();
  showToast('並べ替えました');
}

// タッチ対応の並べ替え
let touchDragIdx = null;

function onTouchStart(e, idx) {
  if (!reorderMode) return;
  touchDragIdx = idx;
  const card = e.currentTarget.closest('.card');
  if (card) card.style.opacity = '0.5';
}

function onTouchMove(e) {
  if (touchDragIdx === null) return;
  e.preventDefault();
  const touch = e.touches[0];
  const elem = document.elementFromPoint(touch.clientX, touch.clientY);
  const targetCard = elem ? elem.closest('.card[data-idx]') : null;
  document.querySelectorAll('.card.drag-over').forEach(el => el.classList.remove('drag-over'));
  if (targetCard) {
    const idx = Number(targetCard.dataset.idx);
    if (idx !== touchDragIdx) targetCard.classList.add('drag-over');
  }
}

function onTouchEnd(e) {
  if (touchDragIdx === null) return;
  const touch = e.changedTouches[0];
  const elem = document.elementFromPoint(touch.clientX, touch.clientY);
  const targetCard = elem ? elem.closest('.card[data-idx]') : null;
  if (targetCard) {
    const dstIdx = Number(targetCard.dataset.idx);
    if (dstIdx !== touchDragIdx) {
      const md = getMonthData();
      const item = md.payments.splice(touchDragIdx, 1)[0];
      md.payments.splice(dstIdx, 0, item);
      openNotes = {};
      save();
      showToast('並べ替えました');
    }
  }
  document.querySelectorAll('.card').forEach(c => {
    c.style.opacity = '';
    c.classList.remove('drag-over');
  });
  touchDragIdx = null;
  render();
}

function render() {
  document.getElementById('monthDisplay').innerText = formatMonthDisplay(data.currentMonth);
  renderIncomeTemplates();
  renderIncomeHistory();
  renderPayments();
  renderAllocation();
  renderArchive();
  calculate();

  const btn = document.getElementById('reorderBtn');
  if (btn) {
    btn.classList.toggle('active', reorderMode);
    btn.innerText = reorderMode ? '完了' : '並べ替え';
  }
  const helpText = document.getElementById('paymentHelpText');
  if (helpText) {
    helpText.innerText = reorderMode
      ? 'ハンドル(⋮⋮)をドラッグして並べ替え。上にあるほど優先度が高い。'
      : '優先順位は上から順（番号で表示）。チェックで支払い完了。';
  }
}

function renderIncomeTemplates() {
  const list = document.getElementById("incomeList");
  const md = getMonthData();
  if (data.incomeTemplates.length === 0) {
    list.innerHTML = "<div class=\"empty-state\"><div class=\"empty-icon\">💼</div><div>収入元を追加してください<br>(給料、副業など)</div></div>";
    return;
  }
  var html = "";
  data.incomeTemplates.forEach(function(item, i) {
    var recorded = md.recordedTemplates.includes(i);
    var btnHtml = recorded
      ? "<button class=\"btn btn-ghost\" disabled style=\"color:#9ca3af;cursor:not-allowed;\">✓ 入金済</button>"
      : "<button class=\"btn btn-success\" onclick=\"recordIncome(" + i + ")\">入金</button>";
    var nameVal = escapeHtml(item.name);
    var amtVal = escapeHtml(item.amount);
    html += "<div class=\"card\">";
    html += "<div class=\"card-row\">";
    html += "<input type=\"text\" class=\"input-name\" placeholder=\"収入名（例：給料）\" value=\"" + nameVal + "\" oninput=\"updateIncomeTemplate(" + i + ", &quot;name&quot;, this.value)\">";
    html += "</div>";
    html += "<div class=\"card-row\">";
    html += "<input type=\"text\" class=\"input-amount\" placeholder=\"金額\" value=\"" + (amtVal ? Number(amtVal).toLocaleString() : '') + "\" inputmode=\"numeric\" onfocus=\"unformatAmountInput(this)\" onblur=\"formatAmountInput(this);updateIncomeTemplate(" + i + ", &quot;amount&quot;, getAmountValue(this))\" oninput=\"updateIncomeTemplate(" + i + ", &quot;amount&quot;, getAmountValue(this))\">";
    html += btnHtml;
    html += "<button class=\"btn btn-ghost btn-icon\" onclick=\"deleteIncomeTemplate(" + i + ")\">🗑</button>";
    html += "</div></div>";
  });
  list.innerHTML = html;
}

function renderIncomeHistory() {
  const list = document.getElementById('incomeHistoryList');
  const history = getMonthData().history || [];
  if (history.length === 0) {
    list.innerHTML = `<div class="empty-state" style="padding:20px"><div style="font-size:13px">まだ入金記録はありません</div></div>`;
    return;
  }
  const reversed = [...history].map((h, i) => ({ ...h, idx: i })).reverse();
  list.innerHTML = reversed.map(h => `
    <div class="history-item">
      <div>
        <div>${escapeHtml(h.name)}</div>
        <div class="history-meta">${formatDate(h.date)}</div>
      </div>
      <div style="display:flex; align-items:center; gap:6px">
        <span class="history-amount">+${yen(h.amount)}円</span>
        <button class="history-delete" onclick="deleteHistoryItem(${h.idx})">×</button>
      </div>
    </div>
  `).join('');
}

function renderPayments() {
  const list = document.getElementById('paymentList');
  const payments = getMonthData().payments;
  if (payments.length === 0) {
    list.innerHTML = `
      <div class="empty-state">
        <div class="empty-icon">📋</div>
        <div>支払いを追加してください<br>(家賃、ローン、カードなど)</div>
      </div>
    `;
    return;
  }

  list.innerHTML = payments.map((item, i) => {
    const noteOpen = openNotes[i];
    const draggable = reorderMode ? 'draggable="true"' : '';
    const dragHandlers = reorderMode ? `
      ondragstart="onDragStart(event, ${i})"
      ondragend="onDragEnd(event)"
      ondragover="onDragOver(event, ${i})"
      ondrop="onDrop(event, ${i})"
    ` : '';

    return `
    <div class="card ${item.paid ? 'paid' : ''}" data-idx="${i}" ${draggable} ${dragHandlers}>
      <div class="card-row">
        ${reorderMode
          ? `<div class="drag-handle" ontouchstart="onTouchStart(event, ${i})" ontouchmove="onTouchMove(event)" ontouchend="onTouchEnd(event)">⋮⋮</div>`
          : `<div class="checkbox ${item.paid ? 'checked' : ''}" onclick="togglePaid(${i})"></div>`
        }
        <div class="priority-num">${i + 1}</div>
        <input type="text" class="input-name" placeholder="支払い名" value="${escapeHtml(item.name)}" oninput="updatePayment(${i}, 'name', this.value)" ${item.paid ? 'style="text-decoration:line-through;color:#9ca3af"' : ''} ${reorderMode ? 'disabled' : ''}>
      </div>
      <div class="card-row">
        <input type="text" class="input-amount" placeholder="金額" value="${item.amount ? Number(item.amount).toLocaleString() : ''}" inputmode="numeric" onfocus="unformatAmountInput(this)" onblur="formatAmountInput(this);updatePayment(${i}, 'amount', getAmountValue(this))" oninput="updatePayment(${i}, 'amount', getAmountValue(this))" ${reorderMode ? 'disabled' : ''}>
        <button class="note-toggle" onclick="toggleNote(${i})" style="flex:1;text-align:left;color:${item.note ? '#4f46e5' : '#9ca3af'}" ${reorderMode ? 'disabled' : ''}>
          ${item.note ? '📝 メモあり' : '＋ メモ追加'}
        </button>
        <button class="btn btn-ghost btn-icon" onclick="deletePayment(${i})" ${reorderMode ? 'disabled' : ''}>🗑</button>
      </div>
      <div class="note-area ${noteOpen ? 'show' : ''}">
        <textarea placeholder="メモ（引落日、カード会社など）" oninput="updatePayment(${i}, 'note', this.value)" ${reorderMode ? 'disabled' : ''}>${escapeHtml(item.note)}</textarea>

```
  </div>
</div>
```

`;
}).join(’’);
}

function renderAllocation() {
const md = getMonthData();
const totalIncome = md.history.reduce((s, h) => s + Number(h.amount || 0), 0);
let available = totalIncome;

const unpaidWithIdx = md.payments.map((p, i) => ({ …p, _idx: i })).filter(p => !p.paid);
const paidWithIdx = md.payments.map((p, i) => ({ …p, _idx: i })).filter(p => p.paid);

const paidTotal = paidWithIdx.reduce((s, p) => s + Number(p.amount || 0), 0);
available -= paidTotal;

let html = ‘’;

if (unpaidWithIdx.length === 0 && paidWithIdx.length === 0) {
html = `<div class="empty-state"> <div class="empty-icon">📊</div> <div>支払いを追加すると<br>自動で振り分け計算されます</div> </div>`;
} else {
unpaidWithIdx.forEach(p => {
const need = Number(p.amount || 0);
const allocated = Math.max(0, Math.min(available, need));
const shortage = need - allocated;
available -= allocated;

```
  const cardClass = shortage === 0 ? '' : (allocated === 0 ? 'shortage' : 'partial');
  const statusBadge = shortage === 0
    ? '<span class="status-badge status-ok">✓ 支払い可能</span>'
    : (allocated === 0
      ? '<span class="status-badge status-shortage">⚠ 全額不足</span>'
      : '<span class="status-badge status-shortage">⚠ 一部不足</span>');

  html += `
    <div class="allocation-card ${cardClass}">
      <div class="allocation-name">
        <span>${escapeHtml(p.name || '未入力')}</span>
        <span class="priority-badge">優先 ${p._idx + 1}</span>
      </div>
      <div class="allocation-detail">
        <span>必要額</span>
        <span>${yen(need)}円</span>
      </div>
      <div class="allocation-detail">
        <span>充当額</span>
        <span class="amount-positive">${yen(allocated)}円</span>
      </div>
      ${shortage > 0 ? `
        <div class="allocation-detail">
          <span>不足額</span>
          <span class="amount-negative">${yen(shortage)}円</span>
        </div>
      ` : ''}
      ${statusBadge}
      ${p.note ? `<div class="allocation-note">${escapeHtml(p.note)}</div>` : ''}
    </div>
  `;
});

if (paidWithIdx.length > 0) {
  html += `<div style="font-size:12px;color:#9ca3af;margin:16px 4px 8px">支払い済み</div>`;
  paidWithIdx.forEach(p => {
    html += `
      <div class="allocation-card paid-card">
        <div class="allocation-name">
          <span style="text-decoration:line-through">${escapeHtml(p.name || '未入力')}</span>
          <span class="priority-badge">優先 ${p._idx + 1}</span>
        </div>
        <div class="allocation-detail">
          <span>金額</span>
          <span>${yen(p.amount || 0)}円</span>
        </div>
        <span class="status-badge status-paid">✓ 支払い済み</span>
        ${p.note ? `<div class="allocation-note">${escapeHtml(p.note)}</div>` : ''}
      </div>
    `;
  });
}
```

}

document.getElementById(‘allocation’).innerHTML = html;
}

function renderArchive() {
const list = document.getElementById(‘archiveList’);
const monthKeys = Object.keys(data.months)
.filter(k => k !== data.currentMonth)
.filter(k => {
const m = data.months[k];
return (m.history && m.history.length > 0) || (m.payments && m.payments.length > 0);
})
.sort()
.reverse();

if (monthKeys.length === 0) {
list.innerHTML = `<div class="empty-state"><div class="empty-icon">📅</div><div>過去の記録はまだありません</div></div>`;
return;
}

list.innerHTML = monthKeys.map(key => {
const m = data.months[key];
const income = (m.history || []).reduce((s, h) => s + Number(h.amount || 0), 0);
const paymentTotal = (m.payments || []).reduce((s, p) => s + Number(p.amount || 0), 0);
const paidCount = (m.payments || []).filter(p => p.paid).length;
const totalCount = (m.payments || []).length;
const remain = income - paymentTotal;

```
return `
  <div class="archive-month" onclick="jumpToMonth('${key}')">
    <div class="archive-title">${formatMonthDisplay(key)}</div>
    <div class="archive-stat"><span>入金合計</span><b style="color:#059669">${yen(income)}円</b></div>
    <div class="archive-stat"><span>支払い合計</span><b style="color:#dc2626">${yen(paymentTotal)}円</b></div>
    <div class="archive-stat"><span>支払い完了</span><b>${paidCount} / ${totalCount} 件</b></div>
    <div class="archive-stat"><span>収支</span><b style="color:${remain >= 0 ? '#4f46e5' : '#dc2626'}">${remain >= 0 ? '+' : ''}${yen(remain)}円</b></div>
  </div>
`;
```

}).join(’’);
}

function jumpToMonth(key) {
data.currentMonth = key;
reorderMode = false;
openNotes = {};
save();
switchTab(‘income’);
render();
}

function calculate() {
const md = getMonthData();
const totalIncome = md.history.reduce((s, h) => s + Number(h.amount || 0), 0);
const totalPayment = md.payments.reduce((s, p) => s + Number(p.amount || 0), 0);
const paidPayment = md.payments.filter(p => p.paid).reduce((s, p) => s + Number(p.amount || 0), 0);
const unpaidPayment = totalPayment - paidPayment;
const remain = totalIncome - paidPayment;

document.getElementById(‘monthIncome’).innerText = yen(totalIncome);
document.getElementById(‘paymentTotal’).innerText = yen(unpaidPayment);
document.getElementById(‘remain’).innerText = yen(remain);

// 支払い済み金額の表示更新
const paidEl = document.getElementById(‘paidPaymentRow’);
if (paidEl) {
if (paidPayment > 0) {
paidEl.style.display = ‘flex’;
document.getElementById(‘paidPaymentAmt’).innerText = yen(paidPayment);
} else {
paidEl.style.display = ‘none’;
}
}

const coverRate = unpaidPayment > 0 ? Math.min(100, (totalIncome / unpaidPayment) * 100) : 100;
const bar = document.getElementById(‘progressBar’);
bar.style.width = coverRate + ‘%’;
bar.classList.remove(‘warning’, ‘danger’);
if (coverRate < 50) bar.classList.add(‘danger’);
else if (coverRate < 100) bar.classList.add(‘warning’);

document.getElementById(‘progressText’).innerText = ’支払いカバー率 ’ + Math.round(coverRate) + ‘%’;

const remainEl = document.getElementById(‘remain’).parentElement;
remainEl.style.color = remain >= 0 ? ‘#4f46e5’ : ‘#dc2626’;
}

function exportData() {
try {
const json = JSON.stringify(data, null, 2);
const blob = new Blob([json], { type: ‘application/json’ });
const url = URL.createObjectURL(blob);
const a = document.createElement(‘a’);
const today = new Date();
const dateStr = `${today.getFullYear()}${String(today.getMonth() + 1).padStart(2, '0')}${String(today.getDate()).padStart(2, '0')}`;
a.href = url;
a.download = `家計やりくり_バックアップ_${dateStr}.json`;
document.body.appendChild(a);
a.click();
document.body.removeChild(a);
URL.revokeObjectURL(url);
showToast(‘エクスポートしました’);
closeMenu();
} catch (e) {
showToast(‘エクスポート失敗：’ + e.message);
}
}

function importData(event) {
const file = event.target.files[0];
if (!file) return;
const reader = new FileReader();
reader.onload = (e) => {
try {
const imported = JSON.parse(e.target.result);
if (!imported.months || typeof imported.months !== ‘object’) {
throw new Error(‘ファイル形式が正しくありません’);
}
showModal(
‘インポート確認’,
‘現在のデータを上書きしてインポートします。よろしいですか？\n（先に「エクスポート」で現在のデータをバックアップすることをおすすめします）’,
() => {
data = imported;
if (!data.currentMonth) data.currentMonth = getCurrentMonthKey();
if (!data.incomeTemplates) data.incomeTemplates = [];
save();
render();
closeMenu();
showToast(‘インポートしました’);
}
);
} catch (err) {
showToast(‘インポート失敗：’ + err.message);
}
};
reader.readAsText(file);
event.target.value = ‘’;
}

function deleteAllData() {
showModal(
‘全削除確認’,
‘本当にすべてのデータを削除しますか？\nこの操作は取り消せません。\n先にエクスポートでバックアップを取ることを強くおすすめします。’,
() => {
localStorage.removeItem(‘budgetAppData_v3’);
localStorage.removeItem(‘budgetAppData_v2’);
localStorage.removeItem(‘repaymentAppData’);
data = {
currentMonth: getCurrentMonthKey(),
incomeTemplates: [],
months: { [getCurrentMonthKey()]: { payments: [], history: [] } }
};
save();
render();
closeMenu();
showToast(‘すべて削除しました’);
}
);
}

load();
render();
</script>

</body>
</html>
