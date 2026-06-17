<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-title" content="NF 충청점 KID">
<title>THE NORTH FACE · 현대백화점 충청점 KID</title>
<style>
*{box-sizing:border-box;margin:0;padding:0;-webkit-tap-highlight-color:transparent}
:root{
  --bg:#fff;--bg2:#f7f7f5;--bg3:#f0efeb;
  --text:#1a1a1a;--text2:#666;--text3:#999;
  --border:rgba(0,0,0,0.1);--border2:rgba(0,0,0,0.18);
  --red:#c62828;--redbg:rgba(198,40,40,0.08);
  --blue:#1565c0;--bluebg:rgba(21,101,192,0.08);
  --green:#2e7d32;--greenbg:rgba(46,125,50,0.08);
  --purple:#6a1b9a;--purplebg:rgba(106,27,154,0.08);
  --orange:#e65100;--orangebg:rgba(230,81,0,0.08);
  --radius:12px;--radius-sm:8px;
}
@media(prefers-color-scheme:dark){:root{
  --bg:#1c1c1e;--bg2:#2c2c2e;--bg3:#3a3a3c;
  --text:#f2f2f7;--text2:#aeaeb2;--text3:#636366;
  --border:rgba(255,255,255,0.1);--border2:rgba(255,255,255,0.18);
  --redbg:rgba(198,40,40,0.15);--bluebg:rgba(21,101,192,0.15);
  --greenbg:rgba(46,125,50,0.15);--purplebg:rgba(106,27,154,0.15);--orangebg:rgba(230,81,0,0.15);
}}
body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',sans-serif;background:var(--bg3);color:var(--text);min-height:100vh}
.app{max-width:960px;margin:0 auto;padding:12px}
.hdr{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius);padding:12px 18px;margin-bottom:10px;display:flex;align-items:center;justify-content:space-between}
.logo{font-size:13px;font-weight:600;letter-spacing:2.5px}
.store-nm{font-size:11px;color:var(--text2);margin-top:2px}
.sync-dot{width:8px;height:8px;border-radius:50%;background:#ccc}
.sync-dot.ok{background:#4caf50}.sync-dot.err{background:#f44336}
.tabs{display:flex;gap:5px;margin-bottom:10px;overflow-x:auto;padding-bottom:2px;scrollbar-width:none}
.tabs::-webkit-scrollbar{display:none}
.tab{padding:7px 14px;border-radius:20px;font-size:12px;font-weight:500;cursor:pointer;border:0.5px solid var(--border);background:var(--bg);color:var(--text2);transition:all .15s;white-space:nowrap;flex-shrink:0}
.tab.active{background:var(--text);color:var(--bg);border-color:var(--text)}
.panel{display:none}.panel.active{display:block}
.card{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius);padding:14px;margin-bottom:10px}
input,select,textarea{width:100%;padding:8px 10px;border:0.5px solid var(--border2);border-radius:var(--radius-sm);font-size:12px;background:var(--bg);color:var(--text);outline:none;font-family:inherit;-webkit-appearance:none}
input:focus,select:focus{border-color:var(--text)}
.btn{padding:8px 14px;border-radius:var(--radius-sm);border:0.5px solid var(--border2);background:var(--bg2);font-size:12px;font-weight:500;cursor:pointer;color:var(--text);font-family:inherit;white-space:nowrap;transition:all .12s}
.btn:hover{background:var(--bg3)}
.btn-dark{background:var(--text);color:var(--bg);border-color:var(--text)}.btn-dark:hover{opacity:.85}
.btn-sm{padding:4px 10px;font-size:11px}
.btn-danger{color:var(--red);border-color:rgba(198,40,40,.25);background:var(--redbg)}
.offline-bar{background:var(--redbg);color:var(--red);text-align:center;font-size:11px;padding:6px;border-radius:8px;margin-bottom:10px;display:none}
.offline-bar.show{display:block}

/* DATE NAV */
.date-nav{display:flex;align-items:center;gap:10px;margin-bottom:12px}
.date-lbl{flex:1;font-size:15px;font-weight:600}
.date-sub{font-size:11px;color:var(--text3);margin-top:1px}
.nav-btn{background:none;border:0.5px solid var(--border2);border-radius:6px;width:28px;height:28px;cursor:pointer;font-size:14px;color:var(--text);display:flex;align-items:center;justify-content:center}
.today-btn{font-size:11px;padding:3px 9px;border-radius:10px;border:0.5px solid var(--border2);background:var(--bg2);cursor:pointer;color:var(--text2)}

/* TASKS */
.task-section{background:var(--bg);border:0.5px solid var(--border);border-radius:var(--radius);padding:13px;margin-bottom:10px}
.task-sec-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:10px}
.task-sec-name{font-size:13px;font-weight:600}
.task-prog{font-size:10px;color:var(--text3);background:var(--bg2);padding:2px 8px;border-radius:10px}
.task-item{display:flex;align-items:flex-start;gap:9px;padding:8px 0;border-bottom:0.5px solid var(--border)}
.task-item:last-of-type{border-bottom:none}
.chk{width:19px;height:19px;border-radius:50%;border:1.5px solid var(--border2);background:none;cursor:pointer;flex-shrink:0;margin-top:1px;display:flex;align-items:center;justify-content:center;position:relative;transition:all .15s}
.chk.done{background:var(--text);border-color:var(--text)}
.chk.done::after{content:'';position:absolute;width:4px;height:8px;border:2px solid var(--bg);border-top:none;border-left:none;transform:rotate(45deg) translate(-1px,-1px)}
.task-body{flex:1;min-width:0}
.task-txt{font-size:13px;line-height:1.4}
.task-txt.done{text-decoration:line-through;color:var(--text3)}
.task-meta{display:flex;align-items:center;gap:5px;margin-top:3px;flex-wrap:wrap}
.bdg{font-size:10px;padding:1px 6px;border-radius:4px;font-weight:500}
.bdg-time{background:var(--bg2);color:var(--text2)}
.bdg-overdue{background:var(--redbg);color:var(--red)}
.bdg-carry{background:var(--orangebg);color:var(--orange)}
.bdg-in{background:var(--bluebg);color:var(--blue)}
.bdg-out{background:var(--purplebg);color:var(--purple)}
.bdg-pickup{background:var(--greenbg);color:var(--green)}
.task-del{background:none;border:none;color:var(--text3);cursor:pointer;font-size:13px;padding:2px;flex-shrink:0}
.task-del:hover{color:var(--red)}
.task-add-row{display:flex;gap:5px;margin-top:9px}
.task-add-row input{flex:1;margin:0}
.task-add-row button{flex-shrink:0}

/* CALENDAR */
.cal-layout{display:grid;grid-template-columns:1fr 260px;gap:10px}
@media(max-width:600px){.cal-layout{grid-template-columns:1fr}}
.cal-nav{display:flex;align-items:center;justify-content:space-between;margin-bottom:10px}
.cal-mon{font-size:15px;font-weight:600}
.cal-dow-row{display:grid;grid-template-columns:repeat(7,1fr);margin-bottom:3px}
.cal-dow{text-align:center;font-size:10px;color:var(--text3);padding:3px 0}
.cal-grid{display:grid;grid-template-columns:repeat(7,1fr);gap:2px}
.cal-cell{min-height:60px;border-radius:6px;padding:4px;cursor:pointer;border:0.5px solid transparent;transition:background .1s}
.cal-cell:hover{background:var(--bg2)}.cal-cell.today{border-color:var(--text)}
.cal-cell.other{opacity:.3}.cal-cell.off-day{background:var(--redbg)}
.cell-num{font-size:11px;font-weight:600;margin-bottom:2px;width:17px;height:17px;display:flex;align-items:center;justify-content:center;border-radius:50%}
.cal-cell.today .cell-num{background:var(--text);color:var(--bg)}
.ev-pill{font-size:9px;border-radius:3px;padding:1px 3px;margin-bottom:1px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;line-height:1.4;border-left:2px solid}
.off-pill{font-size:9px;background:var(--redbg);color:var(--red);border-radius:3px;padding:1px 3px;margin-bottom:1px}
.leg-row{display:flex;gap:8px;flex-wrap:wrap;margin-top:8px}
.leg{display:flex;align-items:center;gap:3px;font-size:10px;color:var(--text2)}
.leg-dot{width:7px;height:7px;border-radius:2px}
.ev-item{display:flex;align-items:flex-start;gap:7px;padding:7px;border-radius:8px;margin-bottom:4px;background:var(--bg2);font-size:12px}
.ev-dot{width:7px;height:7px;border-radius:50%;margin-top:3px;flex-shrink:0}
.ev-body{flex:1;min-width:0}
.ev-ttl{font-weight:500;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
.ev-dt{font-size:10px;color:var(--text2);margin-top:1px}
.ev-del{background:none;border:none;color:var(--text3);cursor:pointer;font-size:12px}

/* OFF */
.stat-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin-bottom:10px}
.stat-box{background:var(--bg2);border-radius:10px;padding:10px;text-align:center}
.stat-num{font-size:20px;font-weight:600}
.stat-lbl{font-size:10px;color:var(--text3);margin-top:1px}
.tag{display:inline-flex;align-items:center;gap:3px;padding:3px 10px;border-radius:12px;font-size:11px;margin:2px;font-weight:500}
.staff-card{background:var(--bg);border:0.5px solid var(--border);border-radius:10px;padding:12px;margin-bottom:8px}
.staff-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:8px;gap:8px}
.staff-nm{font-size:13px;font-weight:600}
.staff-role{font-size:10px;color:var(--text3)}
.edit-btn{background:none;border:none;cursor:pointer;font-size:11px;color:var(--text3);padding:0 2px}
.edit-btn:hover{color:var(--text)}
.nm-inp{border:none;border-bottom:1.5px solid var(--text);background:transparent;font-size:13px;font-weight:600;color:var(--text);outline:none;width:80px;padding:1px 2px}
.off-chip{display:inline-flex;align-items:center;gap:3px;background:var(--bg2);border-radius:10px;padding:3px 8px;font-size:11px;margin:2px}
.off-chip-del{background:none;border:none;cursor:pointer;color:var(--text3);font-size:11px;line-height:1;padding:0}
.off-chip-del:hover{color:var(--red)}
.add-off-row{display:flex;gap:5px;margin-top:8px}
.add-off-row input{flex:1;margin:0}

