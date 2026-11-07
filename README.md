<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="description" content="Official website of Imani Marianists CTC Sports Football Team — One Team. One Dream. One Family.">
<title>Imani Marianists CTC Sports Football Team</title>
<style>
/* ============================================================
   BASE / TOKENS
============================================================ */
*,*::before,*::after{box-sizing:border-box}
:root{
  --red:#C8102E; --red-dark:#9E0C24; --red-soft:#FBEBEE;
  --green:#0B6B3A; --green-dark:#074D29; --green-soft:#E8F3EC;
  --yellow:#FFC72C; --yellow-dark:#E0A800;
  --blue:#1D4ED8; --blue-soft:#E8EDFD;
  --ink:#141A22; --muted:#5B6775; --line:#E3E8EF;
  --bg:#F5F7FA; --white:#fff;
  --shadow:0 10px 30px rgba(15,23,42,.09);
  --shadow-lg:0 20px 45px rgba(15,23,42,.16);
  --radius:16px;
}
html{scroll-behavior:smooth}
body{
  margin:0;background:var(--bg);color:var(--ink);line-height:1.6;
  font-family:"Segoe UI",system-ui,-apple-system,Roboto,Helvetica,Arial,sans-serif;
  -webkit-font-smoothing:antialiased;
}
img{max-width:100%;display:block}
a{color:inherit;text-decoration:none}
button{font-family:inherit}
input,select,textarea{font-family:inherit;font-size:.92rem}
.wrap{width:min(1180px,100% - 2rem);margin-inline:auto}
.sr{position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0 0 0 0)}

/* ============================================================
   HEADER / NAV
============================================================ */
#topbar{
  position:sticky;top:0;z-index:60;
  background:linear-gradient(100deg,var(--red) 0%,var(--red-dark) 55%,#7A0A1B 100%);
  border-bottom:3px solid var(--yellow);
  box-shadow:0 2px 16px rgba(0,0,0,.22);
}
.nav-wrap{position:relative;display:flex;align-items:center;gap:1rem;min-height:68px}
.brand{display:flex;align-items:center;gap:.7rem;color:#fff;flex:none}
.crest{
  width:44px;height:44px;border-radius:50%;flex:none;
  background:radial-gradient(circle at 30% 25%,#12894b,var(--green-dark));
  border:2px solid var(--yellow);
  display:grid;place-items:center;color:#fff;font-weight:900;
  font-size:.86rem;letter-spacing:.5px;text-shadow:0 1px 2px rgba(0,0,0,.4);
}
.brand-text strong{display:block;font-size:.94rem;letter-spacing:.09em;line-height:1.15}
.brand-text small{display:block;font-size:.64rem;letter-spacing:.16em;text-transform:uppercase;color:var(--yellow);font-weight:700}
#nav{margin-left:auto;display:flex;gap:.12rem;flex-wrap:wrap;align-items:center}
#nav a{
  color:#fff;font-size:.82rem;font-weight:600;padding:.48rem .62rem;
  border-radius:9px;opacity:.93;transition:.16s;white-space:nowrap;
}
#nav a:hover{background:rgba(255,255,255,.15);opacity:1}
#nav a.active{background:var(--yellow);color:#3A2A00;opacity:1}
#nav a.nav-admin{border:1px solid rgba(255,255,255,.45)}
#nav a.nav-admin.active{border-color:transparent}
.menu-btn{
  display:none;margin-left:auto;background:rgba(255,255,255,.16);border:0;color:#fff;
  font-size:1.25rem;line-height:1;padding:.42rem .7rem;border-radius:10px;cursor:pointer;
}
@media (max-width:1000px){
  .menu-btn{display:block}
  #nav{
    position:absolute;top:100%;left:0;right:0;margin:0;padding:.5rem;
    background:var(--red-dark);flex-direction:column;align-items:stretch;
    display:none;box-shadow:0 16px 30px rgba(0,0,0,.32);
    border-bottom:3px solid var(--yellow);
  }
  #nav.open{display:flex}
  #nav a{padding:.7rem .8rem;font-size:.9rem}
}