/* INVENTORY */
.inv-search-wrap{position:relative;margin-bottom:10px}
.inv-search-wrap input{padding-left:34px;margin:0}
.inv-s-icon{position:absolute;left:10px;top:50%;transform:translateY(-50%);font-size:13px;pointer-events:none}
.inv-tabs{display:flex;gap:5px;margin-bottom:10px;flex-wrap:wrap}
.inv-tab{padding:5px 14px;border-radius:14px;font-size:11px;font-weight:500;cursor:pointer;border:0.5px solid var(--border);background:var(--bg);color:var(--text2);transition:all .15s}
.inv-tab.active{background:var(--text);color:var(--bg);border-color:var(--text)}
.tbl-wrap{overflow-x:auto;border-radius:10px;border:0.5px solid var(--border)}
.tbl{width:100%;border-collapse:collapse;font-size:12px}
.tbl th{background:var(--bg2);padding:7px 10px;text-align:left;font-weight:600;font-size:11px;color:var(--text2);border-bottom:0.5px solid var(--border);white-space:nowrap}
.tbl td{padding:6px 10px;border-bottom:0.5px solid var(--border);color:var(--text);white-space:nowrap}
.tbl tr:last-child td{border-bottom:none}
.tbl tr:hover td{background:var(--bg2)}
.hl{background:rgba(255,200,0,.32);border-radius:2px;padding:0 1px}
.qty-ok{color:var(--green);font-weight:500}
.qty-low{color:var(--orange);font-weight:500}
.qty-zero{color:var(--red);font-weight:500}
.reload-btn{padding:4px 10px;border-radius:7px;border:0.5px solid var(--border2);background:var(--bg2);font-size:11px;cursor:pointer;color:var(--text2)}
.reload-btn:hover{background:var(--text);color:var(--bg)}

/* MOVEMENT */
.mv-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:10px;flex-wrap:wrap;gap:8px}
.mv-filter-row{display:flex;gap:5px;flex-wrap:wrap;margin-bottom:10px}
.mv-filter{padding:4px 12px;border-radius:12px;font-size:11px;font-weight:500;cursor:pointer;border:0.5px solid var(--border);background:var(--bg);color:var(--text2);transition:all .12s}
.mv-filter.active{background:var(--text);color:var(--bg);border-color:var(--text)}
.mv-add-form{background:var(--bg2);border-radius:10px;padding:12px;margin-bottom:10px}
.mv-add-form-title{font-size:12px;font-weight:600;margin-bottom:8px;color:var(--text2)}
.mv-grid{display:grid;gap:6px;margin-bottom:8px}
.mv-grid-2{grid-template-columns:1fr 1fr}
.mv-grid-3{grid-template-columns:1fr 1fr 1fr}
.mv-grid-4{grid-template-columns:1fr 1fr 1fr 1fr}
.mv-grid input,.mv-grid select{margin:0}
.mv-row{display:flex;align-items:flex-start;gap:8px;padding:8px 0;border-bottom:0.5px solid var(--border)}
.mv-row:last-child{border-bottom:none}
.mv-row.carry{background:rgba(230,81,0,.04);border-radius:6px;padding:8px;margin-bottom:2px;border:0.5px solid rgba(230,81,0,.15)}
.mv-chk{width:19px;height:19px;border-radius:4px;border:1.5px solid var(--border2);background:none;cursor:pointer;flex-shrink:0;margin-top:1px;display:flex;align-items:center;justify-content:center;position:relative;transition:all .15s}
.mv-chk.done{background:var(--green);border-color:var(--green)}
.mv-chk.done::after{content:'✓';color:#fff;font-size:11px;font-weight:700}
.mv-body{flex:1;min-width:0}
.mv-main{display:flex;align-items:center;gap:6px;flex-wrap:wrap}
.mv-chip{font-size:11px;background:var(--bg2);padding:1px 7px;border-radius:6px;color:var(--text2);white-space:nowrap}
.mv-pno{font-size:13px;font-weight:600;color:var(--text)}
.mv-meta{display:flex;align-items:center;gap:5px;margin-top:3px;flex-wrap:wrap}
.mv-del{background:none;border:none;color:var(--text3);cursor:pointer;font-size:13px;padding:2px;flex-shrink:0}
.mv-del:hover{color:var(--red)}
.mv-carry-lbl{font-size:10px;color:var(--orange);font-weight:500}
.mv-done-time{font-size:10px;color:var(--text3)}
.type-chip{font-size:10px;padding:1px 6px;border-radius:5px;font-weight:500}
.type-자동{background:var(--bluebg);color:var(--blue)}
.type-권고{background:var(--purplebg);color:var(--purple)}
.type-요청{background:var(--greenbg);color:var(--green)}
.type-교환{background:var(--orangebg);color:var(--orange)}
.type-주문{background:var(--redbg);color:var(--red)}
.type-NCP몰{background:rgba(0,150,136,.1);color:#00695c}
.type-네이버몰{background:rgba(27,94,32,.1);color:#1b5e20}
.mv-section-empty{font-size:11px;color:var(--text3);padding:10px 0}
.mv-chks{display:flex;flex-direction:column;gap:4px;flex-shrink:0;margin-top:1px}
.mv-chk-wrap{display:flex;align-items:center;gap:3px}
.mv-chk-lbl{font-size:9px;color:var(--text3);white-space:nowrap}
.mv-chk{width:17px;height:17px;border-radius:3px;border:1.5px solid var(--border2);background:none;cursor:pointer;flex-shrink:0;display:flex;align-items:center;justify-content:center;position:relative;transition:all .15s}
.mv-chk.done{background:var(--green);border-color:var(--green)}
.mv-chk.done::after{content:'✓';color:#fff;font-size:10px;font-weight:700;line-height:1}
.mv-chk.disabled{background:var(--text);border-color:var(--text);cursor:default}
.mv-chk.all-done{background:var(--green);border-color:var(--green)}
</style>
</head>
<body>
<div class="app">
  <div class="offline-bar" id="offline-bar">오프라인 — 인터넷 연결 확인</div>
  <div class="hdr">
    <div><div class="logo">THE NORTH FACE</div><div class="store-nm">현대백화점 충청점 · KID</div></div>
    <div style="display:flex;align-items:center;gap:7px">
      <span style="font-size:10px;color:var(--text3)" id="sync-lbl">연결 중...</span>
      <div class="sync-dot" id="sync-dot"></div>
    </div>
  </div>
  <div class="tabs">
    <div class="tab active" onclick="sw('tasks')">당일과제</div>
    <div class="tab" onclick="sw('in')">이동입고</div>
    <div class="tab" onclick="sw('out')">이동출고</div>
    <div class="tab" onclick="sw('pickup')">제품픽업</div>
    <div class="tab" onclick="sw('calendar')">할일 캘린더</div>
    <div class="tab" onclick="sw('off')">휴무 관리</div>
    <div class="tab" onclick="sw('inventory')">재고 관리</div>
  </div>

  <!-- 당일과제 -->
  <div id="panel-tasks" class="panel active">
    <div class="date-nav">
      <button class="nav-btn" onclick="chDay('task',-1)">‹</button>
      <div style="flex:1"><div class="date-lbl" id="task-lbl"></div><div class="date-sub" id="task-sub"></div></div>
      <button class="today-btn" onclick="goToday('task')">오늘</button>
      <button class="nav-btn" onclick="chDay('task',1)">›</button>
    </div>
    <div id="task-sections"><div style="text-align:center;padding:30px;color:var(--text3)">불러오는 중...</div></div>
  </div>

  <!-- 이동입고 -->
  <div id="panel-in" class="panel">
    <div class="date-nav">
      <button class="nav-btn" onclick="chDay('in',-1)">‹</button>
      <div style="flex:1"><div class="date-lbl" id="in-lbl"></div><div class="date-sub" id="in-sub"></div></div>
      <button class="today-btn" onclick="goToday('in')">오늘</button>
      <button class="nav-btn" onclick="chDay('in',1)">›</button>
    </div>
    <div class="mv-filter-row" id="in-filter-row"></div>
    <div class="mv-add-form">
      <div class="mv-add-form-title">+ 이동입고 등록</div>
      <div class="mv-grid mv-grid-4" style="margin-bottom:6px">
        <input type="text" id="in-pno" placeholder="품번">
        <input type="text" id="in-size" placeholder="사이즈">
        <input type="number" id="in-qty" placeholder="개수" min="1">
        <select id="in-type"><option value="">종류 선택</option><option>주문</option><option>물</option><option>단체</option><option>권고</option><option>자동</option></select>
      </div>
      <div style="margin-bottom:8px">
        <input type="text" id="in-note" placeholder="메모(선택)" style="margin:0">
      </div>
      <button class="btn btn-dark" onclick="addMv('in')">등록</button>
    </div>
    <div id="in-list"></div>
  </div>

  <!-- 이동출고 -->
  <div id="panel-out" class="panel">
    <div class="date-nav">
      <button class="nav-btn" onclick="chDay('out',-1)">‹</button>
      <div style="flex:1"><div class="date-lbl" id="out-lbl"></div><div class="date-sub" id="out-sub"></div></div>
      <button class="today-btn" onclick="goToday('out')">오늘</button>
      <button class="nav-btn" onclick="chDay('out',1)">›</button>
    </div>
    <div class="mv-filter-row" id="out-filter-row"></div>
    <div class="mv-add-form">
      <div class="mv-add-form-title">+ 이동출고 등록</div>
      <div class="mv-grid mv-grid-4" style="margin-bottom:6px">
        <input type="text" id="out-pno" placeholder="품번">
        <input type="text" id="out-size" placeholder="사이즈">
        <input type="number" id="out-qty" placeholder="개수" min="1">
        <select id="out-type"><option value="">종류 선택</option><option>자동</option><option>권고</option><option>요청</option><option>교환</option></select>
      </div>
      <div class="mv-grid mv-grid-3" style="margin-bottom:8px">
        <input type="text" id="out-dong" placeholder="출고매장" style="margin:0">
        <input type="text" id="out-waybill" placeholder="운송장번호(동진및택배)" style="margin:0">
        <select id="out-send" style="margin:0"><option value="">동진or택배</option><option>동진</option><option>택배</option></select>
      </div>
      <button class="btn btn-dark" onclick="addMv('out')">등록</button>
    </div>
    <div id="out-list"></div>
  </div>

  <!-- 제품픽업 -->
  <div id="panel-pickup" class="panel">
    <div class="date-nav">
      <button class="nav-btn" onclick="chDay('pickup',-1)">‹</button>
      <div style="flex:1"><div class="date-lbl" id="pickup-lbl"></div><div class="date-sub" id="pickup-sub"></div></div>
      <button class="today-btn" onclick="goToday('pickup')">오늘</button>
      <button class="nav-btn" onclick="chDay('pickup',1)">›</button>
    </div>
    <div class="mv-filter-row" id="pickup-filter-row"></div>
    <div class="mv-add-form">
      <div class="mv-add-form-title">+ 제품픽업 등록</div>
      <div class="mv-grid mv-grid-4" style="margin-bottom:6px">
        <input type="text" id="pickup-pno" placeholder="품번">
        <input type="text" id="pickup-size" placeholder="사이즈">
        <input type="number" id="pickup-qty" placeholder="개수" min="1">
        <select id="pickup-type"><option value="">종류 선택</option><option>NCP몰</option><option>네이버몰</option><option>자동</option><option>권고</option><option>요청</option><option>교환</option><option>주문</option></select>
      </div>
      <div class="mv-grid mv-grid-2" style="margin-bottom:8px">
        <input type="text" id="pickup-loc" placeholder="창고위치">
        <input type="text" id="pickup-note" placeholder="메모(선택)">
      </div>
      <button class="btn btn-dark" onclick="addMv('pickup')">등록</button>
    </div>
    <div id="pickup-list"></div>
  </div>

  <!-- 할일 캘린더 -->
  <div id="panel-calendar" class="panel">
    <div class="cal-layout">
      <div class="card" style="margin-bottom:0">
        <div class="cal-nav">
          <button class="nav-btn" onclick="chMon(-1)">‹</button>
          <div class="cal-mon" id="cal-mon-lbl"></div>
          <button class="nav-btn" onclick="chMon(1)">›</button>
        </div>
        <div class="cal-dow-row">
          <div class="cal-dow">일</div><div class="cal-dow">월</div><div class="cal-dow">화</div>
          <div class="cal-dow">수</div><div class="cal-dow">목</div><div class="cal-dow">금</div><div class="cal-dow">토</div>
        </div>
        <div class="cal-grid" id="cal-grid"></div>
        <div class="leg-row" id="cal-legend"></div>
      </div>
      <div>
        <div class="card" style="margin-bottom:10px">
          <div style="font-size:11px;font-weight:600;color:var(--text3);margin-bottom:8px">일정 추가</div>
          <input type="text" id="ev-title" placeholder="일정 내용" style="margin-bottom:6px">
          <input type="date" id="ev-date" style="margin-bottom:6px">
          <select id="ev-type" style="margin-bottom:8px">
            <option value="store">매장 일정</option><option value="task">업무</option><option value="meet">미팅</option>
            <option value="stock">재고</option><option value="clean">청소/정리</option><option value="etc">기타</option>
          </select>
          <button class="btn btn-dark" style="width:100%" onclick="addEvent()">추가하기</button>
        </div>
        <div class="card" style="margin-bottom:0">
          <div style="font-size:11px;font-weight:600;color:var(--text3);margin-bottom:8px">이번 달 일정</div>
          <div id="ev-list" style="max-height:280px;overflow-y:auto"></div>
        </div>
      </div>
    </div>
  </div>

  <!-- 휴무 관리 -->
  <div id="panel-off" class="panel">
    <div class="stat-grid" id="off-stats"></div>
    <div id="today-off-box" style="background:var(--bg);border:0.5px solid var(--border);border-radius:10px;padding:10px;margin-bottom:10px"></div>
    <div id="staff-list"></div>
    <div class="card">
      <div style="font-size:11px;font-weight:600;color:var(--text3);margin-bottom:8px">직원 추가</div>
      <div style="display:flex;gap:5px;flex-wrap:wrap">
        <select id="new-role" style="flex:1;min-width:90px;margin:0"><option value="점장">점장</option><option value="시니어">시니어</option><option value="주니어">주니어</option><option value="파트">파트타임</option></select>
        <input type="text" id="new-name" placeholder="이름" style="flex:1;min-width:70px;margin:0">
        <button class="btn" onclick="addStaff()">추가</button>
      </div>
    </div>
  </div>

  <!-- 재고 관리 -->
  <div id="panel-inventory" class="panel">
    <div class="inv-search-wrap">
      <span class="inv-s-icon">🔍</span>
      <input type="text" id="inv-search" placeholder="전체 창고 검색 — 품번, 컬러, 사이즈..." oninput="searchInv()">
    </div>
    <div id="inv-search-results"></div>
    <div class="inv-tabs" id="inv-tabs"></div>
    <div id="inv-panel"></div>
  </div>
</div>

<script type="module">
/* ════════════════════════════════════════════════
   Firebase — chungcheong-kid 프로젝트 (KID 전용)
   ════════════════════════════════════════════════ */
import{initializeApp}from"https://www.gstatic.com/firebasejs/10.12.0/firebase-app.js";
import{getFirestore,doc,getDoc,setDoc,onSnapshot}from"https://www.gstatic.com/firebasejs/10.12.0/firebase-firestore.js";

const FB={
  apiKey:"AIzaSyA3SIpzoWYg4eRwXNWE2Z7hvN67DEO61IA",
  authDomain:"chungcheong-kid.firebaseapp.com",
  projectId:"chungcheong-kid",
  storageBucket:"chungcheong-kid.firebasestorage.app",
  messagingSenderId:"163383940846",
  appId:"1:163383940846:web:be6989f91bdc65e90e05ff"
};
const db=getFirestore(initializeApp(FB));

/* ════ 구글 시트 ID (KID용으로 교체하세요) ════ */
const SHEET_ID='1V6R9vc1oIaiJH61oK-t0bdOVCSSTNADDELd_SVQtCsk';

const SHEETS=[{name:'매장재고',label:'매장'},{name:'지2창고',label:'지하2층'},{name:'지3창고',label:'지하3층'},{name:'지4창고',label:'지하4층'},{name:'외부창고',label:'외부창고'}];
const RC={점장:'#1565c0',시니어:'#6a1b9a',주니어:'#2e7d32',파트:'#e65100'};
const EC={store:'#c62828',task:'#1565c0',meet:'#7b1fa2',stock:'#2e7d32',clean:'#e65100',etc:'#5d4037'};
const EL={store:'매장',task:'업무',meet:'미팅',stock:'재고',clean:'청소',etc:'기타'};
const IN_TYPES=['주문','물','단체','권고','자동'];
const OUT_TYPES=['자동','권고','요청','교환'];
const PICKUP_TYPES=['NCP몰','네이버몰','자동','권고','요청','교환','주문'];

const today=new Date();
const todayStr=fmt(today);
let calY=today.getFullYear(),calM=today.getMonth();
let offY=today.getFullYear(),offM=today.getMonth();
let curInvSheet=0;

const dates={task:new Date(today),in:new Date(today),out:new Date(today),pickup:new Date(today)};
const filters={in:'전체',out:'전체',pickup:'전체'};

let DB={staff:[],off:{},events:[],tasks:{},mv_in:{},mv_out:{},mv_pickup:{}};
let INV={};
let savingMain=false;

function fmt(d){return d.getFullYear()+'-'+p2(d.getMonth()+1)+'-'+p2(d.getDate())}
function p2(n){return String(n).padStart(2,'0')}
function dow(s){return['일','월','화','수','목','금','토'][new Date(s+'T00:00:00').getDay()]}
function esc(s){return String(s||'').replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;').replace(/"/g,'&quot;')}
function dnStr(d){const dn=['일','월','화','수','목','금','토'];return d.getFullYear()+'년 '+(d.getMonth()+1)+'월 '+d.getDate()+'일 ('+dn[d.getDay()]+')';}

const mainRef=doc(db,'store','main');
async function loadMain(){
  try{const s=await getDoc(mainRef);if(s.exists()){const d=s.data();DB={staff:d.staff||defS(),off:d.off||{},events:d.events||[],tasks:d.tasks||{},mv_in:d.mv_in||{},mv_out:d.mv_out||{},mv_pickup:d.mv_pickup||{}};}else{DB.staff=defS();await saveMain();}setSyncOk();renderAll();}
  catch(e){setSyncErr();try{const d=JSON.parse(localStorage.getItem('nf_kid_main')||'null');if(d)DB=d;else DB.staff=defS();}catch(e2){DB.staff=defS();}renderAll();}
}
async function saveMain(){
  if(savingMain)return;savingMain=true;
  try{await setDoc(mainRef,DB);try{localStorage.setItem('nf_kid_main',JSON.stringify(DB))}catch(e){}setSyncOk();}
  catch(e){setSyncErr();try{localStorage.setItem('nf_kid_main',JSON.stringify(DB))}catch(e2){}}
  savingMain=false;
}
onSnapshot(mainRef,(s)=>{if(s.exists()&&!savingMain){const d=s.data();DB={staff:d.staff||DB.staff,off:d.off||{},events:d.events||[],tasks:d.tasks||{},mv_in:d.mv_in||{},mv_out:d.mv_out||{},mv_pickup:d.mv_pickup||{}};setSyncOk();renderAll();}},()=>setSyncErr());

function defS(){return[{id:'s1',role:'점장',name:'점장'},{id:'s2',role:'시니어',name:'시니어'},{id:'s3',role:'주니어',name:'주니어'}];}
function setSyncOk(){document.getElementById('sync-dot').className='sync-dot ok';document.getElementById('sync-lbl').textContent='실시간 연결됨';document.getElementById('offline-bar').classList.remove('show');}
function setSyncErr(){document.getElementById('sync-dot').className='sync-dot err';document.getElementById('sync-lbl').textContent='오프라인';document.getElementById('offline-bar').classList.add('show');}
function renderAll(){renderTasks();['in','out','pickup'].forEach(t=>{if(document.getElementById('panel-'+t).classList.contains('active'))renderMv(t);});if(document.getElementById('panel-calendar').classList.contains('active'))renderCal();if(document.getElementById('panel-off').classList.contains('active'))renderOff();}

window.sw=function(id){
  document.querySelectorAll('.tab').forEach((t,i)=>t.classList.toggle('active',['tasks','in','out','pickup','calendar','off','inventory'][i]===id));
  document.querySelectorAll('.panel').forEach(p=>p.classList.remove('active'));
  document.getElementById('panel-'+id).classList.add('active');
  if(id==='calendar')renderCal();else if(id==='off')renderOff();else if(id==='inventory')renderInvPanel();else if(['tasks','in','out','pickup'].includes(id))renderMv(id);
};

window.chDay=function(type,d){dates[type].setDate(dates[type].getDate()+d);renderMv(type);}
window.goToday=function(type){dates[type]=new Date(today);renderMv(type);}

function renderMv(type){
  if(type==='task'||type==='tasks'){renderTasks();return;}
  updateDateNav(type);
  if(type==='in')renderIn();
  else if(type==='out')renderOut();
  else if(type==='pickup')renderPickup();
}
function updateDateNav(type){
  const d=dates[type];const ds=fmt(d);const isToday=ds===todayStr;const isPast=ds<todayStr;
  document.getElementById(type+'-lbl').textContent=dnStr(d);
  document.getElementById(type+'-sub').textContent=isToday?'오늘':isPast?'지난 날':'미래';
}

function renderTasks(){
  const d=dates.task||(dates.task=new Date(today));
  const ds=fmt(d);const isToday=ds===todayStr;const isPast=ds<todayStr;
  document.getElementById('task-lbl').textContent=dnStr(d);
  document.getElementById('task-sub').textContent=isToday?'오늘':isPast?'지난 날':'미래';
  if(!DB.tasks[ds])DB.tasks[ds]={store:[],staff:{}};
  const prev=DB.tasks[fmt(new Date(new Date(ds+'T00:00:00').getTime()-86400000))];
  const uncheckedItems=[];
  ['mv_in','mv_out','mv_pickup'].forEach(mvKey=>{
    const mvData=DB[mvKey]||{};
    const label=mvKey==='mv_in'?'이동입고':mvKey==='mv_out'?'이동출고':'제품픽업';
    const color=mvKey==='mv_in'?'bdg-in':mvKey==='mv_out'?'bdg-out':'bdg-pickup';
    const checkDates=[];
    checkDates.push(todayStr);
    if(mvKey==='mv_in'){Object.keys(mvData).sort().forEach(d=>{if(d<todayStr)checkDates.push(d);});}
    else{for(let d=1;d<=3;d++){checkDates.push(fmt(new Date(new Date(todayStr+'T00:00:00').getTime()-d*86400000)));}}
    checkDates.forEach(checkDs=>{
      const items=(mvData[checkDs]||[]).filter(i=>{
        if(mvKey==='mv_out'){const noJ=['자동','권고'].includes(i.type||'');return !(i.chkDong&&(i.chkJeonsan||noJ));}
        if(mvKey==='mv_in') return !(i.checked||(i.store&&i.duedate&&i.indate));
        return !i.checked;
      });
      items.forEach(i=>{
        const isCarry=checkDs!==todayStr;
        uncheckedItems.push({label,color,text:i.pno+(i.size?' ('+i.size+')':'')+(i.qty?' x'+i.qty:''),type:i.type||'',isCarry,ds:checkDs});
      });
    });
  });
  let html='';
  if(isToday&&uncheckedItems.length>0){
    html+=`<div class="task-section" style="border-color:rgba(21,101,192,.2)"><div class="task-sec-hdr"><span class="task-sec-name" style="color:var(--blue)">⚠ 미완료 이동/픽업</span><span class="task-prog">${uncheckedItems.length}건</span></div><div>`;
    uncheckedItems.forEach(u=>{html+=`<div class="task-item"><div class="task-body"><div style="display:flex;align-items:center;gap:5px;flex-wrap:wrap"><span class="bdg ${u.color}">${u.label}</span>${u.isCarry?'<span class="bdg bdg-carry">전날 미완료</span>':''}<span class="task-txt">${esc(u.text)}</span>${u.type?`<span class="type-chip type-${u.type}">${esc(u.type)}</span>`:''}</div>${u.isCarry?`<div class="task-meta"><span style="font-size:10px;color:var(--text3)">${u.ds}</span></div>`:''}</div></div>`;});
    html+='</div></div>';
  }
  const storeItems=[...(DB.tasks[ds].store||[])];
  if(isToday){
    ['mv_in','mv_out','mv_pickup'].forEach(mvKey=>{
      const mvData=DB[mvKey]||{};
      const label=mvKey==='mv_in'?'이동입고':mvKey==='mv_out'?'이동출고':'제품픽업';
      const cdates=[todayStr];
      if(mvKey==='mv_in'){Object.keys(mvData).sort().forEach(d=>{if(d<todayStr)cdates.push(d);});}
      else{for(let k=1;k<=3;k++)cdates.push(fmt(new Date(new Date(todayStr+'T00:00:00').getTime()-k*86400000)));}
      cdates.forEach(checkDs=>{
        const mvItems=(mvData[checkDs]||[]).filter(it=>{
          if(mvKey==='mv_out'){const noJ=['자동','권고'].includes(it.type||'');return !(it.chkDong&&(it.chkJeonsan||noJ));}
          if(mvKey==='mv_in') return !(it.checked||(it.store&&it.duedate&&it.indate));
          return !it.checked;
        });
        mvItems.forEach(it=>{
          const isCarry=checkDs!==todayStr;
          const txt=`[${label}] ${it.pno}${it.size?' ('+it.size+')':''}${it.qty?' x'+it.qty:''}${it.type?' / '+it.type:''}${isCarry?' ← '+checkDs+' 미완료':''}`;
          storeItems.push({id:'__mv__'+it.id+'_'+checkDs,text:txt,done:false,doneAt:null,_isMv:true});
        });
      });
    });
  }
  html+=mkTaskSection('store','매장 전체',ds,storeItems,prev,null);
  DB.staff.forEach(s=>{
    if(!DB.tasks[ds].staff)DB.tasks[ds].staff={};
    if(!DB.tasks[ds].staff[s.id])DB.tasks[ds].staff[s.id]=[];
    html+=mkTaskSection('staff',s.role+' '+s.name,ds,DB.tasks[ds].staff[s.id],prev,s.id);
  });
  document.getElementById('task-sections').innerHTML=html;
}

function mkTaskSection(type,label,ds,items,prev,sid){
  const done=items.filter(t=>t.done).length;
  let pv=[];
  if(prev){if(type==='store')pv=(prev.store||[]).filter(t=>!t.done);else if(sid&&prev.staff)pv=(prev.staff[sid]||[]).filter(t=>!t.done);}
  const key=(type==='store'?'s':sid||'x')+ds.replace(/-/g,'');
  let rows=pv.map(pt=>`<div class="task-item"><div class="chk ${pt.done?'done':''}" onclick="checkCarry('${ds}','${type}','${sid||''}','${pt.id}')"></div><div class="task-body"><div class="task-txt ${pt.done?'done':''}">${esc(pt.text)}</div><div class="task-meta"><span class="bdg bdg-carry">전날 미완료</span>${pt.doneAt?`<span class="bdg bdg-time">완료 ${pt.doneAt}</span>`:''}</div></div></div>`).join('');
  rows+=items.map(t=>`<div class="task-item"><div class="chk ${t.done?'done':''}" onclick="checkTask('${ds}','${type}','${sid||''}','${t.id}')"></div><div class="task-body"><div class="task-txt ${t.done?'done':''}">${esc(t.text)}</div><div class="task-meta">${t.doneAt?`<span class="bdg bdg-time">완료 ${t.doneAt}</span>`:''}${(!t.done&&ds<todayStr)?'<span class="bdg bdg-overdue">미완료</span>':''}</div></div><button class="task-del" onclick="delTask('${ds}','${type}','${sid||''}','${t.id}')">✕</button></div>`).join('');
  if(!rows)rows='<div class="mv-section-empty">할일 없음</div>';
  return`<div class="task-section"><div class="task-sec-hdr"><span class="task-sec-name">${label}</span><span class="task-prog">${done}/${items.length}</span></div><div>${rows}</div><div class="task-add-row"><input type="text" id="inp-${key}" placeholder="할일 입력 후 Enter" onkeydown="if(event.key==='Enter')addTask('${ds}','${type}','${sid||''}','inp-${key}')"><button class="btn" onclick="addTask('${ds}','${type}','${sid||''}','inp-${key}')">추가</button></div></div>`;
}
function getItems(ds,type,sid){if(!DB.tasks[ds])DB.tasks[ds]={store:[],staff:{}};if(type==='store')return DB.tasks[ds].store;if(!DB.tasks[ds].staff)DB.tasks[ds].staff={};if(!DB.tasks[ds].staff[sid])DB.tasks[ds].staff[sid]=[];return DB.tasks[ds].staff[sid];}
window.addTask=function(ds,type,sid,inpId){const el=document.getElementById(inpId);const txt=el.value.trim();if(!txt)return;getItems(ds,type,sid).push({id:'t'+Date.now(),text:txt,done:false,doneAt:null});el.value='';saveMain();renderTasks();};
window.checkTask=function(ds,type,sid,id){const t=getItems(ds,type,sid).find(x=>x.id===id);if(!t||t._isMv)return;t.done=!t.done;if(t.done){const n=new Date();t.doneAt=p2(n.getHours())+':'+p2(n.getMinutes());}else t.doneAt=null;saveMain();renderTasks();};
window.checkCarry=function(ds,type,sid,pid){const prevDs=fmt(new Date(new Date(ds+'T00:00:00').getTime()-86400000));const t=getItems(prevDs,type,sid).find(x=>x.id===pid);if(!t)return;t.done=!t.done;if(t.done){const n=new Date();t.doneAt=p2(n.getHours())+':'+p2(n.getMinutes());}else t.doneAt=null;saveMain();renderTasks();};
window.delTask=function(ds,type,sid,id){if(id.startsWith('__mv__'))return;const items=getItems(ds,type,sid);const i=items.findIndex(x=>x.id===id);if(i>-1)items.splice(i,1);saveMain();renderTasks();};

function getMvItems(key,ds){if(!DB[key])DB[key]={};if(!DB[key][ds])DB[key][ds]=[];return DB[key][ds];}
function renderFilterRow(type,types){
  const el=document.getElementById(type+'-filter-row');if(!el)return;
  const all=['전체',...types];
  el.innerHTML=all.map(t=>`<div class="mv-filter ${filters[type]===t?'active':''}" onclick="setFilter('${type}','${t}')">${t}</div>`).join('');
}
window.setFilter=function(type,val){filters[type]=val;renderMv(type);};

function renderIn(){
  updateDateNav('in');renderFilterRow('in',IN_TYPES);
  const ds=fmt(dates.in);const f=filters.in;
  const items=getMvItems('mv_in',ds);
  const filtered=items.filter(i=>f==='전체'||i.type===f);
  const allPrevIncomplete=[];
  Object.keys(DB.mv_in||{}).sort().forEach(pastDs=>{
    if(pastDs>=ds)return;
    const pastItems=(DB.mv_in[pastDs]||[]).filter(i=>!(i.checked||(i.store&&i.duedate&&i.indate))).filter(i=>f==='전체'||i.type===f);
    if(pastItems.length)allPrevIncomplete.push({ds:pastDs,items:pastItems});
  });
  let html='';
  if(allPrevIncomplete.length){
    html+=`<div style="font-size:11px;font-weight:600;color:var(--orange);margin-bottom:8px">📌 미완료 이동입고</div>`;
    allPrevIncomplete.forEach(({ds:pastDs,items:pastItems})=>{
      html+=`<div style="font-size:10px;color:var(--text3);margin:6px 0 3px;font-weight:500">${pastDs} (${dow(pastDs)})</div>`;
      pastItems.forEach(i=>{html+=mvInRow(i,pastDs,true);});
    });
    if(filtered.length)html+=`<div style="height:1px;background:var(--border);margin:10px 0"></div>`;
  }
  if(filtered.length){filtered.forEach(i=>{html+=mvInRow(i,ds,false);});}
  if(!filtered.length&&!allPrevIncomplete.length)html='<div class="mv-section-empty">등록된 이동입고 없음</div>';
  document.getElementById('in-list').innerHTML=html;
}
function mvInRow(i,ds,carry){
  const bothDates=i.store&&i.duedate&&i.indate;
  const isCompleted=i.checked||bothDates;
  return`<div class="mv-row ${carry?'carry':''}" style="${isCompleted?'opacity:.5':''}">
    <div class="mv-chk ${isCompleted?'done':''}" onclick="checkMv('mv_in','${ds}','${i.id}')"></div>
    <div class="mv-body">
      <div class="mv-main">
        <span class="mv-pno">${esc(i.pno)}</span>
        ${i.size?`<span class="mv-chip">${esc(i.size)}</span>`:''}
        ${i.qty?`<span class="mv-chip">x${i.qty}</span>`:''}
        ${i.type?`<span class="type-chip type-${i.type}">${esc(i.type)}</span>`:''}
        ${i.note?`<span class="mv-chip">${esc(i.note)}</span>`:''}
        ${i.note2?`<span class="mv-chip">${esc(i.note2)}</span>`:''}
        ${isCompleted?'<span class="mv-done-time">✓ 완료</span>':''}
        ${carry?'<span class="mv-carry-lbl">전날 미완료</span>':''}
      </div>
      <div class="mv-meta">
        ${i.store?`<span class="bdg bdg-time">입고매장: ${esc(i.store)}</span>`:''}
        ${i.duedate?`<span class="bdg bdg-time">구한날: ${i.duedate}</span>`:''}
        ${i.indate?`<span class="bdg bdg-time">입고예정일: ${i.indate}</span>`:''}
        ${i.checkedAt?`<span class="mv-done-time">완료 ${i.checkedAt}</span>`:''}
      </div>
      ${!isCompleted?`<div class="in-date-update" style="margin-top:8px;padding-top:8px;border-top:0.5px solid var(--border)">
        <div style="font-size:10px;color:var(--text3);margin-bottom:6px">✏️ 아래 입력 후 완료처리:</div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:5px;margin-bottom:5px">
          <div><div style="font-size:9px;color:var(--text3);margin-bottom:2px">입고매장</div>
          <input type="text" id="in-st-${i.id}" value="${esc(i.store||'')}" placeholder="입고매장" style="font-size:11px;padding:4px 7px;margin:0"></div>
          <div><div style="font-size:9px;color:var(--text3);margin-bottom:2px">추가메모</div>
          <input type="text" id="in-nt2-${i.id}" value="${esc(i.note2||'')}" placeholder="추가메모(선택)" style="font-size:11px;padding:4px 7px;margin:0"></div>
        </div>
        <div style="display:grid;grid-template-columns:1fr 1fr;gap:5px;margin-bottom:6px">
          <div><div style="font-size:9px;color:var(--text3);margin-bottom:2px">구한날</div>
          <input type="date" id="in-due-${i.id}" value="${i.duedate||''}" style="font-size:11px;padding:4px 7px;margin:0"></div>
          <div><div style="font-size:9px;color:var(--text3);margin-bottom:2px">입고예정일</div>
          <input type="date" id="in-ind-${i.id}" value="${i.indate||''}" style="font-size:11px;padding:4px 7px;margin:0"></div>
        </div>
        <button class="btn btn-sm btn-dark" onclick="updateInDate('${ds}','${i.id}')">저장</button>
      </div>`:''}
    </div>
    <button class="mv-del" onclick="delMv('mv_in','${ds}','${i.id}')">✕</button>
  </div>`;
}

window.addMv=function(type){
  const pno=document.getElementById(type+'-pno').value.trim();
  if(!pno){alert('품번을 입력해주세요');return;}
  const ds=fmt(dates[type]);
  const item={id:'m'+Date.now(),pno,checked:false,checkedAt:null};
  if(type==='in'){
    item.size=document.getElementById('in-size').value.trim()||'';
    item.qty=document.getElementById('in-qty').value||'';
    item.type=document.getElementById('in-type').value||'';
    item.store='';item.note=document.getElementById('in-note').value.trim()||'';item.note2='';item.duedate='';item.indate='';
    ['in-size','in-qty','in-note'].forEach(id=>{document.getElementById(id).value='';});
    document.getElementById('in-type').selectedIndex=0;
  }else if(type==='out'){
    item.size=document.getElementById('out-size').value.trim()||'';
    item.qty=document.getElementById('out-qty').value||'';
    item.type=document.getElementById('out-type').value||'';
    item.dong=document.getElementById('out-dong').value.trim()||'';
    item.waybill=document.getElementById('out-waybill').value.trim()||'';
    item.send=document.getElementById('out-send').value||'';
    ['out-size','out-qty','out-dong','out-waybill'].forEach(id=>{const el=document.getElementById(id);if(el)el.value='';});
    document.getElementById('out-type').selectedIndex=0;document.getElementById('out-send').selectedIndex=0;
  }else if(type==='pickup'){
    item.size=document.getElementById('pickup-size').value.trim()||'';
    item.qty=document.getElementById('pickup-qty').value||'';
    item.type=document.getElementById('pickup-type').value||'';
    item.loc=document.getElementById('pickup-loc').value.trim()||'';
    item.note=document.getElementById('pickup-note').value.trim()||'';
    ['pickup-size','pickup-qty','pickup-loc','pickup-note'].forEach(id=>{document.getElementById(id).value='';});
    document.getElementById('pickup-type').selectedIndex=0;
  }
  document.getElementById(type+'-pno').value='';
  getMvItems('mv_'+type,ds).push(item);
  saveMain();renderMv(type);renderTasks();
};
window.checkMv=function(key,ds,id){
  const items=getMvItems(key,ds);const i=items.find(x=>x.id===id);if(!i)return;
  i.checked=!i.checked;
  if(i.checked){const n=new Date();i.checkedAt=p2(n.getHours())+':'+p2(n.getMinutes());}else i.checkedAt=null;
  saveMain();const type=key.replace('mv_','');renderMv(type);renderTasks();
};
window.updateInDate=function(ds,id){
  const items=getMvItems('mv_in',ds);const i=items.find(x=>x.id===id);if(!i)return;
  const stEl=document.getElementById('in-st-'+id);
  const nt2El=document.getElementById('in-nt2-'+id);
  const dueEl=document.getElementById('in-due-'+id);
  const indEl=document.getElementById('in-ind-'+id);
  if(stEl&&stEl.value.trim())i.store=stEl.value.trim();
  if(nt2El)i.note2=nt2El.value.trim();
  if(dueEl&&dueEl.value)i.duedate=dueEl.value;
  if(indEl&&indEl.value)i.indate=indEl.value;
  if(i.store&&i.duedate&&i.indate){i.checked=true;const n=new Date();i.checkedAt=p2(n.getHours())+':'+p2(n.getMinutes());}
  saveMain();renderIn();renderTasks();
};
window.checkMvDual=function(key,ds,id,which){
  const items=getMvItems(key,ds);const i=items.find(x=>x.id===id);if(!i)return;
  const noJeonsanTypes=['자동','권고'];const noJeonsan=noJeonsanTypes.includes(i.type||'');
  if(which==='dong'){i.chkDong=!i.chkDong;}
  else if(which==='jeonsan'&&!noJeonsan){i.chkJeonsan=!i.chkJeonsan;}
  const allDone=i.chkDong&&(i.chkJeonsan||noJeonsan);
  i.checked=allDone;
  if(allDone&&!i.checkedAt){const n=new Date();i.checkedAt=p2(n.getHours())+':'+p2(n.getMinutes());}
  else if(!allDone){i.checkedAt=null;}
  saveMain();const type=key.replace('mv_','');renderMv(type);renderTasks();
};
window.delMv=function(key,ds,id){
  const items=getMvItems(key,ds);const idx=items.findIndex(x=>x.id===id);if(idx>-1)items.splice(idx,1);
  saveMain();const type=key.replace('mv_','');renderMv(type);renderTasks();
};

function renderOut(){
  updateDateNav('out');renderFilterRow('out',OUT_TYPES);
  const ds=fmt(dates.out);const f=filters.out;
  const items=getMvItems('mv_out',ds);
  const filtered=items.filter(i=>f==='전체'||i.type===f);
  const prev3Incomplete=[];
  for(let d=1;d<=3;d++){
    const pastDs=fmt(new Date(new Date(ds+'T00:00:00').getTime()-d*86400000));
    const pastItems=(DB.mv_out[pastDs]||[]).filter(i=>{const noJ=['자동','권고'].includes(i.type||'');return !(i.chkDong&&(i.chkJeonsan||noJ));}).filter(i=>f==='전체'||i.type===f);
    if(pastItems.length)prev3Incomplete.push({ds:pastDs,items:pastItems});
  }
  let html='';
  if(prev3Incomplete.length){
    html+=`<div style="font-size:11px;font-weight:600;color:var(--orange);margin-bottom:8px">📌 미완료 이동출고 (최근 3일)</div>`;
    prev3Incomplete.forEach(({ds:pastDs,items:pastItems})=>{
      html+=`<div style="font-size:10px;color:var(--text3);margin:6px 0 3px;font-weight:500">${pastDs} (${dow(pastDs)})</div>`;
      pastItems.forEach(i=>{html+=mvOutRow(i,pastDs,true);});
    });
    if(filtered.length)html+=`<div style="height:1px;background:var(--border);margin:10px 0"></div>`;
  }
  if(filtered.length){filtered.forEach(i=>{html+=mvOutRow(i,ds,false);});}
  if(!filtered.length&&!prev3Incomplete.length)html='<div class="mv-section-empty">등록된 이동출고 없음</div>';
  document.getElementById('out-list').innerHTML=html;
}
function mvOutRow(i,ds,carry){
  const noJeonsanTypes=['자동','권고'];const noJeonsan=noJeonsanTypes.includes(i.type||'');
  const chkDong=i.chkDong||false;const chkJeonsan=i.chkJeonsan||false;
  const allDone=chkDong&&(chkJeonsan||noJeonsan);
  return`<div class="mv-row ${carry?'carry':''}" style="${allDone?'opacity:.55':''}">
    <div class="mv-chks">
      <div class="mv-chk-wrap"><div class="mv-chk ${chkDong?'done':''}" onclick="checkMvDual('mv_out','${ds}','${i.id}','dong')" title="동진등록"></div><span class="mv-chk-lbl">동진</span></div>
      <div class="mv-chk-wrap">${noJeonsan?`<div class="mv-chk disabled" style="cursor:default"></div>`:`<div class="mv-chk ${chkJeonsan?'done':''}" onclick="checkMvDual('mv_out','${ds}','${i.id}','jeonsan')" title="전산등록"></div>`}<span class="mv-chk-lbl">전산</span></div>
    </div>
    <div class="mv-body">
      <div class="mv-main">
        <span class="mv-pno">${esc(i.pno)}</span>
        ${i.size?`<span class="mv-chip">${esc(i.size)}</span>`:''}
        ${i.qty?`<span class="mv-chip">x${i.qty}</span>`:''}
        ${i.type?`<span class="type-chip type-${i.type}">${esc(i.type)}</span>`:''}
        ${allDone?'<span class="mv-done-time">✓ 완료</span>':''}
        ${carry?'<span class="mv-carry-lbl">전날 미완료</span>':''}
      </div>
      <div class="mv-meta">
        ${i.dong?`<span class="bdg bdg-time">출고매장: ${esc(i.dong)}</span>`:''}
        ${i.send?`<span class="mv-chip">${esc(i.send)}</span>`:''}
        ${i.waybill?`<span class="bdg bdg-time">운송장: ${esc(i.waybill)}</span>`:''}
        ${i.checkedAt?`<span class="mv-done-time">완료 ${i.checkedAt}</span>`:''}
      </div>
    </div>
    <button class="mv-del" onclick="delMv('mv_out','${ds}','${i.id}')">✕</button>
  </div>`;
}

function renderPickup(){
  updateDateNav('pickup');renderFilterRow('pickup',PICKUP_TYPES);
  const ds=fmt(dates.pickup);const f=filters.pickup;
  const items=getMvItems('mv_pickup',ds);
  const filtered=items.filter(i=>f==='전체'||i.type===f);
  const prev3Pickup=[];
  for(let d=1;d<=3;d++){
    const pastDs=fmt(new Date(new Date(ds+'T00:00:00').getTime()-d*86400000));
    const pastItems=(DB.mv_pickup[pastDs]||[]).filter(i=>!i.checked).filter(i=>f==='전체'||i.type===f);
    if(pastItems.length)prev3Pickup.push({ds:pastDs,items:pastItems});
  }
  let html='';
  if(prev3Pickup.length){
    html+=`<div style="font-size:11px;font-weight:600;color:var(--orange);margin-bottom:8px">📌 미완료 제품픽업 (최근 3일)</div>`;
    prev3Pickup.forEach(({ds:pastDs,items:pastItems})=>{
      html+=`<div style="font-size:10px;color:var(--text3);margin:6px 0 3px;font-weight:500">${pastDs} (${dow(pastDs)})</div>`;
      pastItems.forEach(i=>{html+=mvPickupRow(i,pastDs,true);});
    });
    if(filtered.length)html+=`<div style="height:1px;background:var(--border);margin:10px 0"></div>`;
  }
  if(filtered.length){filtered.forEach(i=>{html+=mvPickupRow(i,ds,false);});}
  if(!filtered.length&&!prev3Pickup.length)html='<div class="mv-section-empty">등록된 제품픽업 없음</div>';
  document.getElementById('pickup-list').innerHTML=html;
}
function mvPickupRow(i,ds,carry){
  return`<div class="mv-row ${carry?'carry':''}">
    <div class="mv-chk ${i.checked?'done':''}" onclick="checkMv('mv_pickup','${ds}','${i.id}')"></div>
    <div class="mv-body">
      <div class="mv-main">
        <span class="mv-pno">${esc(i.pno)}</span>
        ${i.size?`<span class="mv-chip">${esc(i.size)}</span>`:''}
        ${i.qty?`<span class="mv-chip">x${i.qty}</span>`:''}
        ${i.type?`<span class="type-chip type-${i.type}">${esc(i.type)}</span>`:''}
        ${carry?'<span class="mv-carry-lbl">전날 미완료</span>':''}
      </div>
      <div class="mv-meta">
        ${i.loc?`<span class="bdg bdg-time">창고: ${esc(i.loc)}</span>`:''}
        ${i.note?`<span class="mv-chip">${esc(i.note)}</span>`:''}
        ${i.checkedAt?`<span class="mv-done-time">완료 ${i.checkedAt}</span>`:''}
      </div>
    </div>
    <button class="mv-del" onclick="delMv('mv_pickup','${ds}','${i.id}')">✕</button>
  </div>`;
}

window.chMon=function(d){calM+=d;if(calM<0){calM=11;calY--;}if(calM>11){calM=0;calY++;}renderCal();}
function renderCal(){
  document.getElementById('cal-mon-lbl').textContent=calY+'년 '+(calM+1)+'월';
  const grid=document.getElementById('cal-grid');grid.innerHTML='';
  const first=new Date(calY,calM,1).getDay(),days=new Date(calY,calM+1,0).getDate(),prev=new Date(calY,calM,0).getDate();
  for(let i=first-1;i>=0;i--)grid.appendChild(mkCell(calY,calM===0?11:calM-1,prev-i,true));
  for(let i=1;i<=days;i++)grid.appendChild(mkCell(calY,calM,i,false));
  const total=first+days,rem=total%7===0?0:7-total%7;
  for(let i=1;i<=rem;i++)grid.appendChild(mkCell(calY,calM===11?0:calM+1,i,true));
  const types=[...new Set(DB.events.map(e=>e.type))];
  document.getElementById('cal-legend').innerHTML=types.map(t=>`<div class="leg"><div class="leg-dot" style="background:${EC[t]}"></div>${EL[t]||t}</div>`).join('')+'<div class="leg"><div class="leg-dot" style="background:var(--red)"></div>휴무</div>';
  renderEvList();
}
function mkCell(y,m,d,other){
  const ds=y+'-'+p2(m+1)+'-'+p2(d),isT=ds===todayStr;
  const c=document.createElement('div');c.className='cal-cell'+(other?' other':'')+(isT?' today':'');
  const offs=Object.entries(DB.off).filter(([,arr])=>arr&&arr.includes(ds));
  if(offs.length)c.classList.add('off-day');
  const numEl=document.createElement('div');numEl.className='cell-num';numEl.textContent=d;c.appendChild(numEl);
  if(offs.length&&!other){const op=document.createElement('div');op.className='off-pill';op.textContent='휴무 '+offs.length+'명';c.appendChild(op);}
  if(!other){
    DB.events.filter(e=>e.date===ds).slice(0,3).forEach(ev=>{const p=document.createElement('div');p.className='ev-pill';p.style.cssText=`background:${EC[ev.type]}15;color:${EC[ev.type]};border-left-color:${EC[ev.type]}`;p.textContent=ev.title;c.appendChild(p);});
    c.onclick=()=>{document.querySelectorAll('.cal-cell').forEach(x=>x.style.outline='');c.style.outline='2px solid var(--text)';document.getElementById('ev-date').value=ds;renderEvList(ds);};
  }
  return c;
}
function renderEvList(sel){
  const list=document.getElementById('ev-list');
  let evs=DB.events.filter(e=>{const d=new Date(e.date+'T00:00:00');return d.getFullYear()===calY&&d.getMonth()===calM;});
  if(sel)evs=evs.filter(e=>e.date===sel);evs.sort((a,b)=>a.date.localeCompare(b.date));
  if(!evs.length){list.innerHTML='<div style="font-size:11px;color:var(--text3);text-align:center;padding:12px">일정 없음</div>';return;}
  list.innerHTML=evs.map(ev=>`<div class="ev-item"><div class="ev-dot" style="background:${EC[ev.type]||'#888'}"></div><div class="ev-body"><div class="ev-ttl">${esc(ev.title)}</div><div class="ev-dt">${ev.date} (${dow(ev.date)}) · ${EL[ev.type]||ev.type}</div></div><button class="ev-del" onclick="delEv('${ev.id}')">✕</button></div>`).join('');
}
window.addEvent=function(){const t=document.getElementById('ev-title').value.trim(),d=document.getElementById('ev-date').value,ty=document.getElementById('ev-type').value;if(!t||!d)return;DB.events.push({id:'e'+Date.now(),title:t,date:d,type:ty});DB.events.sort((a,b)=>a.date.localeCompare(b.date));document.getElementById('ev-title').value='';saveMain();renderCal();};
window.delEv=function(id){DB.events=DB.events.filter(e=>e.id!==id);saveMain();renderCal();};
document.getElementById('ev-date').value=todayStr;

window.chOffMon=function(d){offM+=d;if(offM<0){offM=11;offY--;}if(offM>11){offM=0;offY++;}renderOff();};
function renderOff(){
  const total=DB.staff.length,todayOffs=DB.staff.filter(s=>(DB.off[s.id]||[]).includes(todayStr));
  const mp=offY+'-'+p2(offM+1),mc=DB.staff.reduce((a,s)=>a+((DB.off[s.id]||[]).filter(d=>d.startsWith(mp)).length),0);
  document.getElementById('off-stats').innerHTML=`<div class="stat-box"><div class="stat-num">${total}</div><div class="stat-lbl">전체 직원</div></div><div class="stat-box"><div class="stat-num" style="color:var(--red)">${todayOffs.length}</div><div class="stat-lbl">오늘 휴무</div></div><div class="stat-box"><div class="stat-num">${mc}</div><div class="stat-lbl">${offM+1}월 휴무일수</div></div>`;
  const toc=document.getElementById('today-off-box');
  toc.innerHTML=`<div style="font-size:11px;font-weight:600;color:var(--text3);margin-bottom:6px">오늘 휴무 (${todayStr})</div>`+(todayOffs.length?todayOffs.map(s=>`<span class="tag" style="background:${RC[s.role]}18;color:${RC[s.role]}">${s.role} ${s.name}</span>`).join(''):'<span style="font-size:12px;color:var(--text3)">전원 근무</span>');
  document.getElementById('staff-list').innerHTML=
    `<div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:8px"><button class="nav-btn" onclick="chOffMon(-1)">‹</button><span style="font-size:14px;font-weight:600">${offY}년 ${offM+1}월 휴무</span><button class="nav-btn" onclick="chOffMon(1)">›</button></div>`+
    DB.staff.map(s=>{const ao=(DB.off[s.id]||[]).sort(),mo=ao.filter(d=>d.startsWith(mp)),col=RC[s.role]||'var(--text)';
      return`<div class="staff-card"><div class="staff-hdr"><div style="display:flex;align-items:center;gap:5px"><div id="nw-${s.id}"><span class="staff-nm" style="color:${col}">${esc(s.name)}</span><button class="edit-btn" onclick="startEdit('${s.id}')">✏️</button></div><span class="staff-role">· ${s.role}</span></div><div style="display:flex;align-items:center;gap:5px"><span style="font-size:10px;background:var(--redbg);color:var(--red);padding:2px 7px;border-radius:8px">${mo.length}일</span><button class="btn btn-sm btn-danger" onclick="removeStaff('${s.id}')">삭제</button></div></div><div>${mo.map(d=>{const di=ao.indexOf(d);return`<span class="off-chip">${d}(${dow(d)})<button class="off-chip-del" onclick="removeOff('${s.id}',${di})">✕</button></span>`;}).join('')||`<span style="font-size:11px;color:var(--text3)">${offM+1}월 휴무 없음</span>`}</div><div class="add-off-row"><input type="date" id="od-${s.id}" value="${todayStr}" style="margin:0"><button class="btn btn-sm" onclick="addOff('${s.id}')">휴무 추가</button></div></div>`;
    }).join('');
}
window.startEdit=function(sid){const s=DB.staff.find(x=>x.id===sid);if(!s)return;const w=document.getElementById('nw-'+sid);w.innerHTML=`<input class="nm-inp" id="ni-${sid}" value="${esc(s.name)}" maxlength="10" onkeydown="if(event.key==='Enter')saveName('${sid}');if(event.key==='Escape')renderOff()"><button class="edit-btn" onclick="saveName('${sid}')">✓</button><button class="edit-btn" onclick="renderOff()">✕</button>`;setTimeout(()=>{const i=document.getElementById('ni-'+sid);if(i){i.focus();i.select();}},40);};
window.saveName=function(sid){const i=document.getElementById('ni-'+sid);if(!i)return;const v=i.value.trim();if(!v)return;const s=DB.staff.find(x=>x.id===sid);if(s)s.name=v;saveMain();renderOff();renderTasks();};
window.addOff=function(sid){const v=document.getElementById('od-'+sid).value;if(!v)return;if(!DB.off[sid])DB.off[sid]=[];if(!DB.off[sid].includes(v)){DB.off[sid].push(v);DB.off[sid].sort();}saveMain();renderOff();};
window.removeOff=function(sid,di){DB.off[sid].splice(di,1);saveMain();renderOff();};
window.addStaff=function(){const role=document.getElementById('new-role').value,name=document.getElementById('new-name').value.trim();if(!name)return;DB.staff.push({id:'s'+Date.now(),role,name});document.getElementById('new-name').value='';saveMain();renderOff();};
window.removeStaff=function(id){if(!confirm('직원을 삭제하시겠습니까?'))return;DB.staff=DB.staff.filter(s=>s.id!==id);delete DB.off[id];saveMain();renderOff();};

function sheetUrl(n){return`https://docs.google.com/spreadsheets/d/${SHEET_ID}/gviz/tq?tqx=out:csv&sheet=${encodeURIComponent(n)}`;}
function parseCSV(csv){return csv.trim().split('\n').map(line=>{const cells=[];let cur='',inQ=false;for(let i=0;i<line.length;i++){const c=line[i];if(c==='"'){if(inQ&&line[i+1]==='"'){cur+='"';i++;}else inQ=!inQ;}else if(c===','&&!inQ){cells.push(cur.trim());cur='';}else cur+=c;}cells.push(cur.trim());return cells;});}
function nowStr(){const n=new Date();return n.getFullYear()+'.'+(n.getMonth()+1)+'.'+n.getDate()+' '+p2(n.getHours())+':'+p2(n.getMinutes());}
async function loadSheet(sn){try{const r=await fetch(sheetUrl(sn));const csv=await r.text();const rows=parseCSV(csv);if(rows.length<1){INV[sn]={headers:[],rows:[],loadedAt:nowStr()};return;}INV[sn]={headers:rows[0],rows:rows.slice(1).filter(r=>r.some(c=>c)),loadedAt:nowStr()};}catch(e){INV[sn]={headers:[],rows:[],loadedAt:'',error:true};}}
async function loadAllSheets(){await Promise.all(SHEETS.map(s=>loadSheet(s.name)));}
function renderInvPanel(){
  document.getElementById('inv-tabs').innerHTML=SHEETS.map((s,i)=>`<div class="inv-tab ${i===curInvSheet?'active':''}" onclick="switchInvSheet(${i})">${s.label}</div>`).join('');
  renderInvSheet();
}
window.switchInvSheet=function(i){curInvSheet=i;document.getElementById('inv-search').value='';document.getElementById('inv-search-results').innerHTML='';renderInvPanel();if(!INV[SHEETS[i].name])loadSheet(SHEETS[i].name).then(()=>renderInvSheet());};
function renderInvSheet(){
  const sh=SHEETS[curInvSheet],inv=INV[sh.name],panel=document.getElementById('inv-panel');
  if(!inv){panel.innerHTML='<div style="text-align:center;padding:30px;color:var(--text3)">불러오는 중...</div>';loadSheet(sh.name).then(()=>renderInvSheet());return;}
  if(inv.error){panel.innerHTML=`<div class="card" style="text-align:center;color:var(--red);padding:20px">로드 실패 — 공개 설정 확인<br><br><button class="reload-btn" onclick="reloadInvSheet()">다시 시도</button></div>`;return;}
  if(!inv.rows||!inv.rows.length){panel.innerHTML=`<div class="card" style="text-align:center;color:var(--text3);padding:20px">${sh.label} — 데이터 없음<br><button class="reload-btn" style="margin-top:8px" onclick="reloadInvSheet()">새로고침</button></div>`;return;}
  panel.innerHTML=`<div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:8px;flex-wrap:wrap;gap:6px"><span style="font-size:11px;color:var(--text3)">구글 시트 · ${inv.loadedAt}</span><div style="display:flex;align-items:center;gap:7px"><span style="font-size:11px;background:var(--bg2);color:var(--text2);padding:2px 8px;border-radius:8px">${inv.rows.length}행</span><button class="reload-btn" onclick="reloadInvSheet()">새로고침</button></div></div>${renderInvTable(inv.headers,inv.rows,'')}`;
}
window.reloadInvSheet=function(){const sn=SHEETS[curInvSheet].name;delete INV[sn];renderInvSheet();};
function renderInvTable(headers,rows,kw){
  if(!headers||!headers.length)return '';
  let html=`<div class="tbl-wrap"><table class="tbl"><thead><tr>${headers.map(h=>`<th>${esc(h)}</th>`).join('')}</tr></thead><tbody>`;
  let cnt=0;
  rows.forEach(row=>{
    if(kw&&!row.some(c=>String(c).toLowerCase().includes(kw.toLowerCase())))return;
    cnt++;html+=`<tr>${row.map((cell,ci)=>{const s=esc(String(cell||''));const v=kw?s.replace(new RegExp('('+kw.replace(/[.*+?^${}()|[\]\\]/g,'\\$&')+')','gi'),'<mark class="hl">$1</mark>'):s;if(ci===headers.length-1&&!isNaN(parseInt(cell))){const n=parseInt(cell);return`<td class="${n===0?'qty-zero':n<=3?'qty-low':'qty-ok'}">${v}</td>`;}return`<td>${v}</td>`;}).join('')}</tr>`;
  });
  html+=`</tbody></table></div>`;
  if(kw&&cnt===0)return`<div style="text-align:center;padding:12px;font-size:12px;color:var(--text3)">결과 없음</div>`;
  return html;
}
window.searchInv=function(){
  const q=document.getElementById('inv-search').value.trim(),res=document.getElementById('inv-search-results');
  if(!q){res.innerHTML='';return;}
  const found=[];
  SHEETS.forEach(sh=>{const inv=INV[sh.name];if(!inv||!inv.rows||!inv.rows.length)return;const mr=inv.rows.filter(r=>r.some(c=>String(c).toLowerCase().includes(q.toLowerCase())));if(mr.length)found.push({label:sh.label,headers:inv.headers,rows:mr});});
  if(!found.length){res.innerHTML=`<div class="card" style="text-align:center;color:var(--text3);font-size:12px;padding:18px">"${esc(q)}" — 결과 없음</div>`;return;}
  const total=found.reduce((a,f)=>a+f.rows.length,0);
  res.innerHTML=`<div style="font-size:11px;color:var(--text2);margin-bottom:8px">총 <b>${total}건</b></div>`+found.map(f=>`<div style="background:var(--bg);border:0.5px solid var(--border);border-radius:10px;padding:10px;margin-bottom:8px"><div style="font-size:11px;font-weight:500;background:var(--bg2);color:var(--text2);padding:2px 8px;border-radius:7px;display:inline-block;margin-bottom:7px">${f.label} · ${f.rows.length}건</div>${renderInvTable(f.headers,f.rows,q)}</div>`).join('');
};

window.addEventListener('online',()=>loadMain());
window.addEventListener('offline',setSyncErr);
loadMain();
setTimeout(()=>{
  const invTab=document.querySelectorAll('.tab')[6];
  if(invTab)invTab.addEventListener('click',()=>{if(Object.keys(INV).length===0)loadAllSheets().then(()=>renderInvSheet());});
},100);
</script>
</body>
</html>