/* ============================================================
   BUTTONS / BADGES
============================================================ */
.btn{
  display:inline-flex;align-items:center;justify-content:center;gap:.42rem;
  padding:.72rem 1.25rem;border-radius:999px;font-weight:800;font-size:.86rem;
  border:2px solid transparent;cursor:pointer;transition:.18s;letter-spacing:.02em;
  text-align:center;
}
.btn:active{transform:scale(.98)}
.btn-yellow{background:var(--yellow);color:#3A2A00}
.btn-yellow:hover{background:#FFD65C;transform:translateY(-2px);box-shadow:0 10px 22px rgba(0,0,0,.22)}
.btn-outline{border-color:rgba(255,255,255,.75);color:#fff;background:rgba(255,255,255,.06)}
.btn-outline:hover{background:#fff;color:var(--red)}
.btn-red{background:var(--red);color:#fff}
.btn-red:hover{background:var(--red-dark);transform:translateY(-2px)}
.btn-green{background:var(--green);color:#fff}
.btn-green:hover{background:var(--green-dark);transform:translateY(-2px)}
.btn-ghost{background:#fff;border-color:var(--line);color:var(--ink)}
.btn-ghost:hover{border-color:var(--red);color:var(--red)}
.btn-sm{padding:.45rem .9rem;font-size:.76rem;border-radius:9px}
.btn-block{width:100%}
.badge{
  display:inline-block;font-size:.66rem;font-weight:800;letter-spacing:.1em;
  text-transform:uppercase;padding:.22rem .6rem;border-radius:999px;
}
.badge.men{background:var(--red-soft);color:var(--red)}
.badge.women{background:var(--green-soft);color:var(--green)}
.badge.up{background:var(--blue-soft);color:var(--blue)}
.badge.done{background:#EEF1F5;color:#54606E}

/* ============================================================
   HERO
============================================================ */
.hero{
  position:relative;overflow:hidden;color:#fff;
  background:linear-gradient(120deg,var(--green-dark) 0%,var(--green) 42%,var(--red) 100%);
}
.hero-bg{position:absolute;inset:0;background-size:cover;background-position:center;opacity:.42}
.hero::before{
  content:"";position:absolute;inset:0;z-index:1;
  background-image:repeating-linear-gradient(135deg,rgba(255,255,255,.05) 0 16px,transparent 16px 32px);
  pointer-events:none;
}
.hero-inner{position:relative;z-index:2;padding:4.4rem 0 3.4rem}
.hero-kicker{
  display:inline-block;font-size:.72rem;font-weight:800;letter-spacing:.2em;
  text-transform:uppercase;color:#3A2A00;background:var(--yellow);
  padding:.34rem .9rem;border-radius:999px;margin:0 0 1rem;
}
.hero-title{
  margin:0;font-size:clamp(2rem,6.2vw,3.7rem);line-height:1.03;
  letter-spacing:.02em;font-weight:900;text-shadow:0 4px 22px rgba(0,0,0,.35);
}
.hero-tag{
  margin:.7rem 0 0;font-size:clamp(.78rem,2.1vw,1rem);font-weight:800;
  letter-spacing:.28em;color:var(--yellow);text-transform:uppercase;
}
.hero-sub{max-width:56ch;margin:1.1rem 0 0;font-size:.98rem;color:rgba(255,255,255,.92)}
.hero-cta{display:flex;flex-wrap:wrap;gap:.7rem;margin-top:1.6rem}
.hero-strip{
  display:grid;grid-template-columns:repeat(auto-fit,minmax(120px,1fr));
  gap:.75rem;margin-top:2.4rem;max-width:720px;
}
.hero-strip>div{
  background:rgba(255,255,255,.12);border:1px solid rgba(255,255,255,.22);
  border-radius:12px;padding:.7rem .9rem;backdrop-filter:blur(6px);
}
.hero-strip b{display:block;font-size:1.4rem;line-height:1.1}
.hero-strip span{font-size:.7rem;letter-spacing:.1em;text-transform:uppercase;opacity:.88}

/* ============================================================
   SECTIONS / CARDS
============================================================ */
.page{padding:2.6rem 0 3.4rem}
.sec{margin-bottom:3rem}
.sec:last-child{margin-bottom:0}
.sec-head{
  display:flex;align-items:flex-end;justify-content:space-between;
  gap:1rem;flex-wrap:wrap;margin-bottom:1.4rem;
}
.eyebrow{
  display:inline-block;font-size:.68rem;font-weight:800;letter-spacing:.18em;
  text-transform:uppercase;color:var(--green);background:var(--green-soft);
  padding:.26rem .72rem;border-radius:999px;margin-bottom:.55rem;
}
.sec-title{margin:0;font-size:clamp(1.25rem,3.4vw,1.7rem);letter-spacing:.01em;line-height:1.2}
.sec-title em{font-style:normal;color:var(--red)}
.sec-sub{margin:.35rem 0 0;color:var(--muted);font-size:.9rem;max-width:62ch}
.card{
  background:#fff;border:1px solid var(--line);border-radius:var(--radius);
  padding:1.3rem;box-shadow:0 2px 10px rgba(15,23,42,.04);
}
.grid-auto{display:grid;gap:1.1rem}
.quick-grid{grid-template-columns:repeat(auto-fit,minmax(165px,1fr))}
.quick-card{
  background:#fff;border:1px solid var(--line);border-radius:14px;padding:1.05rem;
  display:flex;flex-direction:column;gap:.28rem;border-top:4px solid var(--red);
  transition:.2s;
}
.quick-card:nth-child(2n){border-top-color:var(--green)}
.quick-card:nth-child(3n){border-top-color:var(--yellow)}
.quick-card:nth-child(5n){border-top-color:var(--blue)}
.quick-card:hover{transform:translateY(-4px);box-shadow:var(--shadow)}
.quick-card .ico{font-size:1.5rem;line-height:1}
.quick-card b{font-size:.94rem}
.quick-card small{color:var(--muted);font-size:.75rem}

/* news */
.news-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(255px,1fr));gap:1.1rem}
.news-card{
  background:#fff;border:1px solid var(--line);border-radius:14px;padding:1.15rem;
  border-left:5px solid var(--yellow);display:flex;flex-direction:column;gap:.4rem;
}
.news-card h3{margin:0;font-size:1rem;line-height:1.35}
.news-card p{margin:0;font-size:.85rem;color:var(--muted)}
.news-date{font-size:.7rem;font-weight:800;letter-spacing:.12em;text-transform:uppercase;color:var(--red)}

/* ============================================================
   PLAYER CARDS
============================================================ */
.p-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(228px,1fr));gap:1.15rem}
.p-card{
  background:#fff;border:1px solid var(--line);border-radius:16px;overflow:hidden;
  display:flex;flex-direction:column;transition:.22s;
}
.p-card:hover{transform:translateY(-5px);box-shadow:var(--shadow-lg);border-color:#F3C6CF}
.p-card-photo{
  position:relative;aspect-ratio:4/3.3;display:grid;place-items:center;overflow:hidden;
  background:linear-gradient(160deg,#D4233C,var(--red-dark) 65%,#6E0817);
}
.p-card-photo.women{background:linear-gradient(160deg,#12894B,var(--green-dark) 70%,#032715)}
.p-card-photo img{width:100%;height:100%;object-fit:cover}
.p-card-photo .sil{width:62%;height:62%;fill:rgba(255,255,255,.3)}
.p-num{
  position:absolute;top:.6rem;left:.6rem;background:var(--yellow);color:#3A2A00;
  font-weight:900;font-size:.82rem;padding:.14rem .55rem;border-radius:8px;
  box-shadow:0 2px 8px rgba(0,0,0,.25);
}
.p-pos{
  position:absolute;bottom:.6rem;right:.6rem;background:rgba(0,0,0,.55);color:#fff;
  font-size:.64rem;font-weight:800;letter-spacing:.09em;text-transform:uppercase;
  padding:.22rem .6rem;border-radius:999px;backdrop-filter:blur(4px);
}
.p-card-body{padding:.95rem 1rem 1.05rem;display:flex;flex-direction:column;gap:.5rem;flex:1}
.p-name{margin:0;font-size:1rem;line-height:1.25}
.p-meta{margin:0;font-size:.76rem;color:var(--muted)}
.p-mini{display:grid;grid-template-columns:repeat(3,1fr);gap:.35rem;margin-top:.15rem}
.p-mini>div{background:#F7F9FC;border:1px solid var(--line);border-radius:9px;padding:.35rem .2rem;text-align:center}
.p-mini b{display:block;font-size:.92rem;line-height:1.15}
.p-mini span{font-size:.6rem;letter-spacing:.07em;text-transform:uppercase;color:var(--muted);font-weight:700}
.p-card .btn{margin-top:auto}

/* squad toolbar */
.toolbar{
  display:flex;gap:.7rem;flex-wrap:wrap;align-items:center;justify-content:space-between;
  background:#fff;border:1px solid var(--line);border-radius:14px;padding:.75rem .9rem;
  margin-bottom:1.4rem;
}
.search{position:relative;flex:1 1 240px;min-width:180px}
.search input{
  width:100%;padding:.62rem .9rem .62rem 2.2rem;border:1px solid var(--line);
  border-radius:999px;background:#F7F9FC;outline:none;
}
.search input:focus{border-color:var(--green);background:#fff;box-shadow:0 0 0 3px rgba(11,107,58,.12)}
.search::before{content:"🔍";position:absolute;left:.8rem;top:50%;transform:translateY(-50%);font-size:.85rem;opacity:.6}
.seg{display:inline-flex;background:#EEF2F7;border-radius:999px;padding:.22rem;gap:.15rem}
.seg button{
  border:0;background:transparent;padding:.45rem .95rem;border-radius:999px;
  font-size:.8rem;font-weight:800;color:var(--muted);cursor:pointer;transition:.16s;
}
.seg button.on{background:var(--red);color:#fff;box-shadow:0 4px 12px rgba(200,16,46,.3)}
.seg button.on.green{background:var(--green);box-shadow:0 4px 12px rgba(11,107,58,.3)}

/* ============================================================
   PROFILE PAGE
============================================================ */
.profile{display:grid;grid-template-columns:300px 1fr;gap:1.6rem;align-items:start}
@media(max-width:820px){.profile{grid-template-columns:1fr}}
.profile-photo{
  border-radius:18px;overflow:hidden;aspect-ratio:3/3.6;display:grid;place-items:center;
  background:linear-gradient(160deg,#D4233C,var(--red-dark));position:relative;
}
.profile-photo.women{background:linear-gradient(160deg,#12894B,var(--green-dark))}
.profile-photo img{width:100%;height:100%;object-fit:cover}
.profile-photo .sil{width:58%;fill:rgba(255,255,255,.3)}
.profile-num{
  position:absolute;bottom:0;left:0;right:0;text-align:center;font-size:3.4rem;font-weight:900;
  color:rgba(255,255,255,.9);background:linear-gradient(transparent,rgba(0,0,0,.55));
  padding:1.4rem 0 .6rem;line-height:1;
}
.stat-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(104px,1fr));gap:.7rem;margin-top:1rem}
.stat-box{
  background:#fff;border:1px solid var(--line);border-radius:12px;padding:.8rem .5rem;
  text-align:center;border-bottom:3px solid var(--green);
}
.stat-box b{display:block;font-size:1.35rem;line-height:1.1}
.stat-box span{font-size:.65rem;letter-spacing:.08em;text-transform:uppercase;color:var(--muted);font-weight:800}
.stat-box.red{border-bottom-color:var(--red)}
.stat-box.yellow{border-bottom-color:var(--yellow)}
.stat-box.blue{border-bottom-color:var(--blue)}

/* ============================================================
   LEADERBOARDS / STATS
============================================================ */
.lb{background:#fff;border:1px solid var(--line);border-radius:16px;overflow:hidden}
.lb-head{
  padding:.85rem 1rem;font-weight:900;font-size:.8rem;letter-spacing:.12em;text-transform:uppercase;
  color:#fff;background:linear-gradient(90deg,var(--red),var(--red-dark));
}
.lb-head.green{background:linear-gradient(90deg,var(--green),var(--green-dark))}
.lb-row{display:flex;align-items:center;gap:.75rem;padding:.68rem .9rem;border-bottom:1px solid var(--line)}
.lb-row:last-child{border-bottom:0}
.lb-row:hover{background:#FAFBFD}
.lb-rank{
  width:28px;height:28px;flex:none;border-radius:8px;display:grid;place-items:center;
  font-weight:900;font-size:.76rem;background:#EEF1F6;color:#5B6775;
}
.lb-rank.r1{background:var(--yellow);color:#3A2A00}
.lb-rank.r2{background:#D6DEE8;color:#36414F}
.lb-rank.r3{background:#F0C9A0;color:#6B3E12}
.lb-name{flex:1;font-weight:700;font-size:.88rem;min-width:0;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.lb-name small{display:block;font-weight:600;font-size:.7rem;color:var(--muted)}
.lb-val{font-weight:900;font-size:.95rem;color:var(--red)}
.lb-head.green ~ .lb-row .lb-val{color:var(--green)}
.lb-empty{padding:1.6rem 1rem;text-align:center;color:var(--muted);font-size:.85rem}
.two-col{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:1.1rem}

.potm{
  background:linear-gradient(135deg,var(--green-dark),var(--green) 60%,#0F8A4A);
  color:#fff;border-radius:18px;padding:1.4rem;display:flex;align-items:center;gap:1.1rem;
  flex-wrap:wrap;
}
.potm .avatar{
  width:72px;height:72px;border-radius:50%;flex:none;display:grid;place-items:center;
  background:rgba(255,255,255,.16);border:2px solid var(--yellow);font-weight:900;font-size:1.4rem;
}
.potm h4{margin:0;font-size:1.05rem}
.potm p{margin:.15rem 0 0;font-size:.82rem;opacity:.9}
.potm .tag{
  margin-left:auto;background:var(--yellow);color:#3A2A00;font-weight:900;font-size:.68rem;
  letter-spacing:.12em;text-transform:uppercase;padding:.35rem .8rem;border-radius:999px;
}

/* ============================================================
   MATCHES
============================================================ */
.match-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:1.1rem}
.match{background:#fff;border:1px solid var(--line);border-radius:16px;padding:1rem 1.1rem;display:flex;flex-direction:column;gap:.7rem}
.match-top{display:flex;justify-content:space-between;align-items:center;gap:.5rem;font-size:.72rem;color:var(--muted);font-weight:700;letter-spacing:.05em}
.match-teams{display:grid;grid-template-columns:1fr auto 1fr;align-items:center;gap:.6rem}
.match-teams .tn{font-weight:800;font-size:.88rem;line-height:1.25}
.match-teams .tn.right{text-align:right}
.score{
  font-weight:900;font-size:1.2rem;background:#F4F6FA;border:1px solid var(--line);
  padding:.35rem .75rem;border-radius:11px;white-space:nowrap;color:var(--red);
}
.score.vs{color:var(--green);font-size:.95rem}
.match-meta{font-size:.78rem;color:var(--muted);border-top:1px dashed var(--line);padding-top:.6rem}
.match-meta b{color:var(--ink)}
.match-report{font-size:.82rem;color:var(--muted);margin:0}

/* ============================================================
   GALLERY
============================================================ */
.gal-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(195px,1fr));gap:.9rem}
.gal-item{
  position:relative;border-radius:14px;overflow:hidden;aspect-ratio:4/3;
  display:grid;place-items:center;color:rgba(255,255,255,.62);
  background:linear-gradient(140deg,#1F2937,#0B6B3A);cursor:pointer;
}
.gal-item:nth-child(3n){background:linear-gradient(140deg,#7A0A1B,#C8102E)}
.gal-item:nth-child(4n){background:linear-gradient(140deg,#123B63,#1D4ED8)}
.gal-item img{width:100%;height:100%;object-fit:cover;transition:.3s}
.gal-item:hover img{transform:scale(1.06)}
.gal-item .ph{font-size:2rem;opacity:.55}
.gal-cap{
  position:absolute;inset:auto 0 0 0;padding:1.4rem .8rem .6rem;color:#fff;
  font-size:.76rem;font-weight:700;background:linear-gradient(transparent,rgba(0,0,0,.82));
}
.gal-cap small{display:block;font-weight:600;font-size:.66rem;opacity:.85;text-transform:uppercase;letter-spacing:.1em}

/* ============================================================
   ABOUT / CONTACT
============================================================ */
.value-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:1rem}
.value{background:#fff;border:1px solid var(--line);border-radius:14px;padding:1.1rem;border-top:4px solid var(--green)}
.value h4{margin:.1rem 0 .4rem;font-size:.95rem}
.value p{margin:0;font-size:.82rem;color:var(--muted)}
.prose p{color:var(--muted);font-size:.92rem}
.prose h3{margin-top:0}
.timeline{list-style:none;padding:0;margin:0;display:flex;flex-direction:column;gap:.7rem}
.timeline li{display:flex;gap:.9rem;align-items:flex-start;background:#fff;border:1px solid var(--line);border-radius:12px;padding:.85rem 1rem}
.timeline b{color:var(--red);flex:none;font-size:.82rem;min-width:66px}
.timeline span{font-size:.86rem;color:var(--muted)}
.contact-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(215px,1fr));gap:1rem}
.contact-card{background:#fff;border:1px solid var(--line);border-radius:14px;padding:1.1rem;display:flex;gap:.8rem;align-items:flex-start}
.contact-card .ico{
  width:38px;height:38px;flex:none;border-radius:11px;display:grid;place-items:center;
  background:var(--red-soft);color:var(--red);font-size:1.05rem;
}
.contact-card b{display:block;font-size:.78rem;letter-spacing:.09em;text-transform:uppercase;color:var(--muted)}
.contact-card span{font-size:.9rem;font-weight:600;word-break:break-word}
.socials{display:flex;gap:.6rem;flex-wrap:wrap;margin-top:1rem}
.socials a{
  padding:.5rem 1rem;border-radius:999px;background:#fff;border:1px solid var(--line);
  font-size:.8rem;font-weight:800;transition:.16s;
}
.socials a:hover{background:var(--green);border-color:var(--green);color:#fff}

/* ============================================================
   FORMS
============================================================ */
label{display:flex;flex-direction:column;gap:.3rem;font-size:.75rem;font-weight:800;letter-spacing:.06em;text-transform:uppercase;color:var(--muted)}
input,select,textarea{
  padding:.62rem .75rem;border:1px solid var(--line);border-radius:10px;background:#F9FAFC;
  color:var(--ink);outline:none;transition:.16s;width:100%;text-transform:none;font-weight:500;letter-spacing:0;
}
input:focus,select:focus,textarea:focus{border-color:var(--green);background:#fff;box-shadow:0 0 0 3px rgba(11,107,58,.12)}
textarea{resize:vertical;min-height:74px}
.form-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(190px,1fr));gap:.9rem}
.form-grid .full{grid-column:1/-1}
.form-head{grid-column:1/-1;display:flex;align-items:center;justify-content:space-between;gap:1rem;flex-wrap:wrap}
.form-head h3{margin:0;font-size:1.05rem}
.form-actions{grid-column:1/-1;display:flex;gap:.6rem;flex-wrap:wrap}
.photo-row{grid-column:1/-1;display:flex;align-items:center;gap:1rem;flex-wrap:wrap}
.photo-prev{
  width:78px;height:78px;border-radius:12px;overflow:hidden;flex:none;display:grid;place-items:center;
  background:linear-gradient(160deg,#D4233C,var(--red-dark));
}
.photo-prev img{width:100%;height:100%;object-fit:cover}
.photo-prev .sil{width:60%;fill:rgba(255,255,255,.4)}
.file-btn{position:relative;overflow:hidden}
.hint{font-size:.78rem;color:var(--muted);margin:.4rem 0 0}
code{background:#EEF2F7;padding:.1rem .4rem;border-radius:6px;font-size:.82em}

/* ============================================================
   ADMIN
============================================================ */
.admin-head{
  background:linear-gradient(120deg,var(--red-dark),var(--red) 60%,#8C0F27);
  color:#fff;border-radius:18px;padding:1.5rem;margin-bottom:1.4rem;
  display:flex;align-items:center;gap:1rem;flex-wrap:wrap;
}
.admin-head h2{margin:0;font-size:1.25rem}
.admin-head p{margin:.2rem 0 0;font-size:.82rem;opacity:.9}
.admin-head .btn{margin-left:auto}
.tabs{display:flex;gap:.4rem;flex-wrap:wrap;margin-bottom:1.2rem}
.tabs button{
  border:1px solid var(--line);background:#fff;padding:.55rem 1rem;border-radius:999px;
  font-size:.8rem;font-weight:800;color:var(--muted);cursor:pointer;transition:.16s;
}
.tabs button.on{background:var(--green);border-color:var(--green);color:#fff}
.admin-bar{display:flex;gap:.7rem;flex-wrap:wrap;align-items:center;justify-content:space-between;margin-bottom:1rem}
.adm-list{display:flex;flex-direction:column;gap:.55rem}
.adm-row{
  display:flex;align-items:center;gap:.85rem;background:#fff;border:1px solid var(--line);
  border-radius:12px;padding:.6rem .85rem;flex-wrap:wrap;
}
.adm-avatar{
  width:40px;height:40px;border-radius:10px;flex:none;display:grid;place-items:center;overflow:hidden;
  background:linear-gradient(160deg,#D4233C,var(--red-dark));font-weight:900;color:#fff;font-size:.82rem;
}
.adm-avatar.women{background:linear-gradient(160deg,#12894B,var(--green-dark))}
.adm-avatar img{width:100%;height:100%;object-fit:cover}
.adm-info{flex:1 1 180px;min-width:0}
.adm-info b{display:block;font-size:.88rem}
.adm-info small{color:var(--muted);font-size:.74rem}
.adm-actions{display:flex;gap:.4rem;margin-left:auto}
.gate{max-width:420px;margin:2rem auto}

/* ============================================================
   FOOTER
============================================================ */
footer{
  background:#101620;color:#B9C3CF;padding:2.6rem 0 1.4rem;margin-top:2rem;
  border-top:4px solid var(--red);
}
.foot-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:1.6rem}
.foot-grid h4{color:#fff;margin:0 0 .6rem;font-size:.82rem;letter-spacing:.14em;text-transform:uppercase}
.foot-grid p,.foot-grid a{font-size:.84rem;color:#B9C3CF;display:block;margin:.18rem 0}
.foot-grid a:hover{color:var(--yellow)}
.foot-tag{color:var(--yellow);font-weight:900;letter-spacing:.18em;font-size:.74rem;text-transform:uppercase}
.foot-bottom{
  border-top:1px solid #22303F;margin-top:1.8rem;padding-top:1.1rem;
  display:flex;justify-content:space-between;gap:1rem;flex-wrap:wrap;
  font-size:.76rem;color:#7C8899;
}
.empty{text-align:center;color:var(--muted);padding:2rem 1rem;font-size:.88rem;background:#fff;border:1px dashed var(--line);border-radius:14px}
</style>
</head>
<body>

<header id="topbar">
  <div class="wrap nav-wrap">
    <a class="brand" href="#home">
      <span class="crest">IM</span>
      <span class="brand-text">
        <strong>IMANI MARIANISTS</strong>
        <small>CTC Sports Football Team</small>
      </span>
    </a>
    <button class="menu-btn" id="menuBtn" aria-label="Toggle menu" aria-expanded="false">☰</button>
    <nav id="nav">
      <a href="#home">Home</a>
      <a href="#men">Men's Team</a>
      <a href="#women">Women's Team</a>
      <a href="#stats">Goals &amp; Stats</a>
      <a href="#matches">Matches</a>
      <a href="#gallery">Gallery</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
      <a href="#admin" class="nav-admin">Admin</a>
    </nav>
  </div>
</header>

<main id="view"></main>

<footer>
  <div class="wrap">
    <div class="foot-grid">
      <div>
        <h4>Imani Marianists CTC</h4>
        <p class="foot-tag">One Team. One Dream. One Family.</p>
        <p style="margin-top:.7rem">Official home of the Imani Marianists CTC Sports Football Team — developing talent, building character and playing with pride.</p>
      </div>
      <div>
        <h4>Explore</h4>
        <a href="#men">Men's Team</a>
        <a href="#women">Women's Team</a>
        <a href="#stats">Goals &amp; Statistics</a>
        <a href="#matches">Fixtures &amp; Results</a>
        <a href="#gallery">Gallery</a>
      </div>
      <div>
        <h4>Club</h4>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
        <a href="#admin">Admin Dashboard</a>
      </div>
      <div>
        <h4>Get in touch</h4>
        <a href="mailto:info@imanimarianistsctc.org">info@imanimarianistsctc.org</a>
        <a href="tel:+254700000000">+254 700 000 000</a>
        <p>Nairobi, Kenya</p>
      </div>
    </div>
    <div class="foot-bottom">
      <span>© <span id="year"></span> Imani Marianists CTC Sports Football Team. All rights reserved.</span>
      <span>Placeholder content — update via the Admin Dashboard.</span>
    </div>
  </div>
</footer>

<script>
/* ============================================================
   1. DATA LAYER  (localStorage "database")
============================================================ */
const STORAGE_KEY = 'imani_ctc_football_v1';
const POSITIONS = ['Goalkeeper','Defender','Midfielder','Forward'];
const GAL_CATS = ['Team','Training','Men','Women','Match Day','Awards'];

function uid(){ return Math.random().toString(36).slice(2,10); }
function esc(v){
  return String(v === null || v === undefined ? '' : v)
    .replace(/[&<>"']/g, c => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[c]));
}
function iso(offset){
  const d = new Date();
  d.setDate(d.getDate() + (offset||0));
  return d.toISOString().slice(0,10);
}
function fmtDate(str){
  if(!str) return 'To be confirmed';
  const d = new Date(str + 'T00:00:00');
  if(isNaN(d)) return esc(str);
  return d.toLocaleDateString('en-GB',{day:'numeric',month:'short',year:'numeric'});
}

const SIL = '<svg class="sil" viewBox="0 0 100 100" aria-hidden="true"><circle cx="50" cy="32" r="17"/><path d="M50 54c-17.6 0-29 11.6-29 27.2V100h58V81.2C79 65.6 67.6 54 50 54z"/></svg>';

/* ---------- Seed (all placeholder, no invented names or stats) ---------- */
function makeSquad(squad){
  const plan = [['Goalkeeper',2],['Defender',4],['Midfielder',4],['Forward',3]];
  const out = [];
  let num = 1;
  plan.forEach(([pos, qty]) => {
    for(let i=0;i<qty;i++){
      out.push({
        id: uid(), squad, name: 'Player Name ' + String(num).padStart(2,'0'),
        number: num, position: pos, age: '', nationality: 'Kenya',
        matches: 0, goals: 0, assists: 0, yellow: 0, red: 0,
        bio: 'Player biography coming soon. This is placeholder information — an administrator can update the full profile, photograph and statistics from the Admin Dashboard.',
        photo: ''
      });
      num++;
    }
  });
  return out;
}

function seed(){
  return {
    settings: { heroImage: '', adminPass: 'imani2024' },
    players: [...makeSquad('men'), ...makeSquad('women')],
    matches: [
      { id:uid(), squad:'men', status:'upcoming', opponent:'Opponent To Be Announced', date:iso(7),  time:'15:00', venue:'Imani Marianists Grounds', home:true,  goalsFor:null, goalsAgainst:null, scorers:'', report:'' },
      { id:uid(), squad:'women', status:'upcoming', opponent:'Opponent To Be Announced', date:iso(10), time:'13:00', venue:'Imani Marianists Grounds', home:true,  goalsFor:null, goalsAgainst:null, scorers:'', report:'' },
      { id:uid(), squad:'men', status:'upcoming', opponent:'Opponent To Be Announced', date:iso(18), time:'16:00', venue:'Away Ground', home:false, goalsFor:null, goalsAgainst:null, scorers:'', report:'' },
      { id:uid(), squad:'women', status:'upcoming', opponent:'Opponent To Be Announced', date:iso(24), time:'15:00', venue:'Away Ground', home:false, goalsFor:null, goalsAgainst:null, scorers:'', report:'' }
    ],
    gallery: GAL_CATS.map(cat => ({ id:uid(), title:'Photo title placeholder', category:cat, image:'' })).slice(0,6),
    news: [
      { id:uid(), date:iso(-2), title:'Pre-season training resumes for both squads', body:'The men\'s and women\'s squads have returned to the training ground ahead of the new campaign. Full schedule details will be shared with players and supporters shortly.' },
      { id:uid(), date:iso(-9), title:'Supporters welcome at Imani Marianists Grounds', body:'Fans are invited to attend our next home fixture. Entry arrangements and kick-off times will be confirmed closer to match day.' },
      { id:uid(), date:iso(-16), title:'Club announces new football development programme', body:'A structured pathway for young players from the community is being introduced, focusing on skills, discipline and teamwork.' }
    ]
  };
}

let DB;
function load(){
  try{
    const raw = localStorage.getItem(STORAGE_KEY);
    if(raw){
      const parsed = JSON.parse(raw);
      if(parsed && parsed.players) return parsed;
    }
  }catch(e){ console.warn('Could not read saved data', e); }
  const fresh = seed();
  try{ localStorage.setItem(STORAGE_KEY, JSON.stringify(fresh)); }catch(e){}
  return fresh;
}
function save(){
  try{ localStorage.setItem(STORAGE_KEY, JSON.stringify(DB)); }
  catch(e){ alert('Storage limit reached. Please try smaller images or remove some photos.'); }
}
DB = load();

/* ============================================================
   2. HELPERS
============================================================ */
const state = {
  statsSquad: 'men',
  matchFilter: 'all',
  galFilter: 'all',
  adminTab: 'players',
  adminSquad: 'men',
  editing: null,
  pendingPhoto: undefined
};

function isAdmin(){ return sessionStorage.getItem('imani_admin') === '1'; }
function setAdmin(v){ v ? sessionStorage.setItem('imani_admin','1') : sessionStorage.removeItem('imani_admin'); }

function squadPlayers(squad){ return DB.players.filter(p => p.squad === squad); }
function totalGoals(squad){ return squadPlayers(squad).reduce((s,p) => s + (+p.goals||0), 0); }
function totalAssists(squad){ return squadPlayers(squad).reduce((s,p) => s + (+p.assists||0), 0); }
function totalApps(squad){ return squadPlayers(squad).reduce((s,p) => s + (+p.matches||0), 0); }
function squadName(squad){ return squad === 'men' ? "Men's Team" : "Women's Team"; }
function getPlayer(id){ return DB.players.find(p => p.id === id); }

function playerOfMonth(squad){
  const list = squadPlayers(squad).filter(p => (p.goals + p.assists) > 0);
  if(!list.length) return null;
  return list.sort((a,b) => (b.goals + b.assists) - (a.goals + a.assists) || b.goals - a.goals)[0];
}

function initials(name){
  return String(name||'?').split(/\s+/).filter(Boolean).slice(0,2).map(w => w[0]).join('').toUpperCase();
}

/* ============================================================
   3. REUSABLE COMPONENTS
============================================================ */
function playerCard(p){
  const cls = p.squad === 'women' ? 'women' : '';
  return `
  <article class="p-card">
    <div class="p-card-photo ${cls}">
      ${p.photo ? `<img src="${p.photo}" alt="${esc(p.name)}">` : SIL}
      <span class="p-num">#${esc(p.number)}</span>
      <span class="p-pos">${esc(p.position)}</span>
    </div>
    <div class="p-card-body">
      <h3 class="p-name">${esc(p.name)}</h3>
      <p class="p-meta">${p.age ? esc(p.age) + ' yrs · ' : ''}${esc(p.nationality || 'Nationality TBC')}</p>
      <div class="p-mini">
        <div><b>${p.matches||0}</b><span>Apps</span></div>
        <div><b>${p.goals||0}</b><span>Goals</span></div>
        <div><b>${p.assists||0}</b><span>Assists</span></div>
      </div>
      <a class="btn btn-sm btn-green" href="#player/${p.id}">View Profile</a>
    </div>
  </article>`;
}

function leaderboard(title, rows, unit, green){
  const body = rows.length
    ? rows.map((r,i) => `
        <div class="lb-row">
          <span class="lb-rank ${i===0?'r1':i===1?'r2':i===2?'r3':''}">${i+1}</span>
          <span class="lb-name">${esc(r.name)}<small>#${esc(r.number)} · ${esc(r.position)}</small></span>
          <span class="lb-val">${r.value}<small style="font-weight:700;font-size:.7rem;color:var(--muted)"> ${unit}</small></span>
        </div>`).join('')
    : `<div class="lb-empty">No ${unit.toLowerCase()} recorded yet. Statistics appear here once updated in the Admin Dashboard.</div>`;
  return `<div class="lb"><div class="lb-head ${green?'green':''}">${esc(title)}</div>${body}</div>`;
}

function statBox(value, label, colour){
  return `<div class="stat-box ${colour||''}"><b>${value}</b><span>${label}</span></div>`;
}

/* ============================================================
   4. PAGES
============================================================ */
function renderHome(){
  const news = DB.news.slice().sort((a,b) => String(b.date).localeCompare(String(a.date))).slice(0,3);
  const upcoming = DB.matches.filter(m => m.status === 'upcoming').sort((a,b)=>String(a.date).localeCompare(String(b.date))).slice(0,2);
  return `
  <section class="hero">
    <div class="hero-bg" ${DB.settings.heroImage ? `style="background-image:url('${DB.settings.heroImage}')"` : ''}></div>
    <div class="hero-inner wrap">
      <p class="hero-kicker">⚽ CTC Sports · Football</p>
      <h1 class="hero-title">IMANI MARIANISTS</h1>
      <p class="hero-tag">One Team. One Dream. One Family.</p>
      <p class="hero-sub">The official home of the Imani Marianists CTC Sports Football Team — men's and women's squads, player statistics, fixtures, results and everything happening around the club.</p>
      <div class="hero-cta">
        <a class="btn btn-yellow" href="#men">Men's Team</a>
        <a class="btn btn-outline" href="#women">Women's Team</a>
        <a class="btn btn-outline" href="#matches">Fixtures &amp; Results</a>
      </div>
      <div class="hero-strip">
        <div><b>${squadPlayers('men').length}</b><span>Men's Players</span></div>
        <div><b>${squadPlayers('women').length}</b><span>Women's Players</span></div>
        <div><b>${totalGoals('men') + totalGoals('women')}</b><span>Total Goals</span></div>
        <div><b>${DB.matches.filter(m=>m.status==='upcoming').length}</b><span>Upcoming Fixtures</span></div>
      </div>
    </div>
  </section>

  <div class="wrap page">

    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Quick Links</span>
          <h2 class="sec-title">Explore the <em>club</em></h2>
        </div>
      </div>
      <div class="grid-auto quick-grid">
        <a class="quick-card" href="#men"><span class="ico">🔴</span><b>Men's Team</b><small>Squad &amp; profiles</small></a>
        <a class="quick-card" href="#women"><span class="ico">🟢</span><b>Women's Team</b><small>Squad &amp; profiles</small></a>
        <a class="quick-card" href="#players"><span class="ico">👥</span><b>Players</b><small>Search all players</small></a>
        <a class="quick-card" href="#stats"><span class="ico">📊</span><b>Goals &amp; Stats</b><small>Leaderboards</small></a>
        <a class="quick-card" href="#matches"><span class="ico">📅</span><b>Matches</b><small>Fixtures &amp; results</small></a>
      </div>
    </section>

    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Latest</span>
          <h2 class="sec-title">Team <em>news</em> &amp; announcements</h2>
        </div>
        <a class="btn btn-sm btn-ghost" href="#about">About the club</a>
      </div>
      <div class="news-grid">
        ${news.length ? news.map(n => `
          <article class="news-card">
            <span class="news-date">${fmtDate(n.date)}</span>
            <h3>${esc(n.title)}</h3>
            <p>${esc(n.body)}</p>
          </article>`).join('') : '<div class="empty">No news published yet.</div>'}
      </div>
    </section>

    ${upcoming.length ? `
    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Next Up</span>
          <h2 class="sec-title">Upcoming <em>fixtures</em></h2>
        </div>
        <a class="btn btn-sm btn-ghost" href="#matches">All matches</a>
      </div>
      <div class="match-grid">${upcoming.map(matchCard).join('')}</div>
    </section>` : ''}

  </div>`;
}

function renderSquadPage(squad){
  const list = squadPlayers(squad).sort((a,b) => (+a.number||0) - (+b.number||0));
  const other = squad === 'men' ? 'women' : 'men';
  return `
  <div class="wrap page">
    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">${squad === 'men' ? '🔴 Red Squad' : '🟢 Green Squad'}</span>
          <h2 class="sec-title">${squadName(squad)} <em>squad</em></h2>
          <p class="sec-sub">Meet the players representing Imani Marianists CTC Sports. Tap any player card to open the full profile and statistics.</p>
        </div>
        <a class="btn btn-sm btn-ghost" href="#${other}">Switch to ${squadName(other)}</a>
      </div>

      <div class="toolbar">
        <div class="search">
          <input type="search" id="playerSearch" data-squad="${squad}" placeholder="Search by name, number, position…" aria-label="Search players">
        </div>
        <div class="seg">
          <button class="${squad==='men'?'on':''}" data-act="go" data-href="#men">Men</button>
          <button class="${squad==='women'?'on green':''}" data-act="go" data-href="#women">Women</button>
        </div>
      </div>

      <div class="p-grid" id="playerGrid">
        ${list.length ? list.map(playerCard).join('') : '<div class="empty">No players added to this squad yet.</div>'}
      </div>
    </section>
  </div>`;
}

function renderPlayersPage(){
  const list = DB.players.slice().sort((a,b) => a.name.localeCompare(b.name));
  return `
  <div class="wrap page">
    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">All Players</span>
          <h2 class="sec-title">Player <em>directory</em></h2>
          <p class="sec-sub">Search across both the men's and women's squads.</p>
        </div>
      </div>
      <div class="toolbar">
        <div class="search">
          <input type="search" id="playerSearch" data-squad="" placeholder="Search all players…" aria-label="Search all players">
        </div>
        <span class="badge men">${squadPlayers('men').length} Men</span>
        <span class="badge women">${squadPlayers('women').length} Women</span>
      </div>
      <div class="p-grid" id="playerGrid">
        ${list.length ? list.map(playerCard).join('') : '<div class="empty">No players yet.</div>'}
      </div>
    </section>
  </div>`;
}

function renderProfile(id){
  const p = getPlayer(id);
  if(!p){
    return `<div class="wrap page"><div class="empty">Player not found. <a href="#players" style="color:var(--red);font-weight:800">Back to players</a></div></div>`;
  }
  const cls = p.squad === 'women' ? 'women' : '';
  return `
  <div class="wrap page">
    <p style="margin:0 0 1rem"><a href="#${p.squad}" style="font-size:.82rem;font-weight:800;color:var(--green)">← Back to ${squadName(p.squad)}</a></p>
    <div class="profile">
      <div class="profile-photo ${cls}">
        ${p.photo ? `<img src="${p.photo}" alt="${esc(p.name)}">` : SIL}
        <span class="profile-num">#${esc(p.number)}</span>
      </div>
      <div>
        <span class="badge ${p.squad}" style="margin-bottom:.5rem">${squadName(p.squad)}</span>
        <h1 style="margin:.2rem 0 .3rem;font-size:clamp(1.5rem,4vw,2.1rem)">${esc(p.name)}</h1>
        <p style="margin:0;color:var(--muted);font-size:.9rem">
          <strong style="color:var(--red)">${esc(p.position)}</strong>
          ${p.age ? ' · ' + esc(p.age) + ' years' : ''}
          ${p.nationality ? ' · ' + esc(p.nationality) : ''}
        </p>

        <div class="stat-grid">
          ${statBox(p.matches||0,'Matches','')}
          ${statBox(p.goals||0,'Goals','red')}
          ${statBox(p.assists||0,'Assists','blue')}
          ${statBox(p.yellow||0,'Yellow','yellow')}
          ${statBox(p.red||0,'Red','red')}
        </div>

        <div class="card" style="margin-top:1.2rem">
          <h3 style="margin-top:0;font-size:1rem">Player Biography</h3>
          <p style="margin:0;color:var(--muted);font-size:.9rem">${esc(p.bio || 'Biography not provided yet.')}</p>
        </div>
      </div>
    </div>
  </div>`;
}

function renderStats(){
  const squad = state.statsSquad;
  const players = squadPlayers(squad);

  const scorers = players.filter(p => p.goals > 0)
    .sort((a,b) => b.goals - a.goals).slice(0,6)
    .map(p => ({name:p.name, number:p.number, position:p.position, value:p.goals}));

  const assists = players.filter(p => p.assists > 0)
    .sort((a,b) => b.assists - a.assists).slice(0,6)
    .map(p => ({name:p.name, number:p.number, position:p.position, value:p.assists}));

  const apps = players.filter(p => p.matches > 0)
    .sort((a,b) => b.matches - a.matches).slice(0,6)
    .map(p => ({name:p.name, number:p.number, position:p.position, value:p.matches}));

  const potm = playerOfMonth(squad);

  return `
  <div class="wrap page">
    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Statistics</span>
          <h2 class="sec-title">Goals &amp; <em>statistics</em></h2>
          <p class="sec-sub">Leaderboards are generated automatically from player statistics stored in the club database.</p>
        </div>
        <div class="seg">
          <button class="${squad==='men'?'on':''}" data-act="stats-squad" data-squad="men">Men</button>
          <button class="${squad==='women'?'on green':''}" data-act="stats-squad" data-squad="women">Women</button>
        </div>
      </div>

      <div class="stat-grid" style="margin-bottom:1.2rem">
        ${statBox(totalGoals(squad), 'Team Goals', 'red')}
        ${statBox(totalAssists(squad), 'Total Assists', 'blue')}
        ${statBox(totalApps(squad), 'Appearances', '')}
        ${statBox(players.length, 'Squad Size', 'yellow')}
      </div>

      ${potm ? `
      <div class="potm" style="margin-bottom:1.2rem">
        <div class="avatar">${esc(initials(potm.name))}</div>
        <div>
          <h4>${esc(potm.name)}</h4>
          <p>#${esc(potm.number)} · ${esc(potm.position)} — ${potm.goals} goals, ${potm.assists} assists</p>
        </div>
        <span class="tag">Player of the Month</span>
      </div>` : `
      <div class="potm" style="margin-bottom:1.2rem">
        <div class="avatar">★</div>
        <div><h4>Player of the Month</h4><p>Not yet selected — statistics will determine this once matches are played.</p></div>
      </div>`}

      <div class="two-col">
        ${leaderboard('Top Goal Scorers', scorers, 'goals', false)}
        ${leaderboard('Assists Leaders', assists, 'assists', true)}
        ${leaderboard('Most Appearances', apps, 'apps', false)}
      </div>
    </section>
  </div>`;
}

function matchCard(m){
  const played = m.status === 'played';
  const badge = played ? '<span class="badge done">Full Time</span>' : '<span class="badge up">Upcoming</span>';
  const score = played
    ? `<span class="score">${m.goalsFor ?? 0} - ${m.goalsAgainst ?? 0}</span>`
    : `<span class="score vs">VS</span>`;
  return `
  <article class="match">
    <div class="match-top">
      ${badge}
      <span class="badge ${m.squad}">${m.squad === 'men' ? 'Men' : 'Women'}</span>
    </div>
    <div class="match-teams">
      <div class="tn">Imani Marianists</div>
      ${score}
      <div class="tn right">${esc(m.opponent || 'TBA')}</div>
    </div>
    <div class="match-meta">
      <div>📅 <b>${fmtDate(m.date)}</b>${m.time ? ' · ' + esc(m.time) : ''}</div>
      <div>📍 ${esc(m.venue || 'Venue TBC')} · ${m.home ? 'Home' : 'Away'}</div>
      ${played && m.scorers ? `<div style="margin-top:.35rem">⚽ <b>Scorers:</b> ${esc(m.scorers)}</div>` : ''}
    </div>
    ${m.report ? `<p class="match-report">${esc(m.report)}</p>` : ''}
  </article>`;
}

function renderMatches(){
  const f = state.matchFilter;
  const filter = m => f === 'all' || m.squad === f;
  const upcoming = DB.matches.filter(m => m.status === 'upcoming' && filter(m))
    .sort((a,b) => String(a.date).localeCompare(String(b.date)));
  const results = DB.matches.filter(m => m.status === 'played' && filter(m))
    .sort((a,b) => String(b.date).localeCompare(String(a.date)));

  return `
  <div class="wrap page">
    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Fixtures</span>
          <h2 class="sec-title">Upcoming <em>matches</em></h2>
        </div>
        <div class="seg">
          <button class="${f==='all'?'on':''}" data-act="match-filter" data-f="all">All</button>
          <button class="${f==='men'?'on':''}" data-act="match-filter" data-f="men">Men</button>
          <button class="${f==='women'?'on green':''}" data-act="match-filter" data-f="women">Women</button>
        </div>
      </div>
      <div class="match-grid">
        ${upcoming.length ? upcoming.map(matchCard).join('') : '<div class="empty">No upcoming fixtures scheduled yet. Add them in the Admin Dashboard.</div>'}
      </div>
    </section>

    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Results</span>
          <h2 class="sec-title">Previous <em>matches</em></h2>
        </div>
      </div>
      <div class="match-grid">
        ${results.length ? results.map(matchCard).join('') : '<div class="empty">No results recorded yet. Match results added in the Admin Dashboard will appear here.</div>'}
      </div>
    </section>
  </div>`;
}

function renderGallery(){
  const cats = ['all', ...GAL_CATS];
  const list = DB.gallery.filter(g => state.galFilter === 'all' || g.category === state.galFilter);
  return `
  <div class="wrap page">
    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Gallery</span>
          <h2 class="sec-title">Team <em>gallery</em></h2>
          <p class="sec-sub">Team photographs, training sessions, match-day moments, celebrations and awards.</p>
        </div>
      </div>
      <div class="tabs" style="margin-bottom:1.2rem">
        ${cats.map(c => `<button class="${state.galFilter===c?'on':''}" data-act="gal-filter" data-f="${c}">${c === 'all' ? 'All Photos' : c}</button>`).join('')}
      </div>
      <div class="gal-grid">
        ${list.length ? list.map(g => `
          <figure class="gal-item" style="margin:0">
            ${g.image ? `<img src="${g.image}" alt="${esc(g.title)}">` : '<span class="ph">📷</span>'}
            <figcaption class="gal-cap">${esc(g.title)}<small>${esc(g.category)}</small></figcaption>
          </figure>`).join('') : '<div class="empty">No photos in this category yet.</div>'}
      </div>
    </section>
  </div>`;
}

function renderAbout(){
  return `
  <div class="wrap page">
    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">About Us</span>
          <h2 class="sec-title">Who we <em>are</em></h2>
        </div>
      </div>
      <div class="card prose">
        <h3>Our History</h3>
        <p>Imani Marianists CTC Sports is a community football club built around faith, discipline and a shared love of the game. What began as a small group of players training together has grown into a club fielding both men's and women's football teams, supported by coaches, volunteers and a proud community of supporters.</p>
        <p>This website is the club's official platform — a place to follow the squads, track statistics, keep up with fixtures and celebrate the achievements of our players.</p>
      </div>
    </section>

    <section class="sec">
      <div class="two-col">
        <div class="card prose">
          <h3>Our Mission</h3>
          <p>To develop talented, disciplined and confident footballers, giving young people from our community a positive environment in which to grow — on and off the pitch.</p>
        </div>
        <div class="card prose">
          <h3>Our Vision</h3>
          <p>To be a respected football club recognised for developing home-grown talent, competing with integrity and representing our community with pride.</p>
        </div>
      </div>
    </section>

    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Values</span>
          <h2 class="sec-title">What we <em>stand for</em></h2>
        </div>
      </div>
      <div class="value-grid">
        <div class="value"><h4>Teamwork</h4><p>One team. One dream. One family. We win and lose together.</p></div>
        <div class="value"><h4>Discipline</h4><p>Commitment to training, punctuality and respect for coaches, opponents and officials.</p></div>
        <div class="value"><h4>Respect</h4><p>Fair play on the pitch and integrity in everything we do as a club.</p></div>
        <div class="value"><h4>Growth</h4><p>A clear pathway for young players to develop their skills and confidence.</p></div>
      </div>
    </section>

    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Achievements</span>
          <h2 class="sec-title">Club <em>milestones</em></h2>
        </div>
      </div>
      <ul class="timeline">
        <li><b>Year</b><span>Achievement placeholder — add tournament wins, league positions and honours here.</span></li>
        <li><b>Year</b><span>Achievement placeholder — record appearances, top scorer awards or community recognition.</span></li>
        <li><b>Year</b><span>Achievement placeholder — youth team progress and player development milestones.</span></li>
      </ul>
    </section>

    <section class="sec">
      <div class="card prose" style="border-left:5px solid var(--yellow)">
        <h3 style="margin-bottom:.4rem">Talent Development</h3>
        <p style="margin:0">We are committed to developing football talent at every level. Our coaching programme focuses on technical skill, tactical understanding, physical conditioning and personal character — helping every player reach their potential while staying rooted in the values of the club.</p>
      </div>
    </section>
  </div>`;
}

function renderContact(){
  return `
  <div class="wrap page">
    <section class="sec">
      <div class="sec-head">
        <div>
          <span class="eyebrow">Contact</span>
          <h2 class="sec-title">Get in <em>touch</em></h2>
          <p class="sec-sub">For fixtures, trials, sponsorship or general enquiries, reach out to the club.</p>
        </div>
      </div>
      <div class="contact-grid">
        <div class="contact-card"><span class="ico">✉️</span><div><b>Email</b><span>info@imanimarianistsctc.org</span></div></div>
        <div class="contact-card"><span class="ico">📞</span><div><b>Phone</b><span>+254 700 000 000</span></div></div>
        <div class="contact-card"><span class="ico">📍</span><div><b>Location</b><span>Imani Marianists CTC Grounds, Nairobi, Kenya</span></div></div>
        <div class="contact-card"><span class="ico">🕒</span><div><b>Training</b><span>Tue &amp; Thu · 4:00 PM – 6:00 PM</span></div></div>
      </div>

      <div class="socials">
        <a href="#" onclick="return false">Facebook</a>
        <a href="#" onclick="return false">X / Twitter</a>
        <a href="#" onclick="return false">Instagram</a>
        <a href="#" onclick="return false">YouTube</a>
      </div>
    </section>

    <section class="sec">
      <div class="card">
        <h3 style="margin-top:0">Send us a message</h3>
        <form class="form-grid" data-form="contact">
          <label>Your Name<input name="name" required placeholder="Full name"></label>
          <label>Email<input name="email" type="email" required placeholder="you@example.com"></label>
          <label class="full">Message<textarea name="message" rows="4" required placeholder="How can we help?"></textarea></label>
          <div class="form-actions"><button class="btn btn-red" type="submit">Send Message</button></div>
        </form>
      </div>
    </section>
  </div>`;
}

/* ============================================================
   5. ADMIN DASHBOARD
============================================================ */
function renderAdmin(){
  if(!isAdmin()){
    return `
    <div class="wrap page">
      <div class="card gate">
        <h2 style="margin-top:0">Administrator Login</h2>
        <p style="color:var(--muted);font-size:.86rem;margin-top:0">Sign in to manage squads, statistics, matches, gallery and news.</p>
        <form data-form="login" class="form-grid" style="grid-template-columns:1fr">
          <label>Password<input type="password" name="pass" required placeholder="Enter admin password"></label>
          <div class="form-actions"><button class="btn btn-red btn-block" type="submit">Sign In</button></div>
        </form>
        <p class="hint">Demo password: <code>imani2024</code> (change it in Settings after logging in).</p>
      </div>
    </div>`;
  }

  const tabs = [['players','Players'],['matches','Matches'],['gallery','Gallery'],['news','News'],['settings','Settings']];
  let body = '';
  if(state.adminTab === 'players') body = adminPlayers();
  if(state.adminTab === 'matches') body = adminMatches();
  if(state.adminTab === 'gallery') body = adminGallery();
  if(state.adminTab === 'news') body = adminNews();
  if(state.adminTab === 'settings') body = adminSettings();

  return `
  <div class="wrap page">
    <div class="admin-head">
      <div>
        <h2>Admin Dashboard</h2>
        <p>Manage Imani Marianists CTC Sports Football Team</p>
      </div>
      <button class="btn btn-yellow btn-sm" data-act="logout">Sign Out</button>
    </div>
    <div class="tabs">
      ${tabs.map(([k,label]) => `<button class="${state.adminTab===k?'on':''}" data-act="admin-tab" data-tab="${k}">${label}</button>`).join('')}
    </div>
    ${body}
  </div>`;
}

function adminPlayers(){
  const squad = state.adminSquad;
  const list = squadPlayers(squad).sort((a,b) => (+a.number||0) - (+b.number||0));
  return `
  <div class="admin-bar">
    <div class="seg">
      <button class="${squad==='men'?'on':''}" data-act="admin-squad" data-squad="men">Men's Squad</button>
      <button class="${squad==='women'?'on green':''}" data-act="admin-squad" data-squad="women">Women's Squad</button>
    </div>
    <button class="btn btn-red btn-sm" data-act="adm-new">+ Add New Player</button>
  </div>

  ${state.editing ? playerForm(state.editing) : ''}

  <div class="adm-list">
    ${list.length ? list.map(p => `
      <div class="adm-row">
        <div class="adm-avatar ${p.squad==='women'?'women':''}">
          ${p.photo ? `<img src="${p.photo}" alt="">` : esc(p.number)}
        </div>
        <div class="adm-info">
          <b>${esc(p.name)}</b>
          <small>#${esc(p.number)} · ${esc(p.position)} · ${p.goals||0}G ${p.assists||0}A ${p.matches||0}Apps</small>
        </div>
        <div class="adm-actions">
          <button class="btn btn-sm btn-ghost" data-act="adm-edit" data-id="${p.id}">Edit</button>
          <button class="btn btn-sm btn-red" data-act="adm-del" data-id="${p.id}">Delete</button>
        </div>
      </div>`).join('') : '<div class="empty">No players in this squad yet.</div>'}
  </div>`;
}

function playerForm(p){
  const isNew = !p.id;
  return `
  <form class="card form-grid" data-form="player" style="margin-bottom:1.2rem">
    <input type="hidden" name="id" value="${esc(p.id||'')}">
    <div class="form-head">
      <h3>${isNew ? 'Add New Player' : 'Edit Player'}</h3>
      <button type="button" class="btn btn-sm btn-ghost" data-act="adm-cancel">Cancel</button>
    </div>
    <div class="photo-row">
      <div class="photo-prev" id="photoPreview">${p.photo ? `<img src="${p.photo}" alt="">` : SIL}</div>
      <div>
        <label class="btn btn-sm btn-ghost file-btn" style="display:inline-flex;text-transform:none;letter-spacing:0;font-size:.78rem">
          Upload Player Photo
          <input type="file" accept="image/*" data-upload="player-photo" hidden>
        </label>
        <p class="hint">JPG or PNG. Images are automatically resized.</p>
      </div>
    </div>
    <label>Full Name<input name="name" value="${esc(p.name)}" required></label>
    <label>Jersey Number<input name="number" type="number" min="1" max="99" value="${esc(p.number)}" required></label>
    <label>Playing Position
      <select name="position">
        ${POSITIONS.map(x => `<option ${x===p.position?'selected':''}>${x}</option>`).join('')}
      </select>
    </label>
    <label>Age<input name="age" type="number" min="8" max="60" value="${esc(p.age)}"></label>
    <label>Nationality<input name="nationality" value="${esc(p.nationality)}"></label>
    <label>Matches Played<input name="matches" type="number" min="0" value="${esc(p.matches||0)}"></label>
    <label>Goals Scored<input name="goals" type="number" min="0" value="${esc(p.goals||0)}"></label>
    <label>Assists<input name="assists" type="number" min="0" value="${esc(p.assists||0)}"></label>
    <label>Yellow Cards<input name="yellow" type="number" min="0" value="${esc(p.yellow||0)}"></label>
    <label>Red Cards<input name="red" type="number" min="0" value="${esc(p.red||0)}"></label>
    <label class="full">Short Biography<textarea name="bio" rows="3">${esc(p.bio)}</textarea></label>
    <div class="form-actions">
      <button class="btn btn-red" type="submit">${isNew ? 'Add Player' : 'Save Changes'}</button>
      <button type="button" class="btn btn-ghost" data-act="adm-cancel">Cancel</button>
    </div>
  </form>`;
}

function adminMatches(){
  const list = DB.matches.slice().sort((a,b) => String(b.date).localeCompare(String(a.date)));
  return `
  <div class="card" style="margin-bottom:1.2rem">
    <h3 style="margin-top:0">Add / Update Match</h3>
    <form class="form-grid" data-form="match">
      <label>Squad
        <select name="squad"><option value="men">Men's Team</option><option value="women">Women's Team</option></select>
      </label>
      <label>Status
        <select name="status"><option value="upcoming">Upcoming Fixture</option><option value="played">Played (Result)</option></select>
      </label>
      <label>Opponent<input name="opponent" required placeholder="Opponent name"></label>
      <label>Date<input name="date" type="date" required value="${iso(7)}"></label>
      <label>Kick-off Time<input name="time" placeholder="15:00"></label>
      <label>Venue<input name="venue" placeholder="Ground name"></label>
      <label>Home / Away
        <select name="home"><option value="true">Home</option><option value="false">Away</option></select>
      </label>
      <label>Goals For<input name="goalsFor" type="number" min="0" placeholder="—"></label>
      <label>Goals Against<input name="goalsAgainst" type="number" min="0" placeholder="—"></label>
      <label class="full">Goal Scorers<input name="scorers" placeholder="e.g. Player Name 09 (2), Player Name 11"></label>
      <label class="full">Match Report<textarea name="report" rows="3" placeholder="Short match report…"></textarea></label>
      <div class="form-actions"><button class="btn btn-red" type="submit">Save Match</button></div>
    </form>
  </div>

  <div class="adm-list">
    ${list.length ? list.map(m => `
      <div class="adm-row">
        <div class="adm-avatar ${m.squad==='women'?'women':''}">${m.squad==='men'?'M':'W'}</div>
        <div class="adm-info">
          <b>Imani Marianists vs ${esc(m.opponent)}</b>
          <small>${fmtDate(m.date)} · ${m.status==='played' ? `Result ${m.goalsFor ?? 0}-${m.goalsAgainst ?? 0}` : 'Upcoming'} · ${esc(m.venue||'Venue TBC')}</small>
        </div>
        <div class="adm-actions">
          <button class="btn btn-sm btn-red" data-act="match-del" data-id="${m.id}">Delete</button>
        </div>
      </div>`).join('') : '<div class="empty">No matches added yet.</div>'}
  </div>`;
}

function adminGallery(){
  return `
  <div class="card" style="margin-bottom:1.2rem">
    <h3 style="margin-top:0">Upload Team Photograph</h3>
    <form class="form-grid" data-form="gallery">
      <label>Photo Title<input name="title" required placeholder="e.g. Match day squad"></label>
      <label>Category
        <select name="category">${GAL_CATS.map(c => `<option>${c}</option>`).join('')}</select>
      </label>
      <label class="full">Image File<input type="file" accept="image/*" name="file" data-upload="gallery-photo" required></label>
      <div class="form-actions"><button class="btn btn-red" type="submit">Upload Photo</button></div>
    </form>
    <p class="hint">Tip: photos are stored in your browser's local storage. Use reasonably sized images.</p>
  </div>

  <div class="adm-list">
    ${DB.gallery.length ? DB.gallery.map(g => `
      <div class="adm-row">
        <div class="adm-avatar" style="background:#111">
          ${g.image ? `<img src="${g.image}" alt="">` : '📷'}
        </div>
        <div class="adm-info"><b>${esc(g.title)}</b><small>${esc(g.category)}</small></div>
        <div class="adm-actions"><button class="btn btn-sm btn-red" data-act="gal-del" data-id="${g.id}">Delete</button></div>
      </div>`).join('') : '<div class="empty">Gallery is empty.</div>'}
  </div>`;
}

function adminNews(){
  return `
  <div class="card" style="margin-bottom:1.2rem">
    <h3 style="margin-top:0">Publish Announcement</h3>
    <form class="form-grid" data-form="news">
      <label>Title<input name="title" required placeholder="Announcement title"></label>
      <label>Date<input name="date" type="date" required value="${iso(0)}"></label>
      <label class="full">Message<textarea name="body" rows="3" required placeholder="Announcement details…"></textarea></label>
      <div class="form-actions"><button class="btn btn-red" type="submit">Publish</button></div>
    </form>
  </div>

  <div class="adm-list">
    ${DB.news.length ? DB.news.slice().sort((a,b)=>String(b.date).localeCompare(String(a.date))).map(n => `
      <div class="adm-row">
        <div class="adm-info"><b>${esc(n.title)}</b><small>${fmtDate(n.date)} · ${esc(String(n.body).slice(0,90))}…</small></div>
        <div class="adm-actions"><button class="btn btn-sm btn-red" data-act="news-del" data-id="${n.id}">Delete</button></div>
      </div>`).join('') : '<div class="empty">No announcements yet.</div>'}
  </div>`;
}

function adminSettings(){
  return `
  <div class="two-col">
    <div class="card">
      <h3 style="margin-top:0">Hero Banner Image</h3>
      <form class="form-grid" data-form="hero">
        <label class="full">Team Photograph<input type="file" accept="image/*" name="file" data-upload="hero-photo" required></label>
        <div class="form-actions">
          <button class="btn btn-red" type="submit">Set Banner</button>
          ${DB.settings.heroImage ? '<button type="button" class="btn btn-ghost" data-act="hero-clear">Remove Banner</button>' : ''}
        </div>
      </form>
      <p class="hint">This image is used as the background of the homepage banner.</p>
    </div>

    <div class="card">
      <h3 style="margin-top:0">Change Admin Password</h3>
      <form class="form-grid" data-form="password">
        <label class="full">New Password<input type="password" name="pass" required minlength="4" placeholder="New password"></label>
        <div class="form-actions"><button class="btn btn-green" type="submit">Update Password</button></div>
      </form>
    </div>

    <div class="card">
      <h3 style="margin-top:0">Demo Statistics</h3>
      <p style="color:var(--muted);font-size:.85rem;margin-top:0">The site ships with zero statistics so nothing is invented. Use this button to preview the leaderboards with temporary sample numbers, or simply enter real statistics player by player.</p>
      <div class="form-actions">
        <button class="btn btn-ghost" data-act="fill-demo">Fill Demo Statistics</button>
        <button class="btn btn-ghost" data-act="clear-stats">Clear All Statistics</button>
      </div>
    </div>

    <div class="card">
      <h3 style="margin-top:0;color:var(--red)">Danger Zone</h3>
      <p style="color:var(--muted);font-size:.85rem;margin-top:0">Reset the entire website database back to its original placeholder state. This cannot be undone.</p>
      <button class="btn btn-red" data-act="reset-all">Reset All Data</button>
    </div>
  </div>`;
}

/* ============================================================
   6. ROUTER
============================================================ */
function router(scrollTop = true){
  const raw = (location.hash || '#home').replace(/^#\/?/, '');
  const parts = raw.split('/');
  const route = parts[0] || 'home';
  const param = parts[1] || '';

  let html = '';
  switch(route){
    case 'men':     html = renderSquadPage('men'); break;
    case 'women':   html = renderSquadPage('women'); break;
    case 'players': html = renderPlayersPage(); break;
    case 'player':  html = renderProfile(param); break;
    case 'stats':   html = renderStats(); break;
    case 'matches': html = renderMatches(); break;
    case 'gallery': html = renderGallery(); break;
    case 'about':   html = renderAbout(); break;
    case 'contact': html = renderContact(); break;
    case 'admin':   html = renderAdmin(); break;
    default:        html = renderHome();
  }

  document.getElementById('view').innerHTML = html;

  document.querySelectorAll('#nav a').forEach(a => {
    a.classList.toggle('active', a.getAttribute('href') === '#' + route);
  });

  document.getElementById('nav').classList.remove('open');
  document.getElementById('menuBtn').setAttribute('aria-expanded','false');
  if(scrollTop) window.scrollTo(0,0);
}

window.addEventListener('hashchange', () => router(true));

/* ============================================================
   7. IMAGE HANDLING
============================================================ */
function readImage(file, maxW = 700){
  return new Promise((resolve, reject) => {
    const reader = new FileReader();
    reader.onload = () => {
      const img = new Image();
      img.onload = () => {
        const scale = Math.min(1, maxW / img.width);
        const c = document.createElement('canvas');
        c.width = Math.round(img.width * scale);
        c.height = Math.round(img.height * scale);
        c.getContext('2d').drawImage(img, 0, 0, c.width, c.height);
        resolve(c.toDataURL('image/jpeg', 0.82));
      };
      img.onerror = reject;
      img.src = reader.result;
    };
    reader.onerror = reject;
    reader.readAsDataURL(file);
  });
}

/* ============================================================
   8. EVENTS
============================================================ */
document.getElementById('menuBtn').addEventListener('click', () => {
  const nav = document.getElementById('nav');
  const open = nav.classList.toggle('open');
  document.getElementById('menuBtn').setAttribute('aria-expanded', String(open));
});

/* live search */
document.addEventListener('input', e => {
  if(e.target.id === 'playerSearch'){
    const squad = e.target.dataset.squad;
    const q = e.target.value.trim().toLowerCase();
    const list = DB.players
      .filter(p => (!squad || p.squad === squad))
      .filter(p => !q || [p.name, p.number, p.position, p.nationality, p.squad]
        .join(' ').toLowerCase().includes(q))
      .sort((a,b) => (+a.number||0) - (+b.number||0));
    const grid = document.getElementById('playerGrid');
    if(grid) grid.innerHTML = list.length
      ? list.map(playerCard).join('')
      : '<div class="empty">No players match your search.</div>';
  }
});

/* photo uploads (live preview) */
document.addEventListener('change', async e => {
  const input = e.target;
  if(input.dataset.upload === 'player-photo' && input.files[0]){
    try{
      const data = await readImage(input.files[0], 500);
      state.pendingPhoto = data;
      const prev = document.getElementById('photoPreview');
      if(prev) prev.innerHTML = `<img src="${data}" alt="">`;
    }catch(err){ alert('Could not read that image.'); }
  }
  if(input.dataset.upload === 'gallery-photo' && input.files[0]){
    try{ state.pendingPhoto = await readImage(input.files[0], 900); }
    catch(err){ alert('Could not read that image.'); }
  }
  if(input.dataset.upload === 'hero-photo' && input.files[0]){
    try{ state.pendingPhoto = await readImage(input.files[0], 1400); }
    catch(err){ alert('Could not read that image.'); }
  }
});

/* clicks */
document.addEventListener('click', e => {
  const el = e.target.closest('[data-act]');
  if(!el) return;
  const act = el.dataset.act;

  if(act === 'go'){
    location.hash = el.dataset.href;
    return;
  }

  /* ---------- public filters ---------- */
  if(act === 'stats-squad'){
    state.statsSquad = el.dataset.squad;
    router(false);
    return;
  }
  if(act === 'match-filter'){
    state.matchFilter = el.dataset.f;
    router(false);
    return;
  }
  if(act === 'gal-filter'){
    state.galFilter = el.dataset.f;
    router(false);
    return;
  }

  /* ---------- admin ---------- */
  if(act === 'logout'){
    setAdmin(false);
    state.editing = null;
    location.hash = '#home';
    router(true);
    return;
  }
  if(act === 'admin-tab'){
    state.adminTab = el.dataset.tab;
    state.editing = null;
    router(false);
    return;
  }
  if(act === 'admin-squad'){
    state.adminSquad = el.dataset.squad;
    state.editing = null;
    router(false);
    return;
  }
  if(act === 'adm-new'){
    state.pendingPhoto = undefined;
    state.editing = {
      id:'', squad: state.adminSquad, name:'', number:'', position:'Defender',
      age:'', nationality:'Kenya', matches:0, goals:0, assists:0,
      yellow:0, red:0, bio:'', photo:''
    };
    router(false);
    return;
  }
  if(act === 'adm-edit'){
    const p = getPlayer(el.dataset.id);
    if(p){
      state.pendingPhoto = undefined;
      state.editing = Object.assign({}, p);
      router(false);
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }
    return;
  }
  if(act === 'adm-cancel'){
    state.editing = null;
    state.pendingPhoto = undefined;
    router(false);
    return;
  }
  if(act === 'adm-del'){
    if(confirm('Remove this player from the squad?')){
      DB.players = DB.players.filter(p => p.id !== el.dataset.id);
      save(); router(false);
    }
    return;
  }
  if(act === 'match-del'){
    if(confirm('Delete this match?')){
      DB.matches = DB.matches.filter(m => m.id !== el.dataset.id);
      save(); router(false);
    }
    return;
  }
  if(act === 'gal-del'){
    if(confirm('Delete this photo?')){
      DB.gallery = DB.gallery.filter(g => g.id !== el.dataset.id);
      save(); router(false);
    }
    return;
  }
  if(act === 'news-del'){
    if(confirm('Delete this announcement?')){
      DB.news = DB.news.filter(n => n.id !== el.dataset.id);
      save(); router(false);
    }
    return;
  }
  if(act === 'hero-clear'){
    DB.settings.heroImage = '';
    save(); router(false);
    return;
  }
  if(act === 'fill-demo'){
    if(!confirm('Fill both squads with temporary sample statistics for preview?')) return;
    DB.players.forEach(p => {
      const base = Math.floor(Math.random() * 14) + 4;
      p.matches = base;
      p.goals = p.position === 'Forward' ? Math.floor(Math.random()*12)
              : p.position === 'Midfielder' ? Math.floor(Math.random()*7)
              : p.position === 'Defender' ? Math.floor(Math.random()*3) : 0;
      p.assists = Math.floor(Math.random()*7);
      p.yellow = Math.floor(Math.random()*4);
      p.red = Math.random() < 0.1 ? 1 : 0;
    });
    save(); router(false);
    return;
  }
  if(act === 'clear-stats'){
    if(!confirm('Reset every player statistic to zero?')) return;
    DB.players.forEach(p => { p.matches = 0; p.goals = 0; p.assists = 0; p.yellow = 0; p.red = 0; });
    save(); router(false);
    return;
  }
  if(act === 'reset-all'){
    if(!confirm('Reset ALL website data back to the original placeholders? This cannot be undone.')) return;
    DB = seed();
    save();
    state.editing = null;
    location.hash = '#home';
    router(true);
    return;
  }
});

/* forms */
document.addEventListener('submit', async e => {
  const form = e.target.closest('form[data-form]');
  if(!form) return;
  e.preventDefault();
  const kind = form.dataset.form;
  const fd = new FormData(form);

  /* ---- login ---- */
  if(kind === 'login'){
    if((fd.get('pass') || '') === DB.settings.adminPass){
      setAdmin(true);
      router(false);
    }else{
      alert('Incorrect password. Try again.');
    }
    return;
  }

  /* ---- player ---- */
  if(kind === 'player'){
    const id = fd.get('id');
    const existing = id ? getPlayer(id) : null;
    const data = {
      name: (fd.get('name') || '').trim(),
      number: +fd.get('number') || 0,
      position: fd.get('position') || 'Midfielder',
      age: fd.get('age') ? +fd.get('age') : '',
      nationality: (fd.get('nationality') || '').trim(),
      matches: Math.max(0, +fd.get('matches') || 0),
      goals: Math.max(0, +fd.get('goals') || 0),
      assists: Math.max(0, +fd.get('assists') || 0),
      yellow: Math.max(0, +fd.get('yellow') || 0),
      red: Math.max(0, +fd.get('red') || 0),
      bio: (fd.get('bio') || '').trim(),
      photo: state.pendingPhoto !== undefined ? state.pendingPhoto : (existing ? existing.photo : '')
    };
    if(!data.name){ alert('Please enter the player name.'); return; }

    if(existing){
      Object.assign(existing, data);
    }else{
      DB.players.push(Object.assign({ id: uid(), squad: state.adminSquad }, data));
    }
    state.editing = null;
    state.pendingPhoto = undefined;
    save(); router(false);
    return;
  }

  /* ---- match ---- */
  if(kind === 'match'){
    const status = fd.get('status');
    const gf = fd.get('goalsFor');
    const ga = fd.get('goalsAgainst');
    DB.matches.push({
      id: uid(),
      squad: fd.get('squad'),
      status,
      opponent: (fd.get('opponent') || '').trim() || 'TBA',
      date: fd.get('date') || iso(0),
      time: (fd.get('time') || '').trim(),
      venue: (fd.get('venue') || '').trim(),
      home: fd.get('home') === 'true',
      goalsFor: gf === '' ? null : +gf,
      goalsAgainst: ga === '' ? null : +ga,
      scorers: (fd.get('scorers') || '').trim(),
      report: (fd.get('report') || '').trim()
    });
    save(); router(false);
    return;
  }

  /* ---- gallery ---- */
  if(kind === 'gallery'){
    if(state.pendingPhoto === undefined){ alert('Please choose an image file.'); return; }
    DB.gallery.push({
      id: uid(),
      title: (fd.get('title') || 'Untitled photo').trim(),
      category: fd.get('category') || 'Team',
      image: state.pendingPhoto
    });
    state.pendingPhoto = undefined;
    save(); router(false);
    return;
  }

  /* ---- news ---- */
  if(kind === 'news'){
    DB.news.push({
      id: uid(),
      title: (fd.get('title') || '').trim(),
      date: fd.get('date') || iso(0),
      body: (fd.get('body') || '').trim()
    });
    save(); router(false);
    return;
  }

  /* ---- hero image ---- */
  if(kind === 'hero'){
    if(state.pendingPhoto === undefined){ alert('Please choose an image file.'); return; }
    DB.settings.heroImage = state.pendingPhoto;
    state.pendingPhoto = undefined;
    save(); router(false);
    return;
  }

  /* ---- password ---- */
  if(kind === 'password'){
    const pass = (fd.get('pass') || '').trim();
    if(pass.length < 4){ alert('Password must be at least 4 characters.'); return; }
    DB.settings.adminPass = pass;
    save();
    alert('Admin password updated.');
    return;
  }

  /* ---- contact ---- */
  if(kind === 'contact'){
    const name = fd.get('name');
    const email = fd.get('email');
    const msg = fd.get('message');
    const subject = encodeURIComponent('Website enquiry from ' + name);
    const body = encodeURIComponent(msg + '\n\nFrom: ' + name + ' <' + email + '>');
    window.location.href = `mailto:info@imanimarianistsctc.org?subject=${subject}&body=${body}`;
    form.reset();
    alert('Thank you! Your email app will open so you can send the message.');
    return;
  }
});

/* ============================================================
   9. BOOT
============================================================ */
document.getElementById('year').textContent = new Date().getFullYear();
if(!location.hash) location.hash = '#home';
router(true);
</script>
</body>
</html># docsa