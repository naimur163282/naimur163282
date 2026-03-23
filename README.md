<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MD Naimur Rashid | Textile Engineer & Denim Washing Specialist</title>
<link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&family=VT323&family=Orbitron:wght@400;600;700;800;900&family=Source+Code+Pro:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
<style>
:root{
  --bg:#020c02;--bg2:#040f04;--bg3:#050e05;
  --card:#070f07;--card2:#091209;
  --gold:#00ff41;--golddim:rgba(0,255,65,.1);
  --blue:#00e5ff;--blue2:#39ffdc;
  --teal:#00ff99;--teal2:#00ffbb;
  --pink:#ff0077;--pink2:#ff3399;
  --orange:#ff6600;--orange2:#ff8800;
  --purple:#bf00ff;--purple2:#cc33ff;
  --text:#00ff41;--text2:#7fff7f;--text3:#3d8b3d;
  --border:rgba(0,255,65,.15);--borderg:rgba(0,255,65,.3);
  --grad1:linear-gradient(135deg,#00ff41,#00e5ff);
  --grad2:linear-gradient(135deg,#00ff99,#00e5ff);
  --grad3:linear-gradient(135deg,#ff6600,#ff0077);
  --grad4:linear-gradient(135deg,#bf00ff,#00ff99);
  --scanline:repeating-linear-gradient(0deg,rgba(0,0,0,0.15) 0px,rgba(0,0,0,0.15) 1px,transparent 1px,transparent 2px);
  --glow:0 0 10px rgba(0,255,65,.4),0 0 20px rgba(0,255,65,.2);
  --glow2:0 0 10px rgba(0,229,255,.4),0 0 20px rgba(0,229,255,.2);
}
*{margin:0;padding:0;box-sizing:border-box}html{scroll-behavior:smooth}
body{font-family:'Source Code Pro',monospace;background:var(--bg);color:var(--text);overflow-x:hidden;
  background-image:
    var(--scanline),
    radial-gradient(ellipse at 10% 20%,rgba(0,255,65,.04) 0%,transparent 50%),
    radial-gradient(ellipse at 90% 10%,rgba(0,229,255,.04) 0%,transparent 50%),
    radial-gradient(ellipse at 50% 80%,rgba(0,255,153,.03) 0%,transparent 50%),
    radial-gradient(ellipse at 80% 60%,rgba(191,0,255,.03) 0%,transparent 50%);
}
/* Global cursor blink */
@keyframes blink{0%,100%{opacity:1}50%{opacity:0}}
@keyframes glitch{0%,100%{transform:translate(0);clip-path:none}20%{transform:translate(-2px,1px);clip-path:polygon(0 20%,100% 20%,100% 30%,0 30%)}40%{transform:translate(2px,-1px);clip-path:polygon(0 60%,100% 60%,100% 70%,0 70%)}60%{transform:translate(-1px,2px);clip-path:none}}
@keyframes scanline-move{0%{transform:translateY(-100%)}100%{transform:translateY(100vh)}}
@keyframes flicker{0%,100%{opacity:1}92%{opacity:1}93%{opacity:.7}94%{opacity:1}96%{opacity:.8}97%{opacity:1}}
@keyframes matrix-fall{0%{transform:translateY(-100%);opacity:1}100%{transform:translateY(100vh);opacity:0}}
@keyframes typewriter{from{width:0}to{width:100%}}
@keyframes terminal-boot{0%{opacity:0;transform:scaleY(0)}50%{opacity:1;transform:scaleY(1)}100%{opacity:1}}
/* CRT overlay */
body::before{content:'';position:fixed;inset:0;background:var(--scanline);pointer-events:none;z-index:9998;opacity:.4}
body::after{content:'';position:fixed;inset:0;background:radial-gradient(ellipse at center,transparent 50%,rgba(0,0,0,.7) 100%);pointer-events:none;z-index:9997}

/* NAV */
nav{position:fixed;top:0;width:100%;z-index:1000;background:rgba(2,12,2,.97);backdrop-filter:blur(4px);border-bottom:1px solid var(--border);padding:0 1.5rem;height:62px;display:flex;align-items:center;justify-content:space-between;box-shadow:0 2px 20px rgba(0,255,65,.1),inset 0 -1px 0 rgba(0,255,65,.2)}
.nav-brand{display:flex;align-items:center;gap:.75rem}
.nav-logo{width:40px;height:40px;border-radius:4px;background:transparent;border:1.5px solid var(--gold);display:flex;align-items:center;justify-content:center;position:relative;box-shadow:var(--glow);animation:flicker 8s infinite}
.nav-logo::after{content:'';position:absolute;inset:2px;border-radius:2px;background:rgba(0,255,65,.07)}
.nav-logo span{position:relative;z-index:1;color:var(--gold);font-family:'Orbitron',monospace;font-size:.85rem;font-weight:700}
.brand-name{font-family:'Orbitron',monospace;font-size:.88rem;font-weight:700;color:var(--text);letter-spacing:.1em;text-shadow:var(--glow)}
.brand-sub{font-size:.6rem;color:var(--teal);letter-spacing:.1em;font-weight:600;font-family:'Share Tech Mono',monospace}
.nav-links{display:flex;gap:.1rem;list-style:none}
.nav-links a{color:var(--text3);text-decoration:none;font-size:.72rem;font-weight:500;padding:.35rem .68rem;border-radius:2px;transition:color .2s;position:relative;font-family:'Share Tech Mono',monospace;letter-spacing:.05em;text-transform:uppercase}
.nav-links a::before{content:'[';color:transparent;margin-right:1px;transition:color .2s}
.nav-links a::after{content:']';color:transparent;margin-left:1px;position:static;width:auto;height:auto;background:none;transition:color .2s;border-radius:0}
.nav-links a:hover{color:var(--gold);text-shadow:var(--glow)}
.nav-links a:hover::before,.nav-links a:hover::after{color:var(--teal)}
.nav-r{display:flex;align-items:center;gap:.5rem}
.cv-btn{background:transparent;color:var(--gold);padding:.42rem 1.1rem;border-radius:2px;font-weight:700;font-size:.72rem;border:1px solid var(--gold);cursor:pointer;font-family:'Orbitron',monospace;transition:all .2s;box-shadow:var(--glow);letter-spacing:.1em;text-transform:uppercase}
.cv-btn:hover{background:rgba(0,255,65,.1);box-shadow:0 0 20px rgba(0,255,65,.5)}
.hamburger{display:none;flex-direction:column;gap:5px;cursor:pointer}
.hamburger span{width:22px;height:2px;background:var(--gold)}
.mob-menu{display:none;position:fixed;top:62px;left:0;width:100%;background:rgba(2,12,2,.99);border-bottom:1px solid var(--border);padding:1rem 1.5rem;z-index:999;box-shadow:0 8px 20px rgba(0,255,65,.1)}
.mob-menu a{display:block;color:var(--text2);text-decoration:none;padding:.6rem 0;border-bottom:1px solid var(--border);font-size:.82rem;font-family:'Share Tech Mono',monospace}
.mob-menu.open{display:block}

/* HERO */
.hero{min-height:100vh;padding-top:62px;background:var(--bg);position:relative;overflow:hidden}
/* Matrix rain bg */
.hero::before{content:'';position:absolute;inset:0;background:
  radial-gradient(ellipse at 70% 40%,rgba(0,255,65,.06) 0%,transparent 55%),
  radial-gradient(ellipse at 20% 70%,rgba(0,229,255,.04) 0%,transparent 50%),
  radial-gradient(ellipse at 90% 80%,rgba(0,255,153,.03) 0%,transparent 45%);pointer-events:none}
.hero-grid{display:grid;grid-template-columns:1.1fr 1fr;min-height:calc(100vh - 62px);max-width:1400px;margin:0 auto;padding:2rem;gap:2rem;align-items:center}
.hero-eyebrow{display:flex;align-items:center;gap:.75rem;margin-bottom:1.2rem}
.ey-line{width:30px;height:1px;background:var(--teal);box-shadow:0 0 6px var(--teal)}
.ey-text{font-size:.65rem;letter-spacing:.2em;text-transform:uppercase;color:var(--teal);font-weight:700;font-family:'Share Tech Mono',monospace}
.ey-text::before{content:'> '}
.hero-name{font-family:'Orbitron',monospace;font-size:clamp(2rem,4.5vw,4.2rem);font-weight:900;line-height:1;margin-bottom:.6rem;animation:flicker 12s infinite}
.hero-name .fn{color:var(--gold);display:block;text-shadow:var(--glow)}
.hero-name .ln{color:var(--blue);display:block;text-shadow:var(--glow2)}
.hero-title{font-size:.88rem;color:var(--text2);font-weight:400;margin-bottom:1rem;font-family:'Share Tech Mono',monospace;letter-spacing:.05em}
.hero-title::before{content:'// ';color:var(--text3)}
.washing-tags{display:flex;align-items:center;gap:.45rem;margin-bottom:1rem;flex-wrap:wrap}
.wt{padding:.22rem .72rem;border-radius:2px;font-size:.72rem;font-weight:600;border:1px solid;font-family:'Share Tech Mono',monospace;letter-spacing:.05em}
.wt-b{background:rgba(0,229,255,.07);border-color:rgba(0,229,255,.3);color:var(--blue);box-shadow:0 0 8px rgba(0,229,255,.2)}
.wt-g{background:rgba(0,255,153,.07);border-color:rgba(0,255,153,.3);color:var(--teal);box-shadow:0 0 8px rgba(0,255,153,.2)}
.wt-sep{color:var(--text3);font-weight:700}
.pgd-badge{display:inline-flex;align-items:center;gap:.75rem;background:rgba(191,0,255,.07);border:1px solid rgba(191,0,255,.3);padding:.55rem 1rem;border-radius:2px;margin-bottom:1.15rem;box-shadow:0 0 10px rgba(191,0,255,.15)}
.pgd-title{font-weight:700;font-size:.82rem;color:var(--purple);font-family:'Orbitron',monospace;letter-spacing:.05em;text-shadow:0 0 8px var(--purple)}
.pgd-sub{font-size:.65rem;color:var(--text3);font-family:'Share Tech Mono',monospace}
.hero-perks{display:flex;flex-direction:column;gap:.42rem;margin-bottom:1.4rem}
.perk{display:flex;align-items:center;gap:.55rem;font-size:.8rem;color:var(--text2);font-family:'Share Tech Mono',monospace}
.perk::before{content:'>>  ';color:var(--teal);flex-shrink:0}
.perk strong{color:var(--gold);font-weight:700}
.hero-btns{display:flex;gap:.65rem;flex-wrap:wrap}
.hbtn-p{background:transparent;color:var(--gold);padding:.62rem 1.35rem;border-radius:2px;font-weight:700;font-size:.75rem;border:1.5px solid var(--gold);cursor:pointer;font-family:'Orbitron',monospace;transition:all .2s;box-shadow:var(--glow);letter-spacing:.08em;text-transform:uppercase}
.hbtn-p:hover{background:rgba(0,255,65,.1);transform:translateY(-2px);box-shadow:0 0 30px rgba(0,255,65,.5)}
.hbtn-o{background:transparent;color:var(--blue);padding:.62rem 1.15rem;border-radius:2px;font-weight:600;font-size:.75rem;border:1.5px solid rgba(0,229,255,.4);cursor:pointer;font-family:'Orbitron',monospace;transition:all .2s;letter-spacing:.06em;text-transform:uppercase}
.hbtn-o:hover{border-color:var(--blue);background:rgba(0,229,255,.07);box-shadow:var(--glow2)}
.hbtn-g{background:transparent;color:var(--teal);padding:.62rem 1.15rem;border-radius:2px;font-weight:700;font-size:.75rem;border:1.5px solid rgba(0,255,153,.4);cursor:pointer;font-family:'Orbitron',monospace;transition:all .2s;letter-spacing:.06em;text-transform:uppercase}
.hbtn-g:hover{background:rgba(0,255,153,.07);box-shadow:0 0 20px rgba(0,255,153,.4)}

/* HERO CIRCULAR PHOTO */
.hero-right{position:relative;display:flex;align-items:center;justify-content:center}
.hero-photo-area{position:relative;width:340px;height:340px}
.photo-ring-outer{position:absolute;inset:-18px;border-radius:50%;border:1px solid rgba(0,255,65,.4);animation:ring-spin 8s linear infinite;box-shadow:0 0 20px rgba(0,255,65,.2)}
@keyframes ring-spin{to{transform:rotate(360deg)}}
.photo-ring-dash{position:absolute;inset:-8px;border-radius:50%;border:1px dashed rgba(0,229,255,.3);animation:ring-spin 14s linear infinite reverse}
.photo-circle{width:340px;height:340px;border-radius:50%;overflow:hidden;background:radial-gradient(circle,rgba(0,255,65,.05),rgba(0,12,0,.9));border:2px solid rgba(0,255,65,.4);box-shadow:0 0 0 1px rgba(0,229,255,.2),var(--glow),0 0 80px rgba(0,255,65,.1),inset 0 0 60px rgba(0,255,65,.05);position:relative;display:flex;align-items:center;justify-content:center}
.photo-circle img#heroPhotoImg{width:100%;height:100%;object-fit:cover;object-position:top center;display:none;position:absolute;inset:0;filter:brightness(1.1) contrast(1.1) saturate(0.9) hue-rotate(0deg)}
.photo-circle .photo-placeholder-inner{display:flex;flex-direction:column;align-items:center;justify-content:center;gap:.6rem;pointer-events:none;z-index:2}
.photo-placeholder-inner .icon{font-size:5.5rem;opacity:.3;filter:hue-rotate(120deg)}
.photo-placeholder-inner .hint{font-size:.65rem;color:var(--text3);text-align:center;line-height:1.6;background:rgba(0,255,65,.05);border:1px solid var(--border);border-radius:2px;padding:.4rem 1rem;font-family:'Share Tech Mono',monospace}
.photo-circle::after{content:'';position:absolute;bottom:0;left:0;right:0;height:30%;background:linear-gradient(to top,rgba(0,255,65,.08),transparent);pointer-events:none;border-radius:0 0 50% 50%;z-index:1}
/* Orbit Bubbles */
.ob{position:absolute;z-index:10;background:rgba(2,12,2,.95);border:1px solid rgba(0,255,65,.4);border-radius:4px;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;box-shadow:var(--glow)}
.ob1{width:84px;height:84px;top:-10px;left:-15px;animation:obf1 5s ease-in-out infinite;border-color:rgba(0,229,255,.5)}
.ob2{width:78px;height:78px;bottom:30px;left:-20px;border-color:rgba(0,255,153,.5);animation:obf2 6s ease-in-out infinite}
.ob3{width:88px;height:88px;top:-5px;right:-15px;border-color:rgba(255,0,119,.5);animation:obf1 4.5s ease-in-out infinite .5s}
.ob4{width:80px;height:80px;bottom:20px;right:-18px;border-color:rgba(191,0,255,.5);animation:obf2 5.5s ease-in-out infinite 1s}
@keyframes obf1{0%,100%{transform:translateY(0)}50%{transform:translateY(-10px)}}
@keyframes obf2{0%,100%{transform:translateY(0)}50%{transform:translateY(9px)}}
.ob-num{font-family:'Orbitron',monospace;font-size:1.2rem;font-weight:800;line-height:1}
.ob1 .ob-num{color:var(--blue);text-shadow:var(--glow2)}
.ob2 .ob-num{color:var(--teal);text-shadow:0 0 8px var(--teal)}
.ob3 .ob-num{color:var(--pink);text-shadow:0 0 8px var(--pink)}
.ob4 .ob-num{color:var(--purple);text-shadow:0 0 8px var(--purple)}
.ob-lbl{font-size:.52rem;color:var(--text3);line-height:1.2;margin-top:2px;padding:0 4px;font-family:'Share Tech Mono',monospace;text-transform:uppercase;letter-spacing:.05em}

/* STATS BAR */
.stats-bar{background:rgba(0,12,0,.95);border-top:1px solid rgba(0,255,65,.2);border-bottom:1px solid rgba(0,255,65,.2);padding:.82rem 2rem;box-shadow:0 0 20px rgba(0,255,65,.08) inset}
.stats-inner{max-width:1400px;margin:0 auto;display:flex;justify-content:space-around;flex-wrap:wrap;gap:.4rem}
.si{display:flex;align-items:center;gap:.7rem;padding:.2rem .9rem;border-right:1px solid rgba(0,255,65,.1)}
.si:last-child{border-right:none}
.si-num{font-family:'Orbitron',monospace;font-size:1.3rem;font-weight:700;line-height:1}
.si:nth-child(1) .si-num{color:var(--blue);text-shadow:var(--glow2)}
.si:nth-child(2) .si-num{color:var(--teal);text-shadow:0 0 8px var(--teal)}
.si:nth-child(3) .si-num{color:var(--pink);text-shadow:0 0 8px var(--pink)}
.si:nth-child(4) .si-num{color:var(--purple);text-shadow:0 0 8px var(--purple)}
.si:nth-child(5) .si-num{color:var(--orange);text-shadow:0 0 8px var(--orange)}
.si-lbl{font-size:.58rem;color:var(--text3);text-transform:uppercase;letter-spacing:.08em;line-height:1.2;font-family:'Share Tech Mono',monospace}

/* MAIN */
.main{max-width:1400px;margin:0 auto;padding:1.6rem}
.col3{display:grid;grid-template-columns:1.3fr 1fr .85fr;gap:1.2rem;align-items:start}

/* CARDS */
.dc{background:var(--card);border:1px solid var(--border);border-radius:4px;overflow:hidden;box-shadow:0 2px 16px rgba(0,255,65,.05),inset 0 0 30px rgba(0,255,65,.02)}
.dc-head{padding:.82rem 1.15rem;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;background:rgba(0,255,65,.03)}
.dc-title{font-family:'Orbitron',monospace;font-size:.78rem;font-weight:700;letter-spacing:.12em;text-transform:uppercase;color:var(--gold);text-shadow:var(--glow)}
.dc-line{width:26px;height:1px;background:var(--gold);box-shadow:var(--glow)}

/* EXPERTISE */
.etabs{display:flex;gap:.32rem;padding:.65rem 1.15rem;border-bottom:1px solid var(--border);flex-wrap:wrap}
.etab{padding:.26rem .8rem;border-radius:2px;font-size:.68rem;font-weight:600;cursor:pointer;transition:all .2s;border:1px solid var(--border);background:transparent;color:var(--text3);font-family:'Share Tech Mono',monospace;text-transform:uppercase;letter-spacing:.08em}
.etab.active{background:rgba(0,255,65,.1);color:var(--gold);border-color:var(--gold);box-shadow:var(--glow)}
.etab:hover:not(.active){border-color:var(--blue);color:var(--blue)}
.exp-body{padding:.9rem 1.15rem}
.exp-list{list-style:none;display:flex;flex-direction:column;gap:.38rem}
.exp-list li{display:flex;align-items:center;gap:.52rem;font-size:.77rem;color:var(--text2);padding:.3rem 0;border-bottom:1px solid rgba(0,255,65,.06);font-family:'Share Tech Mono',monospace}
.exp-list li:last-child{border-bottom:none}
.exp-list li strong{color:var(--blue);font-weight:700}

/* R&D */
.rnd-body{padding:.95rem 1.15rem}
.rnd-ptitle{font-weight:700;font-size:.88rem;color:var(--gold);margin-bottom:.32rem;font-family:'Orbitron',monospace;letter-spacing:.06em;text-shadow:var(--glow)}
.approved-b{display:inline-flex;gap:.35rem;align-items:center;background:rgba(0,255,153,.07);border:1px solid rgba(0,255,153,.3);padding:.16rem .56rem;border-radius:2px;font-size:.6rem;font-weight:700;color:var(--teal);letter-spacing:.08em;margin-bottom:.72rem;font-family:'Share Tech Mono',monospace;box-shadow:0 0 8px rgba(0,255,153,.15)}
.rnd-img-box{width:100%;height:110px;border-radius:4px;overflow:hidden;margin-bottom:.72rem;border:1px solid var(--border);background:rgba(0,255,65,.03);display:flex;align-items:center;justify-content:center;position:relative;cursor:pointer}
.rnd-img-box img{width:100%;height:100%;object-fit:cover;display:none}
.rnd-img-ph{font-size:2.8rem;filter:hue-rotate(120deg)}
.rnd-points{display:flex;flex-direction:column;gap:.35rem;margin-bottom:.85rem}
.rnd-pt{display:flex;align-items:center;gap:.45rem;font-size:.73rem;color:var(--text2);font-family:'Share Tech Mono',monospace}
.rnd-dot{width:4px;height:4px;background:var(--teal);flex-shrink:0;box-shadow:0 0 6px var(--teal)}
.rnd-cta{width:100%;background:transparent;color:var(--teal);padding:.5rem;border-radius:2px;font-weight:700;font-size:.72rem;border:1px solid rgba(0,255,153,.4);cursor:pointer;font-family:'Orbitron',monospace;display:flex;align-items:center;justify-content:center;gap:.35rem;transition:all .2s;letter-spacing:.08em;text-transform:uppercase}
.rnd-cta:hover{background:rgba(0,255,153,.07);box-shadow:0 0 20px rgba(0,255,153,.3)}

/* EXP TIMELINE */
.etl{padding:.9rem 1.15rem;display:flex;flex-direction:column}
.etl-item{position:relative;padding-left:1rem;padding-bottom:1.05rem;border-left:1px solid rgba(0,255,65,.2)}
.etl-item:last-child{border-left:1px solid transparent;padding-bottom:0}
.etl-dot{position:absolute;left:-4px;top:4px;width:7px;height:7px;background:var(--text3);box-shadow:0 0 8px rgba(0,255,65,.3)}
.etl-item.cur .etl-dot{background:var(--teal);box-shadow:0 0 8px rgba(0,255,153,.8);animation:pdot 2s infinite}
@keyframes pdot{0%,100%{box-shadow:0 0 8px rgba(0,255,153,.6)}50%{box-shadow:0 0 20px rgba(0,255,153,1)}}
.etl-role{font-weight:700;font-size:.8rem;color:var(--gold);line-height:1.2;font-family:'Orbitron',monospace;letter-spacing:.04em}
.etl-co{font-size:.71rem;font-weight:600;color:var(--blue);margin-top:.16rem;font-family:'Share Tech Mono',monospace}
.etl-date{font-size:.63rem;color:var(--text3);margin-top:.1rem;font-family:'Share Tech Mono',monospace}
.etl-buyer{font-size:.62rem;color:var(--teal);margin-top:.2rem;display:inline-block;background:rgba(0,255,153,.07);padding:.1rem .4rem;font-weight:600;font-family:'Share Tech Mono',monospace;border:1px solid rgba(0,255,153,.2)}

/* CERT SIDEBAR */
.cert-sidebar{padding:.65rem 1.15rem;display:flex;flex-direction:column;gap:.38rem}
.cert-si{display:flex;align-items:center;gap:.52rem;padding:.42rem 0;border-bottom:1px solid rgba(0,255,65,.08);cursor:pointer;transition:all .2s}
.cert-si:last-child{border-bottom:none}
.cert-si:hover{padding-left:.2rem}
.cert-si-img{width:28px;height:28px;border-radius:2px;overflow:hidden;flex-shrink:0;background:rgba(0,255,65,.07);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:.8rem;filter:hue-rotate(120deg)}
.cert-si-img img{width:100%;height:100%;object-fit:cover;border-radius:2px;filter:none}
.cert-si-name{font-size:.7rem;color:var(--text2);font-weight:600;line-height:1.3;font-family:'Share Tech Mono',monospace}
.cert-si-org{font-size:.6rem;color:var(--purple);font-family:'Share Tech Mono',monospace}
.cert-arrow{color:var(--text3);font-size:.7rem;margin-left:auto;transition:all .2s}
.cert-si:hover .cert-arrow{color:var(--gold);transform:translateX(3px)}
.view-all{width:100%;background:rgba(0,255,65,.05);color:var(--gold);padding:.48rem;border-radius:0 0 2px 2px;font-weight:600;font-size:.68rem;border:none;border-top:1px solid var(--border);cursor:pointer;font-family:'Share Tech Mono',monospace;letter-spacing:.08em;text-transform:uppercase;transition:background .2s}
.view-all:hover{background:rgba(0,255,65,.1)}

/* PORTFOLIO */
.port-sec{margin-top:1.3rem}
.sec-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:.9rem}
.sec-title-wrap{display:flex;align-items:center;gap:.65rem}
.stl{width:20px;height:1px;background:var(--gold);box-shadow:var(--glow)}
.str{flex:1;height:1px;background:linear-gradient(90deg,rgba(0,255,65,.2),transparent)}
.sec-ttl{font-family:'Orbitron',monospace;font-size:.88rem;font-weight:700;letter-spacing:.12em;text-transform:uppercase;color:var(--gold);text-shadow:var(--glow)}
.pf-btns{display:flex;gap:.32rem;flex-wrap:wrap}
.pf-btn{padding:.22rem .68rem;border-radius:2px;font-size:.62rem;font-weight:600;cursor:pointer;transition:all .2s;border:1px solid var(--border);background:transparent;color:var(--text3);font-family:'Share Tech Mono',monospace;text-transform:uppercase;letter-spacing:.06em}
.pf-btn.active,.pf-btn:hover{background:rgba(0,255,65,.1);color:var(--gold);border-color:var(--gold);box-shadow:var(--glow)}
.port-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(152px,1fr));gap:.65rem}
.port-card{border-radius:4px;overflow:hidden;position:relative;cursor:pointer;transition:all .3s;border:1px solid var(--border);background:var(--card);box-shadow:0 2px 10px rgba(0,255,65,.04)}
.port-card:hover{transform:translateY(-3px);border-color:rgba(0,255,65,.4);box-shadow:var(--glow)}
.port-img{height:105px;position:relative;overflow:hidden;background:rgba(0,255,65,.03);display:flex;align-items:center;justify-content:center;font-size:2.1rem;filter:hue-rotate(100deg)}
.port-img img{width:100%;height:100%;object-fit:cover;position:absolute;inset:0;filter:none}
.port-ov{position:absolute;inset:0;background:linear-gradient(to top,rgba(2,12,2,.9) 0%,transparent 60%)}
.port-lbl{position:absolute;bottom:0;left:0;right:0;padding:.42rem;text-align:center;z-index:2}
.port-name{font-size:.67rem;font-weight:700;color:var(--gold);display:block;font-family:'Share Tech Mono',monospace;text-transform:uppercase;letter-spacing:.05em}
.port-tech{font-size:.57rem;color:var(--blue);display:block;margin-top:1px;font-weight:600;font-family:'Share Tech Mono',monospace}

/* FULL SECTIONS */
.full-sec{padding:2.4rem 2rem}
.full-sec-inner{max-width:1400px;margin:0 auto}
.fs-hdr{display:flex;align-items:center;gap:.65rem;margin-bottom:.45rem}
.fs-sub{color:var(--text3);font-size:.78rem;margin-bottom:1.6rem;font-family:'Share Tech Mono',monospace}
.fs-sub::before{content:'// '}

/* CERTS GRID */
.certs-full-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(230px,1fr));gap:.85rem}
.cert-card{background:var(--card);border:1px solid var(--border);border-radius:4px;overflow:hidden;cursor:pointer;transition:all .3s;box-shadow:0 2px 12px rgba(0,255,65,.04)}
.cert-card:hover{transform:translateY(-3px);border-color:rgba(0,255,65,.4);box-shadow:var(--glow)}
.cert-card-img{height:115px;background:rgba(0,255,65,.03);display:flex;align-items:center;justify-content:center;font-size:2.7rem;overflow:hidden;filter:hue-rotate(120deg)}
.cert-card-img img{width:100%;height:100%;object-fit:cover;filter:none}
.cert-card-body{padding:.85rem .95rem}
.cert-card-org{font-size:.6rem;color:var(--purple);font-weight:700;letter-spacing:.1em;text-transform:uppercase;margin-bottom:.22rem;font-family:'Share Tech Mono',monospace}
.cert-card-name{font-weight:700;font-size:.77rem;color:var(--text2);line-height:1.4;font-family:'Share Tech Mono',monospace}

/* CASES */
.cases-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:.85rem}
.case-card{background:var(--card);border:1px solid var(--border);border-radius:4px;overflow:hidden;transition:all .3s;box-shadow:0 2px 12px rgba(0,255,65,.04)}
.case-card:hover{transform:translateY(-3px);box-shadow:var(--glow)}
.case-head{background:rgba(0,255,65,.03);padding:.95rem 1.1rem;border-bottom:1px solid var(--border)}
.case-buyer{font-size:.58rem;letter-spacing:.15em;text-transform:uppercase;color:var(--pink);font-weight:700;margin-bottom:.26rem;font-family:'Orbitron',monospace;text-shadow:0 0 8px var(--pink)}
.case-title{font-family:'Orbitron',monospace;font-size:.82rem;font-weight:700;color:var(--gold);letter-spacing:.04em}
.case-body{padding:.95rem 1.1rem}
.case-row{display:flex;gap:.45rem;padding:.32rem 0;border-bottom:1px solid rgba(0,255,65,.06);font-size:.72rem;font-family:'Share Tech Mono',monospace}
.case-row:last-of-type{border-bottom:none}
.cl{color:var(--text3);min-width:105px;flex-shrink:0;font-weight:500}
.cv2{color:var(--text2)}
.case-result{background:rgba(0,255,153,.05);border-left:2px solid var(--teal);padding:.52rem .75rem;border-radius:0 2px 2px 0;margin-top:.65rem;font-size:.71rem;color:var(--teal);line-height:1.6;font-weight:600;font-family:'Share Tech Mono',monospace;box-shadow:0 0 8px rgba(0,255,153,.1)}

/* SKILLS */
.skills-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(165px,1fr));gap:.7rem}
.sk-card{background:var(--card);border:1px solid var(--border);border-radius:4px;padding:.85rem;transition:all .25s;position:relative;overflow:hidden;box-shadow:0 2px 10px rgba(0,255,65,.03)}
.sk-card::before{content:'';position:absolute;left:0;top:0;bottom:0;width:2px;background:var(--gold);box-shadow:var(--glow)}
.sk-card:nth-child(4n+1)::before{background:var(--blue);box-shadow:var(--glow2)}
.sk-card:nth-child(4n+2)::before{background:var(--teal);box-shadow:0 0 8px var(--teal)}
.sk-card:nth-child(4n+3)::before{background:var(--pink);box-shadow:0 0 8px var(--pink)}
.sk-card:nth-child(4n+4)::before{background:var(--purple);box-shadow:0 0 8px var(--purple)}
.sk-card:hover{transform:translateY(-2px);border-color:rgba(0,255,65,.3);box-shadow:var(--glow)}
.sk-icon{font-size:1.1rem;margin-bottom:.35rem;filter:hue-rotate(120deg)}
.sk-name{font-size:.74rem;font-weight:600;color:var(--text2);margin-bottom:.42rem;font-family:'Share Tech Mono',monospace;text-transform:uppercase;letter-spacing:.05em}
.sk-bar{height:2px;background:rgba(0,255,65,.1);border-radius:0;overflow:hidden}
.sk-fill{height:100%;background:linear-gradient(90deg,var(--gold),var(--teal));border-radius:0;width:0;transition:width 1.2s ease;box-shadow:var(--glow)}

/* BUYERS */
.buyers-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(260px,1fr));gap:.85rem}
.buyer-card{background:var(--card);border:1px solid var(--border);border-radius:4px;padding:1.4rem;transition:all .3s;position:relative;overflow:hidden;box-shadow:0 2px 12px rgba(0,255,65,.04)}
.buyer-card::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:var(--gold);box-shadow:var(--glow)}
.buyer-card:nth-child(3n+2)::before{background:var(--teal);box-shadow:0 0 8px var(--teal)}
.buyer-card:nth-child(3n+3)::before{background:var(--blue);box-shadow:var(--glow2)}
.buyer-card:hover{transform:translateY(-3px);border-color:rgba(0,255,65,.3);box-shadow:var(--glow)}
.buyer-card .logo{width:40px;height:40px;border-radius:2px;background:rgba(0,255,65,.07);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:1.2rem;margin-bottom:.85rem;overflow:hidden;filter:hue-rotate(120deg)}
.buyer-card .logo img{width:100%;height:100%;object-fit:cover;border-radius:2px;filter:none}
.buyer-name{font-family:'Orbitron',monospace;font-size:.95rem;font-weight:700;color:var(--gold);margin-bottom:.2rem;letter-spacing:.04em;text-shadow:var(--glow)}
.buyer-proj{color:var(--blue);font-size:.76rem;font-weight:600;margin-bottom:.65rem;font-family:'Share Tech Mono',monospace}
.buyer-spec{font-size:.74rem;color:var(--text2);line-height:1.65;font-family:'Share Tech Mono',monospace}
.q-badge{display:inline-flex;align-items:center;gap:.3rem;background:rgba(0,255,153,.07);color:var(--teal);padding:.22rem .55rem;border-radius:2px;font-size:.65rem;font-weight:700;margin-top:.65rem;font-family:'Share Tech Mono',monospace;border:1px solid rgba(0,255,153,.2)}

/* CONTACT */
.contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:1.8rem;align-items:start}
.ci{display:flex;align-items:center;gap:.82rem;padding:.82rem;background:var(--card);border:1px solid var(--border);border-radius:4px;margin-bottom:.65rem;box-shadow:0 2px 8px rgba(0,255,65,.04)}
.ci-icon{width:32px;height:32px;border-radius:2px;background:rgba(0,255,65,.07);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:.88rem;flex-shrink:0;filter:hue-rotate(120deg)}
.ci-lbl{font-size:.58rem;color:var(--text3);text-transform:uppercase;letter-spacing:.08em;font-family:'Share Tech Mono',monospace}
.ci-val{color:var(--teal);font-weight:600;font-size:.8rem;font-family:'Share Tech Mono',monospace}
.cf-inp{width:100%;background:rgba(0,255,65,.04);border:1px solid var(--border);border-radius:2px;padding:.58rem .85rem;font-family:'Share Tech Mono',monospace;font-size:.77rem;color:var(--text);outline:none;transition:border-color .2s;margin-bottom:.65rem}
.cf-inp:focus{border-color:var(--gold);box-shadow:var(--glow)}
.cf-lbl{display:block;font-size:.62rem;color:var(--text3);text-transform:uppercase;letter-spacing:.08em;margin-bottom:.28rem;font-family:'Share Tech Mono',monospace}
.cf-sub{width:100%;background:transparent;color:var(--gold);padding:.65rem;border-radius:2px;font-weight:700;font-size:.75rem;border:1.5px solid var(--gold);cursor:pointer;font-family:'Orbitron',monospace;transition:all .2s;box-shadow:var(--glow);letter-spacing:.08em;text-transform:uppercase}
.cf-sub:hover{background:rgba(0,255,65,.1);transform:translateY(-1px);box-shadow:0 0 30px rgba(0,255,65,.4)}

/* FOOTER */
.footer-bar{background:rgba(0,8,0,.98);border-top:1px solid var(--border);padding:.78rem 2rem;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:.7rem}
.fc-item{display:flex;align-items:center;gap:.38rem;font-size:.72rem;color:var(--text3);font-family:'Share Tech Mono',monospace}
.footer-contacts{display:flex;gap:1.4rem;flex-wrap:wrap}
.footer-cta{background:transparent;color:var(--gold);padding:.48rem 1.15rem;border-radius:2px;font-weight:700;font-size:.72rem;border:1px solid var(--gold);cursor:pointer;font-family:'Orbitron',monospace;transition:all .2s;box-shadow:var(--glow);letter-spacing:.08em;text-transform:uppercase}
.footer-cta:hover{background:rgba(0,255,65,.1);box-shadow:0 0 20px rgba(0,255,65,.4)}
.soc-btns{display:flex;gap:.42rem}
.soc-b{width:29px;height:29px;border-radius:2px;background:transparent;border:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:.7rem;cursor:pointer;color:var(--text3);transition:all .2s;font-family:'Orbitron',monospace}
.soc-b:hover{border-color:var(--gold);color:var(--gold);box-shadow:var(--glow)}

/* AI CHAT */
.chat-wrap{position:fixed;bottom:1.4rem;right:1.4rem;z-index:2000}
.chat-toggle{width:52px;height:52px;border-radius:2px;background:rgba(0,12,0,.95);border:1.5px solid var(--gold);cursor:pointer;box-shadow:var(--glow);transition:all .3s;display:flex;align-items:center;justify-content:center;color:var(--gold);font-family:'Orbitron',monospace;font-weight:800;font-size:.88rem;letter-spacing:.02em;animation:flicker 10s infinite}
.chat-toggle:hover{transform:scale(1.07);box-shadow:0 0 30px rgba(0,255,65,.6);background:rgba(0,255,65,.1)}
.chat-win{position:absolute;bottom:62px;right:0;width:308px;background:rgba(2,8,2,.98);border:1px solid var(--border);border-radius:4px;box-shadow:var(--glow),0 18px 55px rgba(0,0,0,.8);display:none;flex-direction:column;overflow:hidden}
.chat-win.open{display:flex;animation:cfade .3s ease}
@keyframes cfade{from{opacity:0;transform:translateY(12px) scale(.97)}to{opacity:1;transform:none}}
.chat-hdr{background:rgba(0,255,65,.05);padding:.82rem .95rem;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid var(--border)}
.chat-av{width:32px;height:32px;border-radius:2px;background:transparent;border:1.5px solid var(--gold);display:flex;align-items:center;justify-content:center;color:var(--gold);font-family:'Orbitron',monospace;font-weight:800;font-size:.75rem;flex-shrink:0;box-shadow:var(--glow)}
.chat-hdr-name{font-weight:700;font-size:.78rem;color:var(--gold);font-family:'Orbitron',monospace;letter-spacing:.06em}
.chat-hdr-st{font-size:.62rem;color:var(--teal);font-weight:600;font-family:'Share Tech Mono',monospace}
.chat-hdr-st::before{content:'● '}
.chat-close{background:none;border:none;color:var(--text3);cursor:pointer;font-size:1.05rem;padding:0}
.chat-chips{padding:.42rem;display:flex;flex-wrap:wrap;gap:.26rem;border-bottom:1px solid var(--border);background:rgba(0,255,65,.02)}
.chip{padding:.16rem .48rem;border-radius:2px;border:1px solid var(--border);color:var(--text3);font-size:.62rem;cursor:pointer;background:transparent;transition:all .2s;font-family:'Share Tech Mono',monospace;text-transform:uppercase;letter-spacing:.05em}
.chip:hover{background:rgba(0,255,65,.08);color:var(--gold);border-color:var(--gold)}
.chat-msgs{height:225px;overflow-y:auto;padding:.65rem;display:flex;flex-direction:column;gap:.52rem;background:rgba(0,8,0,.6)}
.chat-msgs::-webkit-scrollbar{width:3px}
.chat-msgs::-webkit-scrollbar-thumb{background:rgba(0,255,65,.2)}
.cm{max-width:84%}
.cm.bot{align-self:flex-start}.cm.user{align-self:flex-end}
.cm-b{padding:.48rem .72rem;border-radius:2px;font-size:.73rem;line-height:1.55;font-family:'Share Tech Mono',monospace}
.cm.bot .cm-b{background:rgba(0,255,65,.06);color:var(--text2);border:1px solid var(--border)}
.cm.bot .cm-b::before{content:'> ';color:var(--gold)}
.cm.user .cm-b{background:rgba(0,229,255,.08);color:var(--blue);border:1px solid rgba(0,229,255,.2)}
.chat-inp-row{padding:.52rem;border-top:1px solid var(--border);display:flex;gap:.38rem;background:rgba(0,8,0,.8)}
.chat-inp{flex:1;background:rgba(0,255,65,.04);border:1px solid var(--border);border-radius:2px;padding:.4rem .7rem;font-size:.72rem;color:var(--text);outline:none;font-family:'Share Tech Mono',monospace}
.chat-inp:focus{border-color:var(--gold);box-shadow:var(--glow)}
.chat-inp::placeholder{color:var(--text3)}
.chat-send{width:28px;height:28px;border-radius:2px;background:transparent;border:1px solid var(--gold);color:var(--gold);cursor:pointer;font-size:.76rem;display:flex;align-items:center;justify-content:center;flex-shrink:0;box-shadow:var(--glow)}
.typing{display:flex;gap:3px;padding:.22rem 0}
.td{width:5px;height:5px;background:rgba(0,255,65,.4);animation:tdb 1.4s infinite}
.td:nth-child(2){animation-delay:.2s}.td:nth-child(3){animation-delay:.4s}
@keyframes tdb{0%,80%,100%{transform:scale(0)}40%{transform:scale(1)}}

/* ═══ ADMIN ═══ */
#adm-wrap{display:none;position:fixed;inset:0;z-index:3000}
.adm-side{position:fixed;left:0;top:0;bottom:0;width:235px;background:rgba(2,8,2,.99);border-right:1px solid var(--border);padding:1.1rem 0;z-index:3001;overflow-y:auto;box-shadow:4px 0 20px rgba(0,255,65,.08)}
.adm-logo{padding:0 1.15rem 1.1rem;border-bottom:1px solid var(--border);margin-bottom:.7rem}
.adm-logo .t{font-family:'Orbitron',monospace;color:var(--gold);font-size:.88rem;font-weight:700;text-shadow:var(--glow)}
.adm-logo small{display:block;color:var(--text3);font-size:.58rem;margin-top:.1rem;font-family:'Share Tech Mono',monospace}
.adm-nav{display:flex;align-items:center;gap:.58rem;padding:.58rem 1.15rem;color:var(--text3);cursor:pointer;font-size:.74rem;transition:all .2s;border-left:2px solid transparent;font-family:'Share Tech Mono',monospace;text-transform:uppercase;letter-spacing:.05em}
.adm-nav.active,.adm-nav:hover{color:var(--gold);background:rgba(0,255,65,.05);border-left-color:var(--gold)}
.adm-section-label{padding:.3rem 1.15rem;font-size:.55rem;color:var(--text3);text-transform:uppercase;letter-spacing:.12em;font-weight:700;margin-top:.4rem;font-family:'Orbitron',monospace}
.adm-main{position:fixed;left:235px;top:0;right:0;bottom:0;background:rgba(2,8,2,.99);overflow-y:auto;padding:1.4rem;z-index:3001}

/* NAV */
nav{position:fixed;top:0;width:100%;z-index:1000;background:rgba(247,244,255,.96);backdrop-filter:blur(16px);border-bottom:1px solid rgba(100,80,180,.15);padding:0 1.5rem;height:62px;display:flex;align-items:center;justify-content:space-between;box-shadow:0 2px 20px rgba(91,110,245,.08)}
.nav-brand{display:flex;align-items:center;gap:.75rem}
.nav-logo{width:40px;height:40px;border-radius:9px;background:var(--grad1);display:flex;align-items:center;justify-content:center;position:relative;box-shadow:0 4px 14px rgba(91,110,245,.35)}
.nav-logo::after{content:'';position:absolute;inset:2px;border-radius:7px;background:rgba(247,244,255,.15)}
.nav-logo span{position:relative;z-index:1;color:#fff;font-family:'Rajdhani',sans-serif;font-size:.95rem;font-weight:700}
.brand-name{font-family:'Rajdhani',sans-serif;font-size:1rem;font-weight:700;color:var(--text);letter-spacing:.05em}
.brand-sub{font-size:.62rem;color:var(--purple);letter-spacing:.07em;font-weight:600}
.nav-links{display:flex;gap:.1rem;list-style:none}
.nav-links a{color:var(--text2);text-decoration:none;font-size:.79rem;font-weight:500;padding:.35rem .68rem;border-radius:4px;transition:color .2s;position:relative}
.nav-links a::after{content:'';position:absolute;bottom:0;left:50%;right:50%;height:2px;background:var(--grad1);transition:all .2s;border-radius:1px}
.nav-links a:hover{color:var(--blue)}.nav-links a:hover::after{left:10%;right:10%}
.nav-r{display:flex;align-items:center;gap:.5rem}
.cv-btn{background:var(--grad1);color:#fff;padding:.42rem 1.1rem;border-radius:6px;font-weight:700;font-size:.79rem;border:none;cursor:pointer;font-family:'Barlow',sans-serif;transition:all .2s;box-shadow:0 4px 14px rgba(91,110,245,.3)}
.cv-btn:hover{transform:translateY(-1px);box-shadow:0 6px 20px rgba(91,110,245,.45)}
.hamburger{display:none;flex-direction:column;gap:5px;cursor:pointer}
.hamburger span{width:22px;height:2px;background:var(--text2)}
.mob-menu{display:none;position:fixed;top:62px;left:0;width:100%;background:rgba(247,244,255,.98);border-bottom:1px solid var(--border);padding:1rem 1.5rem;z-index:999;box-shadow:0 8px 20px rgba(91,110,245,.1)}
.mob-menu a{display:block;color:var(--text2);text-decoration:none;padding:.6rem 0;border-bottom:1px solid var(--border);font-size:.88rem}
.mob-menu.open{display:block}

/* HERO */
.hero{min-height:100vh;padding-top:62px;background:
  radial-gradient(ellipse at 70% 40%,rgba(91,110,245,.1) 0%,transparent 55%),
  radial-gradient(ellipse at 20% 70%,rgba(12,184,160,.08) 0%,transparent 50%),
  radial-gradient(ellipse at 90% 80%,rgba(224,69,138,.07) 0%,transparent 45%),
  var(--bg);position:relative;overflow:hidden}
.hero-grid{display:grid;grid-template-columns:1.1fr 1fr;min-height:calc(100vh - 62px);max-width:1400px;margin:0 auto;padding:2rem;gap:2rem;align-items:center}
.hero-eyebrow{display:flex;align-items:center;gap:.75rem;margin-bottom:1.2rem}
.ey-line{width:30px;height:2px;background:var(--grad1)}
.ey-text{font-size:.68rem;letter-spacing:.14em;text-transform:uppercase;color:var(--purple);font-weight:700}
.hero-name{font-family:'Barlow Condensed',sans-serif;font-size:clamp(2.8rem,5.5vw,5.2rem);font-weight:800;line-height:.94;margin-bottom:.6rem}
.hero-name .fn{background:var(--grad1);-webkit-background-clip:text;-webkit-text-fill-color:transparent;display:block}
.hero-name .ln{color:var(--text);display:block}
.hero-title{font-size:1rem;color:var(--text2);font-weight:400;margin-bottom:1rem}
.washing-tags{display:flex;align-items:center;gap:.45rem;margin-bottom:1rem;flex-wrap:wrap}
.wt{padding:.26rem .82rem;border-radius:20px;font-size:.78rem;font-weight:600;border:1px solid}
.wt-b{background:rgba(91,110,245,.1);border-color:rgba(91,110,245,.3);color:var(--blue)}
.wt-g{background:rgba(12,184,160,.1);border-color:rgba(12,184,160,.35);color:var(--teal)}
.wt-sep{color:var(--purple);font-weight:700}
.pgd-badge{display:inline-flex;align-items:center;gap:.75rem;background:linear-gradient(135deg,rgba(139,92,246,.08),rgba(91,110,245,.05));border:1px solid rgba(139,92,246,.25);padding:.55rem 1rem;border-radius:8px;margin-bottom:1.15rem}
.pgd-title{font-weight:700;font-size:.86rem;background:var(--grad4);-webkit-background-clip:text;-webkit-text-fill-color:transparent;font-family:'Barlow Condensed',sans-serif;letter-spacing:.05em}
.pgd-sub{font-size:.68rem;color:var(--text2)}
.hero-perks{display:flex;flex-direction:column;gap:.42rem;margin-bottom:1.4rem}
.perk{display:flex;align-items:center;gap:.55rem;font-size:.84rem;color:var(--text2)}
.perk strong{color:var(--purple);font-weight:700}
.hero-btns{display:flex;gap:.65rem;flex-wrap:wrap}
.hbtn-p{background:var(--grad1);color:#fff;padding:.62rem 1.35rem;border-radius:8px;font-weight:700;font-size:.84rem;border:none;cursor:pointer;font-family:'Barlow',sans-serif;transition:all .2s;box-shadow:0 4px 16px rgba(91,110,245,.35)}
.hbtn-p:hover{transform:translateY(-2px);box-shadow:0 8px 24px rgba(91,110,245,.5)}
.hbtn-o{background:transparent;color:var(--blue);padding:.62rem 1.15rem;border-radius:8px;font-weight:600;font-size:.84rem;border:1.5px solid rgba(91,110,245,.4);cursor:pointer;font-family:'Barlow',sans-serif;transition:all .2s}
.hbtn-o:hover{border-color:var(--purple);color:var(--purple);background:rgba(139,92,246,.06)}
.hbtn-g{background:var(--grad2);color:#fff;padding:.62rem 1.15rem;border-radius:8px;font-weight:700;font-size:.84rem;border:none;cursor:pointer;font-family:'Barlow',sans-serif;transition:all .2s;box-shadow:0 4px 16px rgba(12,184,160,.3)}
.hbtn-g:hover{transform:translateY(-2px);box-shadow:0 8px 24px rgba(12,184,160,.45)}

/* HERO CIRCULAR PHOTO */
.hero-right{position:relative;display:flex;align-items:center;justify-content:center}
.hero-photo-area{position:relative;width:340px;height:340px}
.photo-ring-outer{position:absolute;inset:-18px;border-radius:50%;border:2px solid transparent;background:linear-gradient(white,white) padding-box,linear-gradient(135deg,#5b6ef5,#e0458a,#0cb8a0,#8b5cf6) border-box;animation:ring-spin 8s linear infinite}
@keyframes ring-spin{to{transform:rotate(360deg)}}
.photo-ring-dash{position:absolute;inset:-8px;border-radius:50%;border:1.5px dashed rgba(139,92,246,.4);animation:ring-spin 14s linear infinite reverse}
.photo-circle{width:340px;height:340px;border-radius:50%;overflow:hidden;background:linear-gradient(160deg,#e8e4ff,#ddf4f0);border:4px solid rgba(91,110,245,.3);box-shadow:0 0 0 1px rgba(224,69,138,.2),0 0 40px rgba(91,110,245,.2),0 0 80px rgba(12,184,160,.1),inset 0 0 40px rgba(255,255,255,.5);position:relative;display:flex;align-items:center;justify-content:center}
.photo-circle img#heroPhotoImg{width:100%;height:100%;object-fit:cover;object-position:top center;display:none;position:absolute;inset:0}
.photo-circle .photo-placeholder-inner{display:flex;flex-direction:column;align-items:center;justify-content:center;gap:.6rem;pointer-events:none;z-index:2}
.photo-placeholder-inner .icon{font-size:5.5rem;opacity:.4}
.photo-placeholder-inner .hint{font-size:.68rem;color:var(--text3);text-align:center;line-height:1.6;background:rgba(255,255,255,.7);border-radius:20px;padding:.4rem 1rem}
.photo-circle::after{content:'';position:absolute;bottom:0;left:0;right:0;height:30%;background:linear-gradient(to top,rgba(91,110,245,.15),transparent);pointer-events:none;border-radius:0 0 50% 50%;z-index:1}
/* Orbit Bubbles */
.ob{position:absolute;z-index:10;background:rgba(255,255,255,.92);border:1.5px solid rgba(91,110,245,.3);border-radius:50%;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;backdrop-filter:blur(8px);box-shadow:0 4px 20px rgba(91,110,245,.15)}
.ob1{width:84px;height:84px;top:-10px;left:-15px;animation:obf1 5s ease-in-out infinite;border-color:rgba(91,110,245,.4)}
.ob2{width:78px;height:78px;bottom:30px;left:-20px;border-color:rgba(12,184,160,.4);animation:obf2 6s ease-in-out infinite}
.ob3{width:88px;height:88px;top:-5px;right:-15px;border-color:rgba(224,69,138,.4);animation:obf1 4.5s ease-in-out infinite .5s}
.ob4{width:80px;height:80px;bottom:20px;right:-18px;border-color:rgba(139,92,246,.4);animation:obf2 5.5s ease-in-out infinite 1s}
@keyframes obf1{0%,100%{transform:translateY(0)}50%{transform:translateY(-10px)}}
@keyframes obf2{0%,100%{transform:translateY(0)}50%{transform:translateY(9px)}}
.ob-num{font-family:'Barlow Condensed',sans-serif;font-size:1.35rem;font-weight:800;line-height:1}
.ob1 .ob-num,.ob4 .ob-num{color:var(--blue)}
.ob2 .ob-num{color:var(--teal)}
.ob3 .ob-num{color:var(--pink)}
.ob-lbl{font-size:.56rem;color:var(--text3);line-height:1.2;margin-top:2px;padding:0 4px}

/* STATS BAR */
.stats-bar{background:linear-gradient(135deg,rgba(91,110,245,.08),rgba(12,184,160,.06),rgba(224,69,138,.06));border-top:1px solid rgba(91,110,245,.15);border-bottom:1px solid rgba(91,110,245,.15);padding:.82rem 2rem}
.stats-inner{max-width:1400px;margin:0 auto;display:flex;justify-content:space-around;flex-wrap:wrap;gap:.4rem}
.si{display:flex;align-items:center;gap:.7rem;padding:.2rem .9rem;border-right:1px solid rgba(91,110,245,.15)}
.si:last-child{border-right:none}
.si-num{font-family:'Barlow Condensed',sans-serif;font-size:1.4rem;font-weight:700;line-height:1}
.si:nth-child(1) .si-num{color:var(--blue)}
.si:nth-child(2) .si-num{color:var(--teal)}
.si:nth-child(3) .si-num{color:var(--pink)}
.si:nth-child(4) .si-num{color:var(--purple)}
.si:nth-child(5) .si-num{color:var(--orange)}
.si-lbl{font-size:.62rem;color:var(--text3);text-transform:uppercase;letter-spacing:.06em;line-height:1.2}

/* MAIN */
.main{max-width:1400px;margin:0 auto;padding:1.6rem}
.col3{display:grid;grid-template-columns:1.3fr 1fr .85fr;gap:1.2rem;align-items:start}

/* DARK CARD → LIGHT CARD */
.dc{background:var(--card);border:1px solid var(--border);border-radius:14px;overflow:hidden;box-shadow:0 2px 16px rgba(91,110,245,.07)}
.dc-head{padding:.82rem 1.15rem;border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:space-between;background:linear-gradient(135deg,rgba(91,110,245,.05),rgba(224,69,138,.03))}
.dc-title{font-family:'Barlow Condensed',sans-serif;font-size:.93rem;font-weight:700;letter-spacing:.07em;text-transform:uppercase;color:var(--text)}
.dc-line{width:26px;height:2px;background:var(--grad1)}

/* EXPERTISE */
.etabs{display:flex;gap:.32rem;padding:.65rem 1.15rem;border-bottom:1px solid var(--border);flex-wrap:wrap}
.etab{padding:.26rem .8rem;border-radius:20px;font-size:.74rem;font-weight:600;cursor:pointer;transition:all .2s;border:1.5px solid var(--border);background:transparent;color:var(--text2);font-family:'Barlow',sans-serif}
.etab.active{background:var(--grad1);color:#fff;border-color:transparent;box-shadow:0 3px 12px rgba(91,110,245,.35)}
.etab:hover:not(.active){border-color:var(--blue);color:var(--blue)}
.exp-body{padding:.9rem 1.15rem}
.exp-list{list-style:none;display:flex;flex-direction:column;gap:.38rem}
.exp-list li{display:flex;align-items:center;gap:.52rem;font-size:.81rem;color:var(--text2);padding:.3rem 0;border-bottom:1px solid rgba(91,110,245,.08)}
.exp-list li:last-child{border-bottom:none}
.exp-list li strong{color:var(--blue);font-weight:700}

/* R&D */
.rnd-body{padding:.95rem 1.15rem}
.rnd-ptitle{font-weight:700;font-size:.9rem;color:var(--text);margin-bottom:.32rem}
.approved-b{display:inline-flex;gap:.35rem;align-items:center;background:rgba(12,184,160,.1);border:1px solid rgba(12,184,160,.35);padding:.16rem .56rem;border-radius:20px;font-size:.62rem;font-weight:700;color:var(--teal);letter-spacing:.05em;margin-bottom:.72rem}
.rnd-img-box{width:100%;height:110px;border-radius:10px;overflow:hidden;margin-bottom:.72rem;border:1px solid rgba(91,110,245,.15);background:linear-gradient(135deg,#e8f5e9,#ddf4f0);display:flex;align-items:center;justify-content:center;position:relative;cursor:pointer}
.rnd-img-box img{width:100%;height:100%;object-fit:cover;display:none}
.rnd-img-ph{font-size:2.8rem}
.rnd-points{display:flex;flex-direction:column;gap:.35rem;margin-bottom:.85rem}
.rnd-pt{display:flex;align-items:center;gap:.45rem;font-size:.76rem;color:var(--text2)}
.rnd-dot{width:5px;height:5px;border-radius:50%;background:var(--teal);flex-shrink:0}
.rnd-cta{width:100%;background:var(--grad2);color:#fff;padding:.5rem;border-radius:8px;font-weight:700;font-size:.78rem;border:none;cursor:pointer;font-family:'Barlow',sans-serif;display:flex;align-items:center;justify-content:center;gap:.35rem;transition:all .2s;box-shadow:0 3px 12px rgba(12,184,160,.3)}
.rnd-cta:hover{transform:translateY(-1px);box-shadow:0 5px 18px rgba(12,184,160,.45)}

/* EXP TIMELINE */
.etl{padding:.9rem 1.15rem;display:flex;flex-direction:column}
.etl-item{position:relative;padding-left:1rem;padding-bottom:1.05rem;border-left:2px solid rgba(91,110,245,.2)}
.etl-item:last-child{border-left:2px solid transparent;padding-bottom:0}
.etl-dot{position:absolute;left:-5px;top:4px;width:8px;height:8px;border-radius:50%;background:var(--purple);box-shadow:0 0 8px rgba(139,92,246,.5)}
.etl-item.cur .etl-dot{background:var(--teal);box-shadow:0 0 8px rgba(12,184,160,.6);animation:pdot 2s infinite}
@keyframes pdot{0%,100%{box-shadow:0 0 8px rgba(12,184,160,.6)}50%{box-shadow:0 0 16px rgba(12,184,160,.9)}}
.etl-role{font-weight:700;font-size:.84rem;color:var(--text);line-height:1.2}
.etl-co{font-size:.74rem;font-weight:600;color:var(--blue);margin-top:.16rem}
.etl-date{font-size:.66rem;color:var(--text3);margin-top:.1rem}
.etl-buyer{font-size:.64rem;color:var(--teal);margin-top:.2rem;display:inline-block;background:rgba(12,184,160,.1);padding:.1rem .4rem;border-radius:3px;font-weight:600}

/* CERT SIDEBAR */
.cert-sidebar{padding:.65rem 1.15rem;display:flex;flex-direction:column;gap:.38rem}
.cert-si{display:flex;align-items:center;gap:.52rem;padding:.42rem 0;border-bottom:1px solid rgba(91,110,245,.1);cursor:pointer;transition:all .2s}
.cert-si:last-child{border-bottom:none}
.cert-si:hover{padding-left:.2rem}
.cert-si-img{width:30px;height:30px;border-radius:6px;overflow:hidden;flex-shrink:0;background:rgba(91,110,245,.1);display:flex;align-items:center;justify-content:center;font-size:.88rem}
.cert-si-img img{width:100%;height:100%;object-fit:cover;border-radius:6px}
.cert-si-name{font-size:.74rem;color:var(--text);font-weight:600;line-height:1.3}
.cert-si-org{font-size:.63rem;color:var(--purple)}
.cert-arrow{color:var(--text3);font-size:.7rem;margin-left:auto;transition:all .2s}
.cert-si:hover .cert-arrow{color:var(--blue);transform:translateX(3px)}
.view-all{width:100%;background:rgba(91,110,245,.07);color:var(--blue);padding:.48rem;border-radius:0 0 12px 12px;font-weight:600;font-size:.73rem;border:none;border-top:1px solid rgba(91,110,245,.15);cursor:pointer;font-family:'Barlow',sans-serif;letter-spacing:.05em;text-transform:uppercase;transition:background .2s}
.view-all:hover{background:rgba(91,110,245,.14)}

/* PORTFOLIO */
.port-sec{margin-top:1.3rem}
.sec-hdr{display:flex;align-items:center;justify-content:space-between;margin-bottom:.9rem}
.sec-title-wrap{display:flex;align-items:center;gap:.65rem}
.stl{width:20px;height:2px;background:linear-gradient(90deg,#5b6ef5,#e0458a)}
.str{flex:1;height:1px;background:linear-gradient(90deg,rgba(91,110,245,.2),transparent)}
.sec-ttl{font-family:'Barlow Condensed',sans-serif;font-size:1rem;font-weight:700;letter-spacing:.1em;text-transform:uppercase;color:var(--text)}
.pf-btns{display:flex;gap:.32rem;flex-wrap:wrap}
.pf-btn{padding:.24rem .72rem;border-radius:20px;font-size:.68rem;font-weight:600;cursor:pointer;transition:all .2s;border:1.5px solid rgba(91,110,245,.2);background:transparent;color:var(--text3);font-family:'Barlow',sans-serif}
.pf-btn.active,.pf-btn:hover{background:linear-gradient(135deg,#5b6ef5,#e0458a);color:#fff;border-color:transparent;box-shadow:0 3px 10px rgba(91,110,245,.3)}
.port-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(152px,1fr));gap:.65rem}
.port-card{border-radius:10px;overflow:hidden;position:relative;cursor:pointer;transition:all .3s;border:1px solid rgba(91,110,245,.15);background:#fff;box-shadow:0 2px 10px rgba(91,110,245,.07)}
.port-card:hover{transform:translateY(-3px);border-color:rgba(91,110,245,.3);box-shadow:0 8px 24px rgba(91,110,245,.15)}
.port-img{height:105px;position:relative;overflow:hidden;background:linear-gradient(135deg,rgba(91,110,245,.08),rgba(224,69,138,.06));display:flex;align-items:center;justify-content:center;font-size:2.1rem}
.port-img img{width:100%;height:100%;object-fit:cover;position:absolute;inset:0}
.port-ov{position:absolute;inset:0;background:linear-gradient(to top,rgba(255,255,255,.9) 0%,transparent 60%)}
.port-lbl{position:absolute;bottom:0;left:0;right:0;padding:.42rem;text-align:center;z-index:2}
.port-name{font-size:.69rem;font-weight:700;color:var(--text);display:block}
.port-tech{font-size:.59rem;color:var(--blue);display:block;margin-top:1px;font-weight:600}

/* FULL SECTIONS */
.full-sec{padding:2.4rem 2rem}
.full-sec-inner{max-width:1400px;margin:0 auto}
.fs-hdr{display:flex;align-items:center;gap:.65rem;margin-bottom:.45rem}
.fs-sub{color:var(--text3);font-size:.83rem;margin-bottom:1.6rem}

/* CERTS GRID */
.certs-full-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(230px,1fr));gap:.85rem}
.cert-card{background:#fff;border:1px solid rgba(91,110,245,.15);border-radius:12px;overflow:hidden;cursor:pointer;transition:all .3s;box-shadow:0 2px 12px rgba(91,110,245,.07)}
.cert-card:hover{transform:translateY(-3px);border-color:rgba(91,110,245,.3);box-shadow:0 10px 28px rgba(91,110,245,.15)}
.cert-card-img{height:115px;background:linear-gradient(135deg,rgba(91,110,245,.1),rgba(224,69,138,.07));display:flex;align-items:center;justify-content:center;font-size:2.7rem;overflow:hidden}
.cert-card-img img{width:100%;height:100%;object-fit:cover}
.cert-card-body{padding:.85rem .95rem}
.cert-card-org{font-size:.63rem;color:var(--purple);font-weight:700;letter-spacing:.07em;text-transform:uppercase;margin-bottom:.22rem}
.cert-card-name{font-weight:700;font-size:.8rem;color:var(--text);line-height:1.4}

/* CASES */
.cases-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:.85rem}
.case-card{background:#fff;border:1px solid rgba(91,110,245,.15);border-radius:12px;overflow:hidden;transition:all .3s;box-shadow:0 2px 12px rgba(91,110,245,.07)}
.case-card:hover{transform:translateY(-3px);box-shadow:0 12px 30px rgba(91,110,245,.15)}
.case-head{background:linear-gradient(135deg,rgba(91,110,245,.07),rgba(224,69,138,.04));padding:.95rem 1.1rem;border-bottom:1px solid rgba(91,110,245,.1)}
.case-buyer{font-size:.6rem;letter-spacing:.12em;text-transform:uppercase;color:var(--pink);font-weight:700;margin-bottom:.26rem}
.case-title{font-family:'Barlow Condensed',sans-serif;font-size:.98rem;font-weight:700;color:var(--text)}
.case-body{padding:.95rem 1.1rem}
.case-row{display:flex;gap:.45rem;padding:.32rem 0;border-bottom:1px solid rgba(91,110,245,.08);font-size:.76rem}
.case-row:last-of-type{border-bottom:none}
.cl{color:var(--text3);min-width:105px;flex-shrink:0;font-weight:500}
.cv2{color:var(--text)}
.case-result{background:rgba(12,184,160,.08);border-left:3px solid #0cb8a0;padding:.52rem .75rem;border-radius:0 6px 6px 0;margin-top:.65rem;font-size:.74rem;color:#0cb8a0;line-height:1.6;font-weight:600}

/* SKILLS */
.skills-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(165px,1fr));gap:.7rem}
.sk-card{background:#fff;border:1px solid rgba(91,110,245,.15);border-radius:10px;padding:.85rem;transition:all .25s;position:relative;overflow:hidden;box-shadow:0 2px 10px rgba(91,110,245,.06)}
.sk-card:nth-child(4n+1)::before{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;background:linear-gradient(180deg,#5b6ef5,#e0458a)}
.sk-card:nth-child(4n+2)::before{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;background:linear-gradient(180deg,#0cb8a0,#5b6ef5)}
.sk-card:nth-child(4n+3)::before{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;background:linear-gradient(180deg,#f07030,#e0458a)}
.sk-card:nth-child(4n+4)::before{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;background:linear-gradient(180deg,#8b5cf6,#0cb8a0)}
.sk-card:hover{transform:translateY(-2px);box-shadow:0 8px 22px rgba(91,110,245,.15)}
.sk-icon{font-size:1.15rem;margin-bottom:.35rem}
.sk-name{font-size:.78rem;font-weight:600;color:var(--text);margin-bottom:.42rem}
.sk-bar{height:3px;background:rgba(91,110,245,.1);border-radius:2px;overflow:hidden}
.sk-fill{height:100%;background:linear-gradient(90deg,#5b6ef5,#e0458a);border-radius:2px;width:0;transition:width 1.2s ease}

/* BUYERS */
.buyers-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(260px,1fr));gap:.85rem}
.buyer-card{background:#fff;border:1px solid rgba(91,110,245,.15);border-radius:12px;padding:1.4rem;transition:all .3s;position:relative;overflow:hidden;box-shadow:0 2px 12px rgba(91,110,245,.07)}
.buyer-card:nth-child(3n+1)::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,#5b6ef5,#e0458a)}
.buyer-card:nth-child(3n+2)::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,#0cb8a0,#5b6ef5)}
.buyer-card:nth-child(3n+3)::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;background:linear-gradient(90deg,#f07030,#e0458a)}
.buyer-card:hover{transform:translateY(-3px);box-shadow:0 12px 30px rgba(91,110,245,.18)}
.buyer-card .logo{width:44px;height:44px;border-radius:9px;background:rgba(91,110,245,.1);display:flex;align-items:center;justify-content:center;font-size:1.3rem;margin-bottom:.85rem;overflow:hidden}
.buyer-card .logo img{width:100%;height:100%;object-fit:cover;border-radius:9px}
.buyer-name{font-family:'Barlow Condensed',sans-serif;font-size:1.05rem;font-weight:700;color:var(--text);margin-bottom:.2rem}
.buyer-proj{color:var(--blue);font-size:.8rem;font-weight:600;margin-bottom:.65rem}
.buyer-spec{font-size:.78rem;color:var(--text2);line-height:1.65}
.q-badge{display:inline-flex;align-items:center;gap:.3rem;background:rgba(12,184,160,.1);color:#0cb8a0;padding:.22rem .55rem;border-radius:4px;font-size:.68rem;font-weight:700;margin-top:.65rem}

/* CONTACT */
.contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:1.8rem;align-items:start}
.ci{display:flex;align-items:center;gap:.82rem;padding:.82rem;background:#fff;border:1px solid rgba(91,110,245,.15);border-radius:10px;margin-bottom:.65rem;box-shadow:0 2px 8px rgba(91,110,245,.06)}
.ci-icon{width:34px;height:34px;border-radius:7px;background:rgba(91,110,245,.1);display:flex;align-items:center;justify-content:center;font-size:.95rem;flex-shrink:0}
.ci-lbl{font-size:.62rem;color:var(--text3);text-transform:uppercase;letter-spacing:.05em}
.ci-val{color:var(--text);font-weight:600;font-size:.83rem}
.cf-inp{width:100%;background:#f7f4ff;border:1.5px solid rgba(91,110,245,.18);border-radius:8px;padding:.58rem .85rem;font-family:'Barlow',sans-serif;font-size:.81rem;color:var(--text);outline:none;transition:border-color .2s;margin-bottom:.65rem}
.cf-inp:focus{border-color:rgba(91,110,245,.45)}
.cf-lbl{display:block;font-size:.66rem;color:var(--text3);text-transform:uppercase;letter-spacing:.05em;margin-bottom:.28rem}
.cf-sub{width:100%;background:linear-gradient(135deg,#5b6ef5,#e0458a);color:#fff;padding:.65rem;border-radius:8px;font-weight:700;font-size:.82rem;border:none;cursor:pointer;font-family:'Barlow',sans-serif;transition:all .2s;box-shadow:0 4px 14px rgba(91,110,245,.3)}
.cf-sub:hover{transform:translateY(-1px);box-shadow:0 6px 20px rgba(91,110,245,.45)}

/* FOOTER */
.footer-bar{background:linear-gradient(135deg,rgba(91,110,245,.07),rgba(224,69,138,.05),rgba(12,184,160,.04));border-top:1.5px solid rgba(91,110,245,.15);padding:.78rem 2rem;display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:.7rem}
.fc-item{display:flex;align-items:center;gap:.38rem;font-size:.76rem;color:var(--text2)}
.footer-contacts{display:flex;gap:1.4rem;flex-wrap:wrap}
.footer-cta{background:linear-gradient(135deg,#5b6ef5,#e0458a);color:#fff;padding:.48rem 1.15rem;border-radius:6px;font-weight:700;font-size:.78rem;border:none;cursor:pointer;font-family:'Barlow',sans-serif;transition:all .2s;box-shadow:0 3px 12px rgba(91,110,245,.3)}
.footer-cta:hover{transform:translateY(-1px);box-shadow:0 5px 18px rgba(91,110,245,.45)}
.soc-btns{display:flex;gap:.42rem}
.soc-b{width:29px;height:29px;border-radius:6px;background:#fff;border:1px solid rgba(91,110,245,.2);display:flex;align-items:center;justify-content:center;font-size:.73rem;cursor:pointer;color:var(--text2);transition:all .2s}
.soc-b:hover{border-color:var(--blue);color:var(--blue)}

/* AI CHAT */
.chat-wrap{position:fixed;bottom:1.4rem;right:1.4rem;z-index:2000}
.chat-toggle{width:52px;height:52px;border-radius:50%;background:linear-gradient(135deg,#5b6ef5,#e0458a);border:none;cursor:pointer;box-shadow:0 5px 18px rgba(91,110,245,.45);transition:all .3s;display:flex;align-items:center;justify-content:center;color:#fff;font-family:'Barlow Condensed',sans-serif;font-weight:800;font-size:1rem;letter-spacing:.02em}
.chat-toggle:hover{transform:scale(1.07);box-shadow:0 8px 24px rgba(91,110,245,.55)}
.chat-win{position:absolute;bottom:62px;right:0;width:308px;background:#fff;border:1px solid rgba(91,110,245,.2);border-radius:16px;box-shadow:0 18px 55px rgba(91,110,245,.18);display:none;flex-direction:column;overflow:hidden}
.chat-win.open{display:flex;animation:cfade .3s ease}
@keyframes cfade{from{opacity:0;transform:translateY(12px) scale(.97)}to{opacity:1;transform:none}}
.chat-hdr{background:linear-gradient(135deg,rgba(91,110,245,.12),rgba(224,69,138,.06));padding:.82rem .95rem;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid rgba(91,110,245,.12)}
.chat-av{width:32px;height:32px;border-radius:50%;background:linear-gradient(135deg,#5b6ef5,#e0458a);display:flex;align-items:center;justify-content:center;color:#fff;font-family:'Barlow Condensed',sans-serif;font-weight:800;font-size:.78rem;flex-shrink:0}
.chat-hdr-name{font-weight:700;font-size:.82rem;color:var(--text)}
.chat-hdr-st{font-size:.65rem;color:#0cb8a0;font-weight:600}
.chat-close{background:none;border:none;color:var(--text3);cursor:pointer;font-size:1.05rem;padding:0}
.chat-chips{padding:.42rem;display:flex;flex-wrap:wrap;gap:.26rem;border-bottom:1px solid rgba(91,110,245,.1);background:rgba(91,110,245,.03)}
.chip{padding:.16rem .48rem;border-radius:12px;border:1px solid rgba(91,110,245,.3);color:var(--blue);font-size:.64rem;cursor:pointer;background:transparent;transition:all .2s;font-family:'Barlow',sans-serif}
.chip:hover{background:rgba(91,110,245,.1)}
.chat-msgs{height:225px;overflow-y:auto;padding:.65rem;display:flex;flex-direction:column;gap:.52rem;background:#fafbff}
.chat-msgs::-webkit-scrollbar{width:3px}
.chat-msgs::-webkit-scrollbar-thumb{background:rgba(91,110,245,.2)}
.cm{max-width:84%}
.cm.bot{align-self:flex-start}.cm.user{align-self:flex-end}
.cm-b{padding:.48rem .72rem;border-radius:10px;font-size:.75rem;line-height:1.55}
.cm.bot .cm-b{background:rgba(91,110,245,.08);color:var(--text);border:1px solid rgba(91,110,245,.15);border-radius:3px 10px 10px 10px}
.cm.user .cm-b{background:linear-gradient(135deg,#5b6ef5,#e0458a);color:#fff;border-radius:10px 3px 10px 10px}
.chat-inp-row{padding:.52rem;border-top:1px solid rgba(91,110,245,.1);display:flex;gap:.38rem;background:#fff}
.chat-inp{flex:1;background:rgba(91,110,245,.05);border:1.5px solid rgba(91,110,245,.15);border-radius:20px;padding:.4rem .7rem;font-size:.74rem;color:var(--text);outline:none;font-family:'Barlow',sans-serif}
.chat-inp:focus{border-color:rgba(91,110,245,.4)}
.chat-send{width:28px;height:28px;border-radius:50%;background:linear-gradient(135deg,#5b6ef5,#e0458a);border:none;color:#fff;cursor:pointer;font-size:.76rem;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.typing{display:flex;gap:3px;padding:.22rem 0}
.td{width:5px;height:5px;border-radius:50%;background:rgba(91,110,245,.4);animation:tdb 1.4s infinite}
.td:nth-child(2){animation-delay:.2s}.td:nth-child(3){animation-delay:.4s}
@keyframes tdb{0%,80%,100%{transform:scale(0)}40%{transform:scale(1)}}

/* ═══ ADMIN ═══ */
#adm-wrap{display:none;position:fixed;inset:0;z-index:3000}
.adm-side{position:fixed;left:0;top:0;bottom:0;width:235px;background:#fff;border-right:1.5px solid rgba(91,110,245,.15);padding:1.1rem 0;z-index:3001;overflow-y:auto;box-shadow:4px 0 20px rgba(91,110,245,.08)}
.adm-logo{padding:0 1.15rem 1.1rem;border-bottom:1px solid rgba(91,110,245,.12);margin-bottom:.7rem}
.adm-logo .t{font-family:'Rajdhani',sans-serif;background:linear-gradient(135deg,#5b6ef5,#e0458a);-webkit-background-clip:text;-webkit-text-fill-color:transparent;font-size:.95rem;font-weight:700}
.adm-logo small{display:block;color:var(--text3);font-size:.61rem;margin-top:.1rem}
.adm-nav{display:flex;align-items:center;gap:.58rem;padding:.58rem 1.15rem;color:var(--text2);cursor:pointer;font-size:.78rem;transition:all .2s;border-left:2px solid transparent}
.adm-nav.active,.adm-nav:hover{color:var(--blue);background:rgba(91,110,245,.06);border-left-color:#5b6ef5}
.adm-section-label{padding:.3rem 1.15rem;font-size:.58rem;color:var(--text3);text-transform:uppercase;letter-spacing:.1em;font-weight:700;margin-top:.4rem}
.adm-main{position:fixed;left:235px;top:0;right:0;bottom:0;background:#f7f4ff;overflow-y:auto;padding:1.4rem;z-index:3001}
.adm-topbar{display:flex;justify-content:space-between;align-items:center;margin-bottom:1.3rem;padding-bottom:.85rem;border-bottom:1px solid rgba(91,110,245,.15)}
.adm-topbar h1{font-family:'Orbitron',monospace;font-size:1.1rem;font-weight:700;color:var(--gold);text-transform:uppercase;letter-spacing:.1em;text-shadow:var(--glow)}
.adm-close{background:transparent;color:var(--text2);border:1px solid var(--border);padding:.36rem .88rem;border-radius:2px;cursor:pointer;font-size:.72rem;font-family:'Share Tech Mono',monospace;text-transform:uppercase}
.adm-topbar{display:flex;justify-content:space-between;align-items:center;margin-bottom:1.3rem;padding-bottom:.85rem;border-bottom:1px solid var(--border)}
.adm-panel{display:none}
.adm-panel.active{display:block}
.adm-stats{display:grid;grid-template-columns:repeat(auto-fill,minmax(135px,1fr));gap:.68rem;margin-bottom:1.3rem}
.adm-sc{background:var(--card);border:1px solid var(--border);border-radius:4px;padding:.85rem;box-shadow:0 2px 8px rgba(0,255,65,.04)}
.adm-sc .n{font-family:'Orbitron',monospace;font-size:1.5rem;font-weight:700;color:var(--gold);text-shadow:var(--glow)}
.adm-sc .l{font-size:.6rem;color:var(--text3);text-transform:uppercase;letter-spacing:.08em;font-family:'Share Tech Mono',monospace}
.afc{background:var(--card);border:1px solid var(--border);border-radius:4px;padding:1.3rem;margin-bottom:1.1rem}
.afc h3{font-family:'Orbitron',monospace;font-size:.82rem;font-weight:700;text-transform:uppercase;letter-spacing:.08em;color:var(--gold);text-shadow:var(--glow);margin-bottom:1rem;display:flex;align-items:center;gap:.45em}
.aform-grid{display:grid;grid-template-columns:1fr 1fr;gap:.68rem}
.aform-full{grid-column:1/-1}
.al{display:block;font-size:.62rem;color:var(--text3);text-transform:uppercase;letter-spacing:.08em;margin-bottom:.28rem;font-weight:600;font-family:'Share Tech Mono',monospace}
.ai{width:100%;background:rgba(0,255,65,.03);border:1px solid var(--border);border-radius:2px;padding:.55rem .82rem;font-family:'Share Tech Mono',monospace;font-size:.77rem;color:var(--text);outline:none;transition:border-color .2s}
.ai:focus{border-color:var(--gold);box-shadow:var(--glow)}
.ai::placeholder{color:var(--text3)}
select.ai option{background:#020c02;color:var(--text)}
textarea.ai{resize:vertical;min-height:72px}
.img-field-wrap{position:relative}
.img-url-inp{padding-right:2.5rem!important}
.img-prev-row{display:flex;align-items:center;gap:.7rem;margin-top:.48rem}
.img-prev-box{width:52px;height:52px;border-radius:2px;background:rgba(0,255,65,.05);border:1px solid var(--border);display:flex;align-items:center;justify-content:center;overflow:hidden;flex-shrink:0;font-size:1.4rem}
.img-prev-box img{width:100%;height:100%;object-fit:cover}
.img-hint-text{font-size:.65rem;color:var(--text3);line-height:1.6;font-family:'Share Tech Mono',monospace}
.img-hint-text a{color:var(--teal);text-decoration:none}
.abtn-save{background:transparent;color:var(--gold);border:1px solid var(--gold);padding:.54rem 1.3rem;border-radius:2px;font-weight:700;font-size:.72rem;cursor:pointer;font-family:'Orbitron',monospace;transition:all .2s;margin-right:.45rem;box-shadow:var(--glow);letter-spacing:.06em;text-transform:uppercase}
.abtn-save:hover{background:rgba(0,255,65,.1);transform:translateY(-1px)}
.abtn-cancel{background:transparent;color:var(--text3);border:1px solid var(--border);padding:.54rem .95rem;border-radius:2px;font-size:.72rem;cursor:pointer;font-family:'Share Tech Mono',monospace;text-transform:uppercase}
.abtn-gold{background:transparent;color:var(--teal);border:1px solid rgba(0,255,153,.4);padding:.54rem 1.3rem;border-radius:2px;font-weight:700;font-size:.72rem;cursor:pointer;font-family:'Orbitron',monospace;transition:all .2s;text-transform:uppercase;letter-spacing:.06em}
.abtn-gold:hover{background:rgba(0,255,153,.07);box-shadow:0 0 20px rgba(0,255,153,.3)}
.atbl-wrap{background:var(--card);border:1px solid var(--border);border-radius:4px;overflow:hidden;margin-top:.2rem}
.atbl{width:100%;border-collapse:collapse}
.atbl th{background:rgba(0,255,65,.05);color:var(--text3);padding:.56rem .85rem;text-align:left;font-size:.62rem;text-transform:uppercase;letter-spacing:.1em;font-family:'Orbitron',monospace}
.atbl td{padding:.54rem .85rem;border-bottom:1px solid rgba(0,255,65,.06);font-size:.72rem;color:var(--text2);vertical-align:middle;font-family:'Share Tech Mono',monospace}
.atbl tr:last-child td{border-bottom:none}
.atbl tr:hover td{background:rgba(0,255,65,.03)}
.tbl-thumb{width:32px;height:32px;border-radius:2px;object-fit:cover}
.tbl-ph{width:32px;height:32px;border-radius:2px;background:rgba(0,255,65,.07);display:inline-flex;align-items:center;justify-content:center;font-size:.88rem;border:1px solid var(--border)}
.btn-add{background:transparent;color:var(--gold);border:1px solid var(--gold);padding:.42rem .95rem;border-radius:2px;font-weight:600;font-size:.68rem;cursor:pointer;font-family:'Share Tech Mono',monospace;margin-bottom:.7rem;display:inline-flex;align-items:center;gap:.38rem;transition:all .2s;text-transform:uppercase;letter-spacing:.05em}
.btn-add:hover{background:rgba(0,255,65,.08)}
.btn-e{background:rgba(0,229,255,.07);color:var(--blue);border:1px solid rgba(0,229,255,.2);padding:.18rem .48rem;border-radius:2px;font-size:.62rem;cursor:pointer;font-family:'Share Tech Mono',monospace}
.btn-d{background:rgba(255,0,119,.07);color:var(--pink);border:1px solid rgba(255,0,119,.2);padding:.18rem .48rem;border-radius:2px;font-size:.62rem;cursor:pointer;font-family:'Share Tech Mono',monospace}
.btn-up{background:rgba(0,255,153,.07);color:var(--teal);border:1px solid rgba(0,255,153,.2);padding:.18rem .48rem;border-radius:2px;font-size:.62rem;cursor:pointer;font-family:'Share Tech Mono',monospace}
.inline-edit{background:rgba(0,255,65,.03);border:1px solid var(--border);border-radius:4px;padding:1rem;margin-bottom:.8rem}
.info-box{background:rgba(0,255,65,.03);border:1px solid rgba(0,255,65,.2);border-radius:2px;padding:.9rem 1rem;margin-bottom:1rem}
.info-box .ib-title{font-size:.72rem;font-weight:700;color:var(--teal);margin-bottom:.42rem;font-family:'Orbitron',monospace;letter-spacing:.05em}
.info-box .ib-text{font-size:.7rem;color:var(--text2);line-height:1.8;font-family:'Share Tech Mono',monospace}
.info-box .ib-text strong{color:var(--gold)}
.info-box .ib-text a{color:var(--teal);text-decoration:none}

/* MODALS */
.cert-over,.wash-over,.login-over{position:fixed;inset:0;background:rgba(0,0,0,.85);z-index:5000;display:none;align-items:center;justify-content:center;backdrop-filter:blur(4px)}
.cert-over.open,.wash-over.open,.login-over.open{display:flex}
.cert-box,.wash-box{background:rgba(2,12,2,.98);border:1px solid var(--border);border-radius:4px;width:90%;max-width:520px;overflow:hidden;box-shadow:var(--glow),0 24px 60px rgba(0,0,0,.8)}
.cert-box-img,.wash-box-img{height:215px;background:rgba(0,255,65,.03);border-bottom:1px solid var(--border);display:flex;align-items:center;justify-content:center;font-size:5rem;overflow:hidden;filter:hue-rotate(120deg)}
.cert-box-img img,.wash-box-img img{width:100%;height:100%;object-fit:cover;filter:none}
.cert-box-body,.wash-box-body{padding:1.3rem}
.cert-box-body h3,.wash-box-body h3{font-family:'Orbitron',monospace;font-size:1rem;font-weight:700;color:var(--gold);margin-bottom:.2rem;letter-spacing:.04em;text-shadow:var(--glow)}
.cbox-org{color:var(--purple);font-size:.75rem;font-weight:600;margin-bottom:.65rem;font-family:'Share Tech Mono',monospace}
.cbox-desc{color:var(--text2);font-size:.78rem;line-height:1.7;font-family:'Share Tech Mono',monospace}
.modal-close-btn{display:block;width:100%;background:transparent;color:var(--gold);border:1px solid var(--gold);padding:.5rem;border-radius:2px;font-weight:600;font-size:.72rem;cursor:pointer;font-family:'Orbitron',monospace;margin-top:.88rem;transition:all .2s;text-transform:uppercase;letter-spacing:.06em}
.modal-close-btn:hover{background:rgba(0,255,65,.1)}

/* LOGIN */
.login-box{background:rgba(2,12,2,.99);border:1px solid var(--border);border-radius:4px;padding:2.2rem;width:330px;box-shadow:var(--glow),0 22px 55px rgba(0,0,0,.8)}
.login-box h2{font-family:'Orbitron',monospace;color:var(--gold);font-size:1.1rem;font-weight:700;text-transform:uppercase;letter-spacing:.1em;margin-bottom:.2rem;text-shadow:var(--glow)}
.login-box p{color:var(--text3);font-size:.74rem;margin-bottom:1.4rem;font-family:'Share Tech Mono',monospace}
.login-box .li{width:100%;background:rgba(0,255,65,.04);border:1px solid var(--border);border-radius:2px;padding:.62rem .85rem;font-family:'Share Tech Mono',monospace;font-size:.78rem;color:var(--text);outline:none;margin-bottom:.65rem;transition:border-color .2s}
.login-box .li:focus{border-color:var(--gold);box-shadow:var(--glow)}
.login-box .lbtn{width:100%;background:transparent;color:var(--gold);padding:.65rem;border-radius:2px;font-weight:700;font-size:.78rem;cursor:pointer;border:1.5px solid var(--gold);font-family:'Orbitron',monospace;transition:all .2s;box-shadow:var(--glow);letter-spacing:.08em;text-transform:uppercase}
.login-box .lbtn:hover{background:rgba(0,255,65,.1);box-shadow:0 0 30px rgba(0,255,65,.4)}
.lerr{color:var(--pink);font-size:.7rem;margin-bottom:.48rem;display:none;font-family:'Share Tech Mono',monospace}
.remember-row{display:flex;align-items:center;gap:.5rem;margin-bottom:.85rem;font-size:.73rem;color:var(--text3);font-family:'Share Tech Mono',monospace}
.remember-row input{accent-color:var(--gold);width:14px;height:14px;cursor:pointer}

/* TOAST */
.toast{position:fixed;top:70px;left:50%;transform:translateX(-50%);background:rgba(2,12,2,.98);color:var(--gold);padding:.55rem 1.4rem;border-radius:2px;font-size:.74rem;font-weight:600;z-index:9999;display:none;border:1px solid var(--gold);box-shadow:var(--glow);white-space:nowrap;font-family:'Share Tech Mono',monospace;text-transform:uppercase;letter-spacing:.06em}

/* SCROLL ANIM */
.sa{opacity:0;transform:translateY(20px);transition:opacity .5s ease,transform .5s ease}
.sa.vis{opacity:1;transform:none}
.sa-d1{transition-delay:.1s}.sa-d2{transition-delay:.2s}.sa-d3{transition-delay:.3s}

@media(max-width:1100px){.col3{grid-template-columns:1fr 1fr}.hero-grid{grid-template-columns:1fr}.hero-right{order:-1}}
@media(max-width:768px){.nav-links{display:none}.hamburger{display:flex}.col3{grid-template-columns:1fr}.contact-grid{grid-template-columns:1fr}.adm-side{width:200px}.adm-main{left:200px}.hero-photo-area{width:260px;height:260px}.photo-circle{width:260px;height:260px}}
</style>
</head>
<body>

<!-- MATRIX RAIN CANVAS -->
<canvas id="matrixCanvas" style="position:fixed;top:0;left:0;z-index:0;opacity:.07;pointer-events:none"></canvas>
<script>
(function(){
  const c=document.getElementById('matrixCanvas');
  const ctx=c.getContext('2d');
  function resize(){c.width=window.innerWidth;c.height=window.innerHeight;}
  resize();window.addEventListener('resize',resize);
  const chars='NAIMURRASHIDTEXTILEDENIMWASHINGENZYMESTONEREACTIVEINDIGO01アイウエオカキクケコ'.split('');
  const cols=Math.floor(window.innerWidth/14);
  const drops=Array(cols).fill(1);
  function draw(){
    ctx.fillStyle='rgba(2,12,2,.05)';
    ctx.fillRect(0,0,c.width,c.height);
    ctx.fillStyle='#00ff41';
    ctx.font='13px Share Tech Mono,monospace';
    drops.forEach((y,i)=>{
      ctx.fillText(chars[Math.floor(Math.random()*chars.length)],i*14,y*14);
      if(y*14>c.height&&Math.random()>.975)drops[i]=0;
      drops[i]++;
    });
  }
  setInterval(draw,50);
})();
</script>

<!-- NAV -->
<nav>
  <div class="nav-brand">
    <div class="nav-logo"><span>MR</span></div>
    <div><div class="brand-name" id="nav-name">MD NAIMUR RASHID</div><div class="brand-sub" id="nav-sub">Textile Washing Specialist</div></div>
  </div>
  <ul class="nav-links">
    <li><a href="#home">Home</a></li>
    <li><a href="#expertise">Expertise</a></li>
    <li><a href="#rnd-sec">R&D</a></li>
    <li><a href="#port-sec">Portfolio</a></li>
    <li><a href="#certs-full">Certificates</a></li>
    <li><a href="#exp-full">Experience</a></li>
    <li><a href="#contact-sec">Contact</a></li>
  </ul>
  <div class="nav-r">
    <button class="cv-btn" onclick="genCV()">📄 Download CV</button>
    <div class="hamburger" onclick="document.getElementById('mobMenu').classList.toggle('open')"><span></span><span></span><span></span></div>
  </div>
</nav>
<div class="mob-menu" id="mobMenu">
  <a href="#home" onclick="this.closest('.mob-menu').classList.remove('open')">Home</a>
  <a href="#expertise" onclick="this.closest('.mob-menu').classList.remove('open')">Expertise</a>
  <a href="#port-sec" onclick="this.closest('.mob-menu').classList.remove('open')">Portfolio</a>
  <a href="#certs-full" onclick="this.closest('.mob-menu').classList.remove('open')">Certificates</a>
  <a href="#contact-sec" onclick="this.closest('.mob-menu').classList.remove('open')">Contact</a>
</div>

<!-- ═══ HERO ═══ -->
<section class="hero" id="home">
  <div class="hero-grid">
    <div>
      <div class="hero-eyebrow"><div class="ey-line"></div><div class="ey-text" id="hero-eyebrow-text">Textile Engineer & Washing Specialist</div></div>
      <div class="hero-name"><span class="fn" id="hero-fn">MD NAIMUR</span><span class="ln" id="hero-ln">RASHID</span></div>
      <div class="hero-title" id="hero-title">Textile Engineer &amp; Washing Specialist</div>
      <div class="washing-tags" id="hero-tags">
        <span class="wt wt-b">Denim</span><span class="wt-sep">•</span>
        <span class="wt wt-b">Knit</span><span class="wt-sep">•</span>
        <span class="wt wt-b">Woven</span><span class="wt-sep">•</span>
        <span class="wt wt-g">Washing</span>
      </div>
      <div class="pgd-badge">
        <div><div class="pgd-title" id="hero-pgd-title">PGD – Garments Business</div><div class="pgd-sub" id="hero-pgd-sub">IBA – Dhaka University</div></div>
      </div>
      <div class="hero-perks" id="hero-perks">
        <div class="perk"><span>⚙️</span> Industrial Washing Expert</div>
        <div class="perk"><span>🔬</span> Chemical Optimization &amp; R&amp;D</div>
        <div class="perk"><span>🏷️</span> <strong>H&amp;M</strong> &amp; <strong>ZARA</strong> Approved Projects</div>
      </div>
      <div class="hero-btns">
        <button class="hbtn-p" onclick="genCV()">📄 Download CV</button>
        <button class="hbtn-o" onclick="document.querySelector('#certs-full').scrollIntoView({behavior:'smooth'})">View Certificates</button>
        <button class="hbtn-g" onclick="document.querySelector('#contact-sec').scrollIntoView({behavior:'smooth'})">Contact Me</button>
      </div>
    </div>

    <!-- CIRCULAR PHOTO -->
    <div class="hero-right">
      <div class="hero-photo-area">
        <div class="photo-ring-outer"></div>
        <div class="photo-ring-dash"></div>
        <div class="photo-circle" id="photoCircle">
          <img id="heroPhotoImg" src="" alt="MD Naimur Rashid" style="display:none">
          <div class="photo-placeholder-inner" id="photoPlaceholder">
            <div class="icon">🧑‍💼</div>
            <div class="hint">Add your photo<br>via Admin Panel</div>
          </div>
        </div>
        <!-- Orbit bubbles -->
        <div class="ob ob1"><div class="ob-num" style="color:var(--blue)">3+</div><div class="ob-lbl">Years Exp.</div></div>
        <div class="ob ob2"><div style="font-size:.62rem;font-weight:800;color:var(--teal);line-height:1.1;font-family:'Orbitron',monospace">BUFT<br>Certified</div><div class="ob-lbl">R&D</div></div>
        <div class="ob ob3"><div style="font-size:.56rem;font-weight:800;color:var(--pink);line-height:1.2;font-family:'Orbitron',monospace">Denim &amp;<br>Knit</div><div class="ob-lbl">Project</div></div>
        <div class="ob ob4"><div class="ob-num" style="color:var(--purple)">25+</div><div class="ob-lbl">Processes</div></div>
      </div>
    </div>
  </div>
</section>

<!-- STATS BAR -->
<div class="stats-bar">
  <div class="stats-inner" id="statsBar">
    <div class="si"><span style="font-size:1.15rem">📅</span><div><div class="si-num">3+</div><div class="si-lbl">Years Experience</div></div></div>
    <div class="si"><span style="font-size:1.15rem">⚙️</span><div><div class="si-num">25+</div><div class="si-lbl">Washing Processes</div></div></div>
    <div class="si"><span style="font-size:1.15rem">🏢</span><div><div class="si-num">15+</div><div class="si-lbl">Buyer Projects</div></div></div>
    <div class="si"><span style="font-size:1.15rem">🎓</span><div><div class="si-num">10+</div><div class="si-lbl">Certifications</div></div></div>
    <div class="si"><span style="font-size:1.15rem">🔬</span><div><div class="si-num">1</div><div class="si-lbl">Industrial R&D</div></div></div>
  </div>
</div>

<!-- MAIN 3-COL -->
<div class="main">
  <div class="col3">
    <!-- COL1: EXPERTISE -->
    <div class="dc sa" id="expertise">
      <div class="dc-head"><div class="dc-title">— Core Expertise</div><div class="dc-line"></div></div>
      <div class="etabs" id="expTabsEl">
        <button class="etab active" onclick="switchExp('denim',this)">Denim</button>
        <button class="etab" onclick="switchExp('knit',this)">Knit</button>
        <button class="etab" onclick="switchExp('woven',this)">Woven</button>
        <button class="etab" onclick="switchExp('dyeing',this)">Dyeing</button>
      </div>
      <div class="exp-body"><ul class="exp-list" id="expList"></ul></div>
    </div>

    <!-- COL2: R&D -->
    <div class="dc sa sa-d1" id="rnd-sec">
      <div class="dc-head"><div class="dc-title" style="color:var(--gold)">— Industrial R&D</div><div class="dc-line"></div></div>
      <div class="rnd-body">
        <div class="rnd-ptitle" id="rndTitle">Natural Mordant Development</div>
        <div class="approved-b">🏷️ H&amp;M • ZARA Approved</div>
        <div class="rnd-img-box" id="rndImgBox">
          <img id="rndImg" src="" style="display:none;width:100%;height:100%;object-fit:cover">
          <span class="rnd-img-ph" id="rndImgPh">🌿</span>
        </div>
        <div class="rnd-points" id="rndPoints">
          <div class="rnd-pt"><div class="rnd-dot"></div>Betel Nut • Banana Peel • Guava Leaves</div>
          <div class="rnd-pt"><div class="rnd-dot"></div>Lab Trials • Scale-Up • Commercial Production</div>
          <div class="rnd-pt"><div class="rnd-dot"></div>Sustainable &amp; Cost Effective</div>
        </div>
        <button class="rnd-cta" onclick="document.querySelector('#cases-sec').scrollIntoView({behavior:'smooth'})">View Project →</button>
      </div>
    </div>

    <!-- COL3 -->
    <div style="display:flex;flex-direction:column;gap:1rem">
      <div class="dc sa sa-d2" id="exp-full">
        <div class="dc-head"><div class="dc-title">— Experience</div></div>
        <div class="etl" id="expTimeline"></div>
      </div>
      <div class="dc sa sa-d3">
        <div class="dc-head"><div class="dc-title">— Certifications</div></div>
        <div class="cert-sidebar" id="certSidebar"></div>
        <button class="view-all" onclick="document.querySelector('#certs-full').scrollIntoView({behavior:'smooth'})">View All Certificates</button>
      </div>
    </div>
  </div>

  <!-- PORTFOLIO -->
  <div class="port-sec sa" id="port-sec">
    <div class="sec-hdr">
      <div class="sec-title-wrap"><div class="stl"></div><div class="sec-ttl">— Washing Portfolio</div><div class="str"></div></div>
      <div class="pf-btns">
        <button class="pf-btn active" onclick="filterPort('all',this)">All</button>
        <button class="pf-btn" onclick="filterPort('denim',this)">Denim</button>
        <button class="pf-btn" onclick="filterPort('knit',this)">Knit</button>
        <button class="pf-btn" onclick="filterPort('woven',this)">Woven</button>
        <button class="pf-btn" onclick="filterPort('effects',this)">Effects</button>
      </div>
    </div>
    <div class="port-grid" id="portGrid"></div>
  </div>
</div>

<!-- CERTS FULL -->
<div style="background:rgba(0,8,0,.95);border-top:1px solid rgba(0,255,65,.1)" class="full-sec" id="certs-full">
  <div class="full-sec-inner">
    <div class="fs-hdr sa"><div class="stl"></div><div class="sec-ttl">— All Certifications</div><div class="str"></div></div>
    <div class="fs-sub sa">Click any certificate to view full details</div>
    <div class="certs-full-grid sa" id="certsGrid"></div>
  </div>
</div>

<!-- CASE STUDIES -->
<div class="full-sec" id="cases-sec">
  <div class="full-sec-inner">
    <div class="fs-hdr sa"><div class="stl"></div><div class="sec-ttl">— Washing Case Studies</div><div class="str"></div></div>
    <div class="fs-sub sa">Technical breakdown of key washing projects.</div>
    <div class="cases-grid" id="casesGrid"></div>
  </div>
</div>

<!-- SKILLS -->
<div style="background:rgba(0,8,0,.95);border-top:1px solid rgba(0,255,65,.1)" class="full-sec">
  <div class="full-sec-inner">
    <div class="fs-hdr sa"><div class="stl"></div><div class="sec-ttl">— Technical Skills</div><div class="str"></div></div>
    <div class="skills-grid sa" id="skillsGrid"></div>
  </div>
</div>

<!-- BUYERS -->
<div class="full-sec">
  <div class="full-sec-inner">
    <div class="fs-hdr sa"><div class="stl"></div><div class="sec-ttl">— Buyer Projects</div><div class="str"></div></div>
    <div class="buyers-grid sa" id="buyersGrid"></div>
  </div>
</div>

<!-- CONTACT -->
<div style="background:rgba(0,8,0,.95);border-top:1px solid rgba(0,255,65,.1)" class="full-sec" id="contact-sec">
  <div class="full-sec-inner">
    <div class="fs-hdr sa"><div class="stl"></div><div class="sec-ttl">— Get In Touch</div><div class="str"></div></div>
    <div class="contact-grid">
      <div class="sa" id="contactInfoEl"></div>
      <div class="dc sa sa-d1" style="padding:1.3rem;background:rgba(0,20,0,.9);border:1px solid rgba(0,255,65,.2)">
        <div style="font-family:'Orbitron',monospace;font-weight:700;font-size:.82rem;text-transform:uppercase;letter-spacing:.08em;color:var(--gold);margin-bottom:1rem;text-shadow:var(--glow)">Send a Message</div>
        <label class="cf-lbl">Full Name</label><input class="cf-inp" id="cfName" placeholder="Your full name">
        <label class="cf-lbl">Email</label><input class="cf-inp" id="cfEmail" placeholder="your@email.com">
        <label class="cf-lbl">Message</label><textarea class="cf-inp" id="cfMsg" rows="4" placeholder="Describe your project..." style="resize:vertical"></textarea>
        <button class="cf-sub" onclick="cfSubmit()">Let's Work Together →</button>
      </div>
    </div>
  </div>
</div>

<!-- FOOTER -->
<div class="footer-bar">
  <div class="footer-contacts" id="footerContacts"></div>
  <button class="footer-cta" onclick="document.querySelector('#contact-sec').scrollIntoView({behavior:'smooth'})">Let's Work Together</button>
  <div class="soc-btns">
    <div class="soc-b" id="socLI">in</div>
    <div class="soc-b" id="socYT">▶</div>
    <div class="soc-b" id="socAdm" onclick="showLogin()" title="Admin">⚙</div>
  </div>
</div>

<!-- AI CHAT -->
<div class="chat-wrap">
  <div class="chat-win" id="chatWin">
    <div class="chat-hdr">
      <div style="display:flex;align-items:center;gap:.58rem">
        <div class="chat-av">MR</div>
        <div><div class="chat-hdr-name">NR Assistant</div><div class="chat-hdr-st">● Online</div></div>
      </div>
      <button class="chat-close" onclick="document.getElementById('chatWin').classList.toggle('open')">✕</button>
    </div>
    <div class="chat-chips">
      <button class="chip" onclick="cs('experience')">Experience</button>
      <button class="chip" onclick="cs('denim washing techniques')">Denim Washing</button>
      <button class="chip" onclick="cs('R&D projects')">R&D</button>
      <button class="chip" onclick="cs('contact info')">Contact</button>
    </div>
    <div class="chat-msgs" id="chatMsgs">
      <div class="cm bot"><div class="cm-b">👋 Hi! I'm Naimur's AI assistant. Ask me about his experience, denim washing, R&D projects or certifications!</div></div>
    </div>
    <div class="chat-inp-row">
      <input class="chat-inp" id="chatInp" placeholder="Ask anything..." onkeydown="if(event.key==='Enter')chatSend()">
      <button class="chat-send" onclick="chatSend()">➤</button>
    </div>
  </div>
  <button class="chat-toggle" onclick="document.getElementById('chatWin').classList.toggle('open')">MR</button>
</div>

<!-- CERT MODAL -->
<div class="cert-over" id="certOver" onclick="if(event.target===this)this.classList.remove('open')">
  <div class="cert-box">
    <div class="cert-box-img" id="cmImg"></div>
    <div class="cert-box-body"><h3 id="cmName"></h3><div class="cbox-org" id="cmOrg"></div><div class="cbox-desc" id="cmDesc"></div><button class="modal-close-btn" onclick="document.getElementById('certOver').classList.remove('open')">Close ✕</button></div>
  </div>
</div>

<!-- WASH MODAL -->
<div class="wash-over" id="washOver" onclick="if(event.target===this)this.classList.remove('open')">
  <div class="wash-box">
    <div class="wash-box-img" id="wmImg"></div>
    <div class="wash-box-body"><div style="font-size:.6rem;letter-spacing:.1em;text-transform:uppercase;color:var(--gold);font-weight:700;margin-bottom:.24rem" id="wmCat"></div><h3 id="wmName" style="margin-bottom:.45rem"></h3><div style="font-size:.8rem;color:var(--text2);line-height:1.7" id="wmDesc"></div><button class="modal-close-btn" onclick="document.getElementById('washOver').classList.remove('open')">Close ✕</button></div>
  </div>
</div>

<!-- LOGIN -->
<div class="login-over" id="loginOver" onclick="if(event.target===this)this.classList.remove('open')">
  <div class="login-box">
    <h2>Admin Login</h2>
    <p>Enter your credentials to manage portfolio</p>
    <input class="li" type="text" id="aUser" placeholder="Username">
    <input class="li" type="password" id="aPass" placeholder="Password">
    <div class="remember-row"><input type="checkbox" id="rememberMe"> <label for="rememberMe">Keep me logged in on this device</label></div>
    <div class="lerr" id="lErr">❌ Invalid username or password.</div>
    <button class="lbtn" onclick="doLogin()">Login to Dashboard</button>
  </div>
</div>

<!-- ═══════════════════════ ADMIN DASHBOARD ═══════════════════════ -->
<div id="adm-wrap">
  <div class="adm-side">
    <div class="adm-logo"><div class="t">NR Admin Panel</div><small>Full Portfolio Manager</small></div>
    <div class="adm-section-label">General</div>
    <div class="adm-nav active" onclick="admNav('dash',this)">📊 Dashboard</div>
    <div class="adm-nav" onclick="admNav('photo',this)">🖼️ Hero Photo</div>
    <div class="adm-nav" onclick="admNav('hero',this)">✏️ Hero Content</div>
    <div class="adm-nav" onclick="admNav('stats',this)">📈 Stats Bar</div>
    <div class="adm-section-label">Sections</div>
    <div class="adm-nav" onclick="admNav('expertise',this)">⚡ Expertise Tabs</div>
    <div class="adm-nav" onclick="admNav('rnd',this)">🔬 R&D Project</div>
    <div class="adm-nav" onclick="admNav('exp',this)">💼 Experience</div>
    <div class="adm-nav" onclick="admNav('edu',this)">🎓 Education</div>
    <div class="adm-section-label">Content</div>
    <div class="adm-nav" onclick="admNav('certs',this)">📜 Certificates</div>
    <div class="adm-nav" onclick="admNav('port',this)">👔 Washing Portfolio</div>
    <div class="adm-nav" onclick="admNav('cases',this)">📋 Case Studies</div>
    <div class="adm-nav" onclick="admNav('skills',this)">🛠️ Skills</div>
    <div class="adm-nav" onclick="admNav('buyers',this)">🏢 Buyer Projects</div>
    <div class="adm-section-label">Profile</div>
    <div class="adm-nav" onclick="admNav('contact',this)">📞 Contact Info</div>
    <div class="adm-nav" onclick="admNav('social',this)">🔗 Social Links</div>
  </div>

  <div class="adm-main">
    <div class="adm-topbar"><h1 id="admTitle">Dashboard</h1><div style="display:flex;gap:.5rem;align-items:center"><button onclick="localStorage.removeItem('nr_admin_session');closeAdm();" style="background:rgba(224,69,138,.1);color:#e0458a;border:1.5px solid rgba(224,69,138,.25);padding:.36rem .88rem;border-radius:6px;cursor:pointer;font-size:.72rem;font-family:Barlow,sans-serif">🔓 Logout</button><button class="adm-close" onclick="closeAdm()">✕ Close</button></div></div>

    <!-- DASHBOARD -->
    <div class="adm-panel active" id="ap-dash">
      <div class="adm-stats" id="admStats"></div>
      <div class="afc">
        <h3>🚀 Quick Actions</h3>
        <div style="display:flex;gap:.55rem;flex-wrap:wrap;margin-bottom:1rem">
          <button class="btn-add" onclick="admNav('photo',document.querySelectorAll('.adm-nav')[1])">🖼️ Update Photo</button>
          <button class="btn-add" onclick="admNav('hero',document.querySelectorAll('.adm-nav')[2])">✏️ Edit Hero</button>
          <button class="btn-add" onclick="admNav('certs',document.querySelectorAll('.adm-nav')[10])">+ Add Certificate</button>
          <button class="btn-add" onclick="admNav('port',document.querySelectorAll('.adm-nav')[11])">+ Add Portfolio</button>
          <button class="abtn-gold" onclick="genCV()">📄 Generate CV</button>
        </div>
        <div class="info-box">
          <div class="ib-title">💡 How to add images to any section:</div>
          <div class="ib-text">
            <strong>Step 1:</strong> Go to <a href="https://imgbb.com" target="_blank">imgbb.com</a> → Upload your image (free, no account needed)<br>
            <strong>Step 2:</strong> After upload → click <em>"Embed codes"</em> → copy the <strong>Direct link</strong> (ends in .jpg/.png)<br>
            <strong>Step 3:</strong> Paste the URL in the image field in any section below → live preview appears<br>
            <strong>Step 4:</strong> Click Save → the image appears on the website instantly ✅
          </div>
        </div>
      </div>
    </div>

    <!-- HERO PHOTO -->
    <div class="adm-panel" id="ap-photo">
      <div class="afc">
        <h3>🖼️ Hero Profile Photo</h3>
        <div class="info-box">
          <div class="ib-title">📌 Upload your photo:</div>
          <div class="ib-text">
            <strong>1.</strong> Go to <a href="https://imgbb.com" target="_blank">imgbb.com</a> → upload your professional photo<br>
            <strong>2.</strong> After upload → <em>Embed codes</em> → copy <strong>Direct link</strong><br>
            <strong>3.</strong> Paste below → preview appears → click Apply
          </div>
        </div>
        <label class="al">Your Photo Direct URL</label>
        <div class="img-field-wrap">
          <input class="ai img-url-inp" id="heroPhotoUrl" placeholder="https://i.ibb.co/xxxxxxx/your-photo.jpg" oninput="prevHeroPhoto(this.value)">
        </div>
        <div class="img-prev-row" style="margin-top:.75rem">
          <div class="img-prev-box" id="heroPhotoPrev" style="width:90px;height:110px;border-radius:50%;border:3px solid var(--blue)"><span>🧑‍💼</span></div>
          <div class="img-hint-text">Live preview of your photo in the circular frame.<br>Recommended: Portrait photo, min 400×500px<br>Best format: JPG/PNG · Best sites: <a href="https://imgbb.com" target="_blank">imgbb.com</a> · <a href="https://imgur.com" target="_blank">imgur.com</a></div>
        </div>
        <div style="margin-top:1.15rem;display:flex;gap:.45rem;flex-wrap:wrap">
          <button class="abtn-save" onclick="applyHeroPhoto()">✅ Apply Photo to Website</button>
          <button class="abtn-cancel" onclick="removeHeroPhoto()">🗑️ Remove Photo</button>
          <button style="background:rgba(240,165,0,.12);color:var(--gold);border:1px solid var(--borderg);padding:.54rem .9rem;border-radius:7px;font-size:.76rem;cursor:pointer;font-family:'Barlow',sans-serif" onclick="testSamplePhoto()">🧪 Test with Sample</button>
        </div>
      </div>
    </div>

    <!-- HERO CONTENT -->
    <div class="adm-panel" id="ap-hero">
      <div class="afc">
        <h3>✏️ Edit Hero Section</h3>
        <div class="aform-grid">
          <div><label class="al">First Name</label><input class="ai" id="hFn" placeholder="MD NAIMUR"></div>
          <div><label class="al">Last Name</label><input class="ai" id="hLn" placeholder="RASHID"></div>
          <div class="aform-full"><label class="al">Job Title</label><input class="ai" id="hTitle" placeholder="Textile Engineer & Washing Specialist"></div>
          <div class="aform-full"><label class="al">Eyebrow Text (small text above name)</label><input class="ai" id="hEyebrow" placeholder="Textile Engineer & Washing Specialist"></div>
          <div><label class="al">Badge Title (e.g. PGD)</label><input class="ai" id="hPgdTitle" placeholder="PGD – Garments Business"></div>
          <div><label class="al">Badge Subtitle</label><input class="ai" id="hPgdSub" placeholder="IBA – Dhaka University"></div>
          <div class="aform-full"><label class="al">Perk 1</label><input class="ai" id="hP1" placeholder="Industrial Washing Expert"></div>
          <div class="aform-full"><label class="al">Perk 2</label><input class="ai" id="hP2" placeholder="Chemical Optimization & R&D"></div>
          <div class="aform-full"><label class="al">Perk 3</label><input class="ai" id="hP3" placeholder="H&M & ZARA Approved Projects"></div>
        </div>
        <div style="margin-top:1rem"><button class="abtn-save" onclick="saveHero()">💾 Save Hero Content</button></div>
      </div>
    </div>

    <!-- STATS BAR -->
    <div class="adm-panel" id="ap-stats">
      <div class="afc">
        <h3>📈 Edit Stats Bar</h3>
        <div id="statsFormEl"></div>
        <button class="abtn-save" onclick="saveStats()">💾 Save Stats</button>
      </div>
    </div>

    <!-- EXPERTISE -->
    <div class="adm-panel" id="ap-expertise">
      <div class="afc">
        <h3>⚡ Edit Expertise Tabs</h3>
        <p style="font-size:.76rem;color:var(--text3);margin-bottom:1rem">Edit the skills shown under each tab. Each line = one skill (use • as separator).</p>
        <div id="expertiseFormEl"></div>
        <button class="abtn-save" onclick="saveExpertise()">💾 Save Expertise</button>
      </div>
    </div>

    <!-- R&D -->
    <div class="adm-panel" id="ap-rnd">
      <div class="afc">
        <h3>🔬 Edit R&D Project</h3>
        <div class="aform-grid">
          <div class="aform-full"><label class="al">Project Title</label><input class="ai" id="rndTitleInp" placeholder="Natural Mordant Development"></div>
          <div class="aform-full"><label class="al">Approval Badge Text</label><input class="ai" id="rndBadge" placeholder="H&M • ZARA Approved"></div>
          <div class="aform-full"><label class="al">Point 1</label><input class="ai" id="rndP1" placeholder="Betel Nut • Banana Peel • Guava Leaves"></div>
          <div class="aform-full"><label class="al">Point 2</label><input class="ai" id="rndP2" placeholder="Lab Trials • Scale-Up • Commercial Production"></div>
          <div class="aform-full"><label class="al">Point 3</label><input class="ai" id="rndP3" placeholder="Sustainable & Cost Effective"></div>
          <div class="aform-full">
            <label class="al">R&D Image URL</label>
            <div class="img-field-wrap"><input class="ai img-url-inp" id="rndImgUrl" placeholder="https://i.ibb.co/xxxxx/rnd-image.jpg" oninput="prevRndImg(this.value)"></div>
            <div class="img-prev-row">
              <div class="img-prev-box" id="rndImgPrevBox"><span>🌿</span></div>
              <div class="img-hint-text">Upload R&D project photo to <a href="https://imgbb.com" target="_blank">imgbb.com</a> → paste direct link here</div>
            </div>
          </div>
        </div>
        <div style="margin-top:1rem"><button class="abtn-save" onclick="saveRnd()">💾 Save R&D Content</button></div>
      </div>
    </div>

    <!-- EXPERIENCE -->
    <div class="adm-panel" id="ap-exp">
      <button class="btn-add" onclick="showExpForm()">+ Add Experience</button>
      <div id="expFormWrap" style="display:none">
        <div class="afc">
          <h3>💼 <span id="expFormTitle">Add Experience</span></h3>
          <div class="aform-grid">
            <div><label class="al">Job Title *</label><input class="ai" id="fExpRole" placeholder="Executive – Washing"></div>
            <div><label class="al">Company *</label><input class="ai" id="fExpCo" placeholder="Fakir Apparels Ltd."></div>
            <div><label class="al">Period</label><input class="ai" id="fExpDate" placeholder="2025 – Present"></div>
            <div><label class="al">Buyer Tag (optional)</label><input class="ai" id="fExpBuyer" placeholder="GAP Buyer Responsible"></div>
            <div class="aform-full"><label class="al">Location</label><input class="ai" id="fExpLoc" placeholder="Narayanganj, Bangladesh"></div>
            <div class="aform-full"><label class="al">Responsibilities (one per line)</label><textarea class="ai" id="fExpDuties" placeholder="Managing washing production&#10;Monitoring quality standards"></textarea></div>
          </div>
          <div style="margin-top:1rem;display:flex;gap:.45rem">
            <button class="abtn-save" onclick="saveExp()">💾 Save</button>
            <button class="abtn-cancel" onclick="document.getElementById('expFormWrap').style.display='none'">Cancel</button>
          </div>
        </div>
      </div>
      <div class="atbl-wrap"><table class="atbl"><thead><tr><th>Role</th><th>Company</th><th>Period</th><th>Actions</th></tr></thead><tbody id="expTbody"></tbody></table></div>
    </div>

    <!-- EDUCATION -->
    <div class="adm-panel" id="ap-edu">
      <button class="btn-add" onclick="showEduForm()">+ Add Education</button>
      <div id="eduFormWrap" style="display:none">
        <div class="afc">
          <h3>🎓 Add Education</h3>
          <div class="aform-grid">
            <div><label class="al">Degree *</label><input class="ai" id="fEduDeg" placeholder="BSc in Textile Engineering"></div>
            <div><label class="al">Institution *</label><input class="ai" id="fEduInst" placeholder="BUFT"></div>
            <div><label class="al">Year</label><input class="ai" id="fEduYear" placeholder="2023"></div>
            <div><label class="al">CGPA / Result</label><input class="ai" id="fEduGpa" placeholder="3.6 / 4.0"></div>
            <div class="aform-full"><label class="al">Status / Notes</label><input class="ai" id="fEduNote" placeholder="Completed · Wet Processing Specialization"></div>
          </div>
          <div style="margin-top:1rem;display:flex;gap:.45rem">
            <button class="abtn-save" onclick="saveEdu()">💾 Save</button>
            <button class="abtn-cancel" onclick="document.getElementById('eduFormWrap').style.display='none'">Cancel</button>
          </div>
        </div>
      </div>
      <div class="atbl-wrap"><table class="atbl"><thead><tr><th>Degree</th><th>Institution</th><th>Year</th><th>CGPA</th><th>Actions</th></tr></thead><tbody id="eduTbody"></tbody></table></div>
    </div>

    <!-- CERTIFICATES -->
    <div class="adm-panel" id="ap-certs">
      <button class="btn-add" onclick="showCertForm()">+ Add Certificate</button>
      <div id="certFormWrap" style="display:none">
        <div class="afc">
          <h3>📜 <span id="certFormTitle">Add Certificate</span></h3>
          <div class="aform-grid">
            <div><label class="al">Certificate Name *</label><input class="ai" id="fCertName" placeholder="Sustainable Dyeing..."></div>
            <div><label class="al">Organization *</label><input class="ai" id="fCertOrg" placeholder="SDC / Cambridge..."></div>
            <div class="aform-full"><label class="al">Description</label><input class="ai" id="fCertDesc" placeholder="Brief description of this certification"></div>
            <div><label class="al">Icon Emoji</label><input class="ai" id="fCertIcon" placeholder="🎨" maxlength="4"></div>
            <div class="aform-full">
              <label class="al">Certificate Image URL (scan / photo from ImgBB)</label>
              <div class="img-field-wrap"><input class="ai img-url-inp" id="fCertImg" placeholder="https://i.ibb.co/xxxxx/certificate.jpg" oninput="prevCertImg(this.value)"></div>
              <div class="img-prev-row">
                <div class="img-prev-box" id="fCertImgPrev"><span id="fCertImgPh">📋</span></div>
                <div class="img-hint-text">Upload certificate scan to <a href="https://imgbb.com" target="_blank">imgbb.com</a> → paste link above<br>Preview updates as you type</div>
              </div>
            </div>
          </div>
          <div style="margin-top:1rem;display:flex;gap:.45rem">
            <button class="abtn-save" onclick="saveCert()">💾 Save Certificate</button>
            <button class="abtn-cancel" onclick="document.getElementById('certFormWrap').style.display='none'">Cancel</button>
          </div>
        </div>
      </div>
      <div class="atbl-wrap"><table class="atbl"><thead><tr><th>Image</th><th>Name</th><th>Organization</th><th>Actions</th></tr></thead><tbody id="certTbody"></tbody></table></div>
    </div>

    <!-- PORTFOLIO -->
    <div class="adm-panel" id="ap-port">
      <button class="btn-add" onclick="showPortForm()">+ Add Portfolio Item</button>
      <div id="portFormWrap" style="display:none">
        <div class="afc">
          <h3>👔 <span id="portFormTitle">Add Portfolio Item</span></h3>
          <div class="aform-grid">
            <div><label class="al">Title *</label><input class="ai" id="fPortName" placeholder="Vintage Denim Effect"></div>
            <div><label class="al">Category *</label><select class="ai" id="fPortCat"><option value="denim">Denim</option><option value="knit">Knit</option><option value="woven">Woven</option><option value="effects">Effects</option></select></div>
            <div><label class="al">Washing Technique</label><input class="ai" id="fPortTech" placeholder="Enzyme + PP Spray"></div>
            <div><label class="al">Icon Emoji (if no image)</label><input class="ai" id="fPortEmoji" placeholder="👖" maxlength="4"></div>
            <div class="aform-full"><label class="al">Description</label><textarea class="ai" id="fPortDesc" placeholder="Technical description of this washing process"></textarea></div>
            <div class="aform-full">
              <label class="al">Garment / Washing Result Image URL</label>
              <div class="img-field-wrap"><input class="ai img-url-inp" id="fPortImg" placeholder="https://i.ibb.co/xxxxx/garment.jpg" oninput="prevPortImg(this.value)"></div>
              <div class="img-prev-row">
                <div class="img-prev-box" id="fPortImgPrev"><span id="fPortImgPh">👔</span></div>
                <div class="img-hint-text">Upload garment photo to <a href="https://imgbb.com" target="_blank">imgbb.com</a> → paste link above<br>This image shows in the portfolio gallery</div>
              </div>
            </div>
          </div>
          <div style="margin-top:1rem;display:flex;gap:.45rem">
            <button class="abtn-save" onclick="savePort()">💾 Save Item</button>
            <button class="abtn-cancel" onclick="document.getElementById('portFormWrap').style.display='none'">Cancel</button>
          </div>
        </div>
      </div>
      <div class="atbl-wrap"><table class="atbl"><thead><tr><th>Image</th><th>Title</th><th>Category</th><th>Technique</th><th>Actions</th></tr></thead><tbody id="portTbody"></tbody></table></div>
    </div>

    <!-- CASE STUDIES -->
    <div class="adm-panel" id="ap-cases">
      <button class="btn-add" onclick="showCaseForm()">+ Add Case Study</button>
      <div id="caseFormWrap" style="display:none">
        <div class="afc">
          <h3>📋 <span id="caseFormTitle">Add Case Study</span></h3>
          <div class="aform-grid">
            <div><label class="al">Buyer / Label</label><input class="ai" id="fCaseBuyer" placeholder="GAP / Internal / R&D"></div>
            <div><label class="al">Project Title *</label><input class="ai" id="fCaseTitle" placeholder="Vintage Denim Development"></div>
            <div><label class="al">Technique</label><input class="ai" id="fCaseTech" placeholder="Enzyme + PP Spray"></div>
            <div><label class="al">Machine</label><input class="ai" id="fCaseMachine" placeholder="Industrial Front-Load (200kg)"></div>
            <div><label class="al">Chemicals</label><input class="ai" id="fCaseChem" placeholder="Cellulase, KMnO₄, Silicone"></div>
            <div><label class="al">Challenge</label><input class="ai" id="fCaseChall" placeholder="Consistent shade across batches"></div>
            <div class="aform-full"><label class="al">Final Result ✅</label><input class="ai" id="fCaseResult" placeholder="Vintage denim achieved with <3% shade variation"></div>
          </div>
          <div style="margin-top:1rem;display:flex;gap:.45rem">
            <button class="abtn-save" onclick="saveCaseStudy()">💾 Save</button>
            <button class="abtn-cancel" onclick="document.getElementById('caseFormWrap').style.display='none'">Cancel</button>
          </div>
        </div>
      </div>
      <div class="atbl-wrap"><table class="atbl"><thead><tr><th>Buyer</th><th>Title</th><th>Technique</th><th>Result</th><th>Actions</th></tr></thead><tbody id="caseTbody"></tbody></table></div>
    </div>

    <!-- SKILLS -->
    <div class="adm-panel" id="ap-skills">
      <button class="btn-add" onclick="showSkillForm()">+ Add Skill</button>
      <div id="skillFormWrap" style="display:none">
        <div class="afc">
          <h3>🛠️ Add Skill</h3>
          <div class="aform-grid">
            <div><label class="al">Skill Name *</label><input class="ai" id="fSkName" placeholder="Enzyme Wash"></div>
            <div><label class="al">Icon Emoji</label><input class="ai" id="fSkIcon" placeholder="🫧" maxlength="4"></div>
            <div><label class="al">Proficiency % (0–100)</label><input class="ai" id="fSkLevel" type="number" min="0" max="100" placeholder="92"></div>
          </div>
          <div style="margin-top:1rem;display:flex;gap:.45rem">
            <button class="abtn-save" onclick="saveSkill()">💾 Save</button>
            <button class="abtn-cancel" onclick="document.getElementById('skillFormWrap').style.display='none'">Cancel</button>
          </div>
        </div>
      </div>
      <div class="atbl-wrap"><table class="atbl"><thead><tr><th>Icon</th><th>Skill</th><th>Level</th><th>Actions</th></tr></thead><tbody id="skillTbody"></tbody></table></div>
    </div>

    <!-- BUYERS -->
    <div class="adm-panel" id="ap-buyers">
      <button class="btn-add" onclick="showBuyerForm()">+ Add Buyer Project</button>
      <div id="buyerFormWrap" style="display:none">
        <div class="afc">
          <h3>🏢 <span id="buyerFormTitle">Add Buyer Project</span></h3>
          <div class="aform-grid">
            <div><label class="al">Buyer Name *</label><input class="ai" id="fBuyerName" placeholder="GAP Denim Washing"></div>
            <div><label class="al">Project / Period</label><input class="ai" id="fBuyerProj" placeholder="Blue Creations Ltd. (2022–2025)"></div>
            <div class="aform-full"><label class="al">Description</label><textarea class="ai" id="fBuyerSpec" placeholder="Details about the buyer project..."></textarea></div>
            <div><label class="al">Quality Badge Text</label><input class="ai" id="fBuyerBadge" placeholder="GAP RSL Compliant"></div>
            <div><label class="al">Logo Icon Emoji</label><input class="ai" id="fBuyerIcon" placeholder="🏷️" maxlength="4"></div>
            <div class="aform-full">
              <label class="al">Buyer Logo Image URL (optional)</label>
              <div class="img-field-wrap"><input class="ai img-url-inp" id="fBuyerImg" placeholder="https://i.ibb.co/xxxxx/logo.jpg" oninput="prevBuyerImg(this.value)"></div>
              <div class="img-prev-row">
                <div class="img-prev-box" id="fBuyerImgPrev"><span id="fBuyerImgPh">🏷️</span></div>
                <div class="img-hint-text">Upload buyer logo to <a href="https://imgbb.com" target="_blank">imgbb.com</a></div>
              </div>
            </div>
          </div>
          <div style="margin-top:1rem;display:flex;gap:.45rem">
            <button class="abtn-save" onclick="saveBuyer()">💾 Save</button>
            <button class="abtn-cancel" onclick="document.getElementById('buyerFormWrap').style.display='none'">Cancel</button>
          </div>
        </div>
      </div>
      <div class="atbl-wrap"><table class="atbl"><thead><tr><th>Logo</th><th>Buyer</th><th>Project</th><th>Actions</th></tr></thead><tbody id="buyerTbody"></tbody></table></div>
    </div>

    <!-- CONTACT INFO -->
    <div class="adm-panel" id="ap-contact">
      <div class="afc">
        <h3>📞 Edit Contact Information</h3>
        <div class="aform-grid">
          <div><label class="al">Full Name</label><input class="ai" id="cName" placeholder="MD Naimur Rashid"></div>
          <div><label class="al">Job Title</label><input class="ai" id="cJobTitle" placeholder="Executive – Washing"></div>
          <div><label class="al">Email</label><input class="ai" id="cEmail" placeholder="mdnaimurrashid752@gmail.com"></div>
          <div><label class="al">Phone / WhatsApp</label><input class="ai" id="cPhone" placeholder="+8801626282048"></div>
          <div><label class="al">Location</label><input class="ai" id="cLoc" placeholder="Dhaka, Bangladesh"></div>
          <div><label class="al">Company</label><input class="ai" id="cCompany" placeholder="Fakir Apparels Ltd., Narayanganj"></div>
        </div>
        <div style="margin-top:1rem"><button class="abtn-save" onclick="saveContact()">💾 Save Contact Info</button></div>
      </div>
    </div>

    <!-- SOCIAL LINKS -->
    <div class="adm-panel" id="ap-social">
      <div class="afc">
        <h3>🔗 Social & Links</h3>
        <div class="aform-grid">
          <div><label class="al">LinkedIn URL</label><input class="ai" id="sLI" placeholder="https://linkedin.com/in/..."></div>
          <div><label class="al">YouTube URL</label><input class="ai" id="sYT" placeholder="https://youtube.com/@..."></div>
        </div>
        <div style="margin-top:1rem"><button class="abtn-save" onclick="saveSocial()">💾 Save Links</button></div>
      </div>
    </div>

  </div><!-- end adm-main -->
</div><!-- end adm-wrap -->

<div class="toast" id="toast"></div>

<!-- ═══════════════════════ JAVASCRIPT ═══════════════════════ -->
<script>
// ══ DATA STORE ══
const DB = {
  heroPhoto:'',
  hero:{fn:'MD NAIMUR',ln:'RASHID',title:'Textile Engineer & Washing Specialist',eyebrow:'Textile Engineer & Washing Specialist',pgdTitle:'PGD – Garments Business',pgdSub:'IBA – Dhaka University',p1:'Industrial Washing Expert',p2:'Chemical Optimization & R&D',p3:'H&M & ZARA Approved Projects'},
  stats:[{icon:'📅',num:'3+',lbl:'Years Experience'},{icon:'⚙️',num:'25+',lbl:'Washing Processes'},{icon:'🏢',num:'15+',lbl:'Buyer Projects'},{icon:'🎓',num:'10+',lbl:'Certifications'},{icon:'🔬',num:'1',lbl:'Industrial R&D'}],
  expertise:{
    denim:[{i:'🫧',t:'<strong>Enzyme</strong> • Stone • Acid Wash'},{i:'🎨',t:'Vintage & <strong>PP Spray</strong>'},{i:'💧',t:'Softener & <strong>Indigo</strong> Wash'},{i:'⚡',t:'CPD Effects & <strong>Distressing</strong>'},{i:'🪨',t:'Heavy Stone & <strong>Bleach</strong>'}],
    knit:[{i:'🧶',t:'Knit <strong>Enzyme</strong> Wash'},{i:'🎨',t:'<strong>Pigment</strong> & Reactive Dyeing'},{i:'🌈',t:'Tie-Dye & <strong>Dip-Dye</strong>'},{i:'🧴',t:'Silicone <strong>Softener</strong> Finish'},{i:'✨',t:'Burnout & <strong>Devore</strong>'}],
    woven:[{i:'🏗️',t:'Woven <strong>Garment</strong> Washing'},{i:'🎭',t:'Finishing & <strong>Fabric</strong> Development'},{i:'⚗️',t:'Chemical <strong>Optimization</strong>'},{i:'📋',t:'Production <strong>Planning</strong>'},{i:'🔍',t:'Quality <strong>Rejection</strong> Control'}],
    dyeing:[{i:'🎨',t:'<strong>Pigment</strong> Dyeing & Chalk'},{i:'⚗️',t:'<strong>Reactive</strong> Dyeing'},{i:'🌿',t:'<strong>Natural Mordant</strong> (H&M/ZARA)'},{i:'🌊',t:'<strong>Direct</strong> Dyeing'},{i:'🔥',t:'<strong>Burnout</strong> Dyeing'}],
  },
  rnd:{title:'Natural Mordant Development',badge:'H&M • ZARA Approved',img:'',p1:'Betel Nut • Banana Peel • Guava Leaves',p2:'Lab Trials • Scale-Up • Commercial Production',p3:'Sustainable & Cost Effective'},
  experience:[
    {id:1,role:'Executive – Washing',co:'Fakir Apparels Ltd.',date:'2025 – Present',buyer:'',loc:'Narayanganj, Bangladesh',duties:'Managing washing production\nMonitoring quality standards\nMachine troubleshooting',cur:true},
    {id:2,role:'Denim Washing Executive',co:'Blue Creations Ltd.',date:'2022 – 2025',buyer:'GAP Buyer Responsible',loc:'Bangladesh',duties:'Managing denim washing for GAP\nLeading shift teams\nRejection control & planning',cur:false},
  ],
  education:[
    {id:1,deg:'Executive MBA (EMBA)',inst:'IBA, University of Dhaka',year:'2026',gpa:'',note:'Enrolled'},
    {id:2,deg:'BSc in Textile Engineering',inst:'BUFT',year:'2023',gpa:'3.6/4.0',note:'Wet Processing Specialization'},
  ],
  certs:[
    {id:1,name:'Sustainable Dyeing of Cellulosic Fibres',org:'Society of Dyers & Colourists',img:'',icon:'🎨',desc:'Eco-friendly reactive dyeing processes for cellulosic fibers, reducing water and chemical usage.'},
    {id:2,name:'Textile Care Labelling',org:'Society of Dyers & Colourists',img:'',icon:'🏷️',desc:'International care labelling standards, ISO symbols, and garment export regulatory compliance.'},
    {id:3,name:'Colour Management for Print Designers',org:'Society of Dyers & Colourists',img:'',icon:'🌈',desc:'Advanced colour theory, ICC profiles, and print-to-fabric colour consistency for fashion.'},
    {id:4,name:'Principles of Printed Textiles',org:'Society of Dyers & Colourists',img:'',icon:'🖨️',desc:'Core textile printing processes: screen, digital, and rotary printing for fashion and industry.'},
    {id:5,name:'Critical Thinking Certification',org:'Cambridge University',img:'',icon:'🏛️',desc:'Analytical reasoning and critical thinking for professional problem-solving environments.'},
  ],
  portfolio:[
    {id:1,name:'Vintage Denim',cat:'denim',tech:'Enzyme + PP Spray',img:'',icon:'👖',desc:'Enzyme wash combined with PP spray for authentic vintage denim per GAP specifications.'},
    {id:2,name:'Acid Wash',cat:'denim',tech:'KMnO₄ Method',img:'',icon:'⚡',desc:'KMnO₄ soaked pumice stone creating high-contrast bleach patterns with antique feel.'},
    {id:3,name:'Indigo Knit',cat:'knit',tech:'Indigo Wash',img:'',icon:'🧶',desc:'Indigo dye application on knit fabric with controlled ring-dyeing effect.'},
    {id:4,name:'Stone Wash',cat:'denim',tech:'Pumice Stone',img:'',icon:'🪨',desc:'Heavy abrasion stone wash creating worn, rugged appearance with natural fading.'},
    {id:5,name:'Stone + Enzyme',cat:'denim',tech:'Enzyme + Stone',img:'',icon:'🫧',desc:'Combined enzyme and stone wash for soft hand-feel with premium distressing.'},
    {id:6,name:'PP Spray Effect',cat:'effects',tech:'KMnO₄ Spray',img:'',icon:'🎨',desc:'Controlled PP spray creating realistic whisker and fading patterns.'},
    {id:7,name:'Bulk Production',cat:'woven',tech:'Multi-Process',img:'',icon:'🏭',desc:'Full-scale bulk washing production for international export buyers.'},
    {id:8,name:'CPD Effect',cat:'effects',tech:'Chemical Effect',img:'',icon:'✨',desc:'Chemical dimensional effect treatment for premium appearance and texture.'},
  ],
  cases:[
    {id:1,buyer:'GAP',title:'Vintage Denim Effect Development',tech:'Enzyme + PP Spray + Softener',machine:'Industrial Front-Load (200kg)',chem:'Cellulase, KMnO₄, Silicone',chall:'Consistent shade across batches',result:'Vintage denim with <3% shade variation, GAP compliant.'},
    {id:2,buyer:'H&M/ZARA',title:'Natural Mordant Development',tech:'Natural Mordant',machine:'Lab equipment + Bulk machine',chem:'Betel Nut, Banana Peel, Guava Leaves',chall:'Commercial scale consistency',result:'60% reduction in synthetic chemicals. H&M & ZARA approved.'},
    {id:3,buyer:'Internal',title:'Rejection Rate Reduction',tech:'Process Optimization',machine:'All washing machines',chem:'Standardized dosing',chall:'Shade inconsistency & surface defects',result:'40% reduction in rejection rate.'},
    {id:4,buyer:'GAP',title:'Eco Enzyme Wash – ZDHC',tech:'Bio-Enzyme Eco-Wash',machine:'Industrial Washer',chem:'Neutral Cellulase + Eco-Softener',chall:'RSL and ZDHC compliance',result:'25% water saving, full RSL compliance.'},
  ],
  skills:[
    {id:1,name:'Enzyme Wash',icon:'🫧',level:92},{id:2,name:'Stone Wash',icon:'🪨',level:93},{id:3,name:'Vintage Wash',icon:'⚡',level:90},
    {id:4,name:'Acid Wash',icon:'💧',level:85},{id:5,name:'PP Spray',icon:'🎨',level:87},{id:6,name:'Indigo Wash',icon:'🔵',level:88},
    {id:7,name:'Silicone Softener',icon:'🧴',level:90},{id:8,name:'Pigment Dyeing',icon:'🎭',level:85},
    {id:9,name:'Reactive Dyeing',icon:'⚗️',level:82},{id:10,name:'Production Mgmt',icon:'🏭',level:90},
    {id:11,name:'Machine Troubleshoot',icon:'⚙️',level:85},{id:12,name:'Rejection Control',icon:'🔍',level:92},
  ],
  buyers:[
    {id:1,name:'GAP Denim Washing',proj:'Blue Creations Ltd. (2022–2025)',spec:'Managed full-scale denim washing for GAP International. Buyer lab dip approvals, production washing, and shade band maintenance across multiple seasons.',badge:'GAP RSL Compliant',icon:'🏷️',img:''},
    {id:2,name:'Denim Finishing',proj:'Fakir Apparels Ltd. (2025–Present)',spec:'Overseeing denim washing operations for international export buyers. Enzyme, stone, and specialty wash programs with zero-defect targets.',badge:'Export Quality',icon:'🌊',img:''},
    {id:3,name:'Chemical Optimization',proj:'Cross-Company Initiative',spec:'Led chemical process optimization projects to reduce production costs, improve quality, and comply with ZDHC requirements.',badge:'ZDHC MRSL Aligned',icon:'⚗️',img:''},
  ],
  contact:{name:'MD Naimur Rashid',jobTitle:'Executive – Washing',email:'mdnaimurrashid752@gmail.com',phone:'+8801626282048',loc:'Dhaka, Bangladesh',company:'Fakir Apparels Ltd., Narayanganj'},
  social:{li:'',yt:''},
  nextId:200,
};

// ══ INIT ══
function init(){
  renderAll();
  switchExp('denim',document.querySelector('.etab.active'));
  loadAdmForms();
}

function renderAll(){
  renderExpTimeline(); renderCertSidebar(); renderCertsGrid();
  renderPortGrid(); renderCasesGrid(); renderSkillsGrid(); renderBuyersGrid();
  renderContactInfo(); renderFooterContacts(); renderAdmTables(); renderAdmStats();
  renderStatsBar();
}

// ══ STATS BAR ══
function renderStatsBar(){
  document.getElementById('statsBar').innerHTML = DB.stats.map(s=>`
    <div class="si"><span style="font-size:1.15rem">${s.icon}</span><div><div class="si-num">${s.num}</div><div class="si-lbl">${s.lbl}</div></div></div>`).join('');
}

// ══ EXPERTISE ══
function switchExp(tab,btn){
  document.querySelectorAll('.etab').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');
  document.getElementById('expList').innerHTML = DB.expertise[tab].map(i=>`<li><span>${i.i}</span><span style="color:var(--blue2);font-size:.7rem">⟶</span><span>${i.t}</span></li>`).join('');
}

// ══ EXPERIENCE TIMELINE ══
function renderExpTimeline(){
  document.getElementById('expTimeline').innerHTML = DB.experience.map(e=>`
    <div class="etl-item${e.cur?' cur':''}">
      <div class="etl-dot"></div>
      <div class="etl-role">${e.role}</div>
      <div class="etl-co">${e.co}</div>
      <div class="etl-date">${e.date}</div>
      ${e.buyer?`<div class="etl-buyer">${e.buyer}</div>`:''}
    </div>`).join('');
}

// ══ CERTS ══
function renderCertSidebar(){
  document.getElementById('certSidebar').innerHTML = DB.certs.slice(0,4).map(c=>`
    <div class="cert-si" onclick="openCert(${c.id})">
      <div class="cert-si-img">${c.img?`<img src="${c.img}" style="width:100%;height:100%;object-fit:cover;border-radius:6px" onerror="this.style.display='none'">`:''}${!c.img?c.icon:''}</div>
      <div><div class="cert-si-name">${c.name.length>32?c.name.slice(0,32)+'…':c.name}</div><div class="cert-si-org">${c.org}</div></div>
      <div class="cert-arrow">›</div>
    </div>`).join('');
}
function renderCertsGrid(){
  document.getElementById('certsGrid').innerHTML = DB.certs.map(c=>`
    <div class="cert-card" onclick="openCert(${c.id})">
      <div class="cert-card-img">${c.img?`<img src="${c.img}" onerror="this.style.display='none'">`:''}${!c.img?`<span>${c.icon}</span>`:''}</div>
      <div class="cert-card-body"><div class="cert-card-org">${c.org}</div><div class="cert-card-name">${c.name}</div></div>
    </div>`).join('');
}
function openCert(id){
  const c=DB.certs.find(x=>x.id===id); if(!c) return;
  document.getElementById('cmImg').innerHTML = c.img?`<img src="${c.img}" style="width:100%;height:100%;object-fit:cover">`:`<span style="font-size:5rem">${c.icon}</span>`;
  document.getElementById('cmName').textContent=c.name;
  document.getElementById('cmOrg').textContent=c.org;
  document.getElementById('cmDesc').textContent=c.desc;
  document.getElementById('certOver').classList.add('open');
}

// ══ PORTFOLIO ══
function renderPortGrid(){
  document.getElementById('portGrid').innerHTML = DB.portfolio.map(p=>`
    <div class="port-card" data-pc="${p.cat}" onclick="openWash(${p.id})">
      <div class="port-img">
        ${p.img?`<img src="${p.img}" onerror="this.style.display='none'">`:''}
        <span style="position:relative;z-index:1">${p.icon}</span>
        <div class="port-ov"></div>
      </div>
      <div class="port-lbl"><span class="port-name">${p.name}</span><span class="port-tech">${p.tech}</span></div>
    </div>`).join('');
}
function openWash(id){
  const p=DB.portfolio.find(x=>x.id===id); if(!p) return;
  document.getElementById('wmImg').innerHTML = p.img?`<img src="${p.img}" style="width:100%;height:100%;object-fit:cover">`:`<span style="font-size:4rem">${p.icon}</span>`;
  document.getElementById('wmCat').textContent=p.cat.toUpperCase()+' · '+p.tech;
  document.getElementById('wmName').textContent=p.name;
  document.getElementById('wmDesc').textContent=p.desc;
  document.getElementById('washOver').classList.add('open');
}
function filterPort(cat,btn){
  document.querySelectorAll('.pf-btn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');
  document.querySelectorAll('.port-card').forEach(c=>{ c.style.display=(cat==='all'||c.dataset.pc===cat)?'block':'none'; });
}

// ══ CASES ══
function renderCasesGrid(){
  document.getElementById('casesGrid').innerHTML = DB.cases.map(c=>`
    <div class="case-card sa vis">
      <div class="case-head"><div class="case-buyer">${c.buyer}</div><div class="case-title">${c.title}</div></div>
      <div class="case-body">
        ${c.tech?`<div class="case-row"><span class="cl">Technique:</span><span class="cv2">${c.tech}</span></div>`:''}
        ${c.machine?`<div class="case-row"><span class="cl">Machine:</span><span class="cv2">${c.machine}</span></div>`:''}
        ${c.chem?`<div class="case-row"><span class="cl">Chemicals:</span><span class="cv2">${c.chem}</span></div>`:''}
        ${c.chall?`<div class="case-row"><span class="cl">Challenge:</span><span class="cv2">${c.chall}</span></div>`:''}
        ${c.result?`<div class="case-result">✅ ${c.result}</div>`:''}
      </div>
    </div>`).join('');
}

// ══ SKILLS ══
function renderSkillsGrid(){
  document.getElementById('skillsGrid').innerHTML = DB.skills.map(s=>`
    <div class="sk-card" style="opacity:1;transform:none">
      <div class="sk-icon">${s.icon}</div>
      <div class="sk-name">${s.name}</div>
      <div class="sk-bar"><div class="sk-fill" style="width:${s.level}%"></div></div>
    </div>`).join('');
}

// ══ BUYERS ══
function renderBuyersGrid(){
  document.getElementById('buyersGrid').innerHTML = DB.buyers.map(b=>`
    <div class="buyer-card">
      <div class="logo">${b.img?`<img src="${b.img}" onerror="this.style.display='none'">${b.icon}`:b.icon}</div>
      <div class="buyer-name">${b.name}</div>
      <div class="buyer-proj">${b.proj}</div>
      <div class="buyer-spec">${b.spec}</div>
      <div class="q-badge">✅ ${b.badge}</div>
    </div>`).join('');
}

// ══ CONTACT ══
function renderContactInfo(){
  const c=DB.contact;
  document.getElementById('contactInfoEl').innerHTML=`
    <p style="color:var(--text2);font-size:.88rem;line-height:1.8;margin-bottom:1.2rem">Available for washing consultations, buyer discussions, and technical project collaborations.</p>
    <div class="ci"><div class="ci-icon">📧</div><div><div class="ci-lbl">Email</div><div class="ci-val">${c.email}</div></div></div>
    <div class="ci"><div class="ci-icon">📞</div><div><div class="ci-lbl">Phone / WhatsApp</div><div class="ci-val">${c.phone}</div></div></div>
    <div class="ci"><div class="ci-icon">📍</div><div><div class="ci-lbl">Location</div><div class="ci-val">${c.loc}</div></div></div>
    <div class="ci"><div class="ci-icon">🏭</div><div><div class="ci-lbl">Current Company</div><div class="ci-val">${c.company}</div></div></div>`;
}
function renderFooterContacts(){
  const c=DB.contact;
  document.getElementById('footerContacts').innerHTML=`
    <div class="fc-item">✉️ ${c.email}</div>
    <div class="fc-item">📞 ${c.phone}</div>
    <div class="fc-item">📍 ${c.loc}</div>`;
}

// ══ HERO PHOTO ══
function prevHeroPhoto(url){
  const b=document.getElementById('heroPhotoPrev');
  if(url) b.innerHTML=`<img src="${url}" style="width:100%;height:100%;object-fit:cover;border-radius:50%" onerror="this.parentElement.innerHTML='<span>❌</span>'">`;
  else b.innerHTML='<span>🧑‍💼</span>';
}
function applyHeroPhoto(){
  const url=document.getElementById('heroPhotoUrl').value.trim();
  if(!url){showToast('❌ Please paste an image URL first');return;}
  DB.heroPhoto=url;
  const img=document.getElementById('heroPhotoImg');
  const ph=document.getElementById('photoPlaceholder');
  img.setAttribute('src',url);
  img.style.cssText='display:block;width:100%;height:100%;object-fit:cover;object-position:top center;position:absolute;inset:0;border-radius:0;';
  ph.style.display='none';
  showToast('✅ Hero photo applied!');
}
function removeHeroPhoto(){
  DB.heroPhoto='';
  document.getElementById('heroPhotoUrl').value='';
  document.getElementById('heroPhotoImg').style.display='none';
  document.getElementById('heroPhotoImg').src='';
  document.getElementById('photoPlaceholder').style.display='flex';
  document.getElementById('heroPhotoPrev').innerHTML='<span>🧑‍💼</span>';
  showToast('Photo removed');
}
function testSamplePhoto(){
  const sampleUrl='https://i.pravatar.cc/400?img=11';
  document.getElementById('heroPhotoUrl').value=sampleUrl;
  prevHeroPhoto(sampleUrl);
  applyHeroPhoto();
}

// ══ HERO CONTENT SAVE ══
function saveHero(){
  const h=DB.hero;
  h.fn=document.getElementById('hFn').value||h.fn;
  h.ln=document.getElementById('hLn').value||h.ln;
  h.title=document.getElementById('hTitle').value||h.title;
  h.eyebrow=document.getElementById('hEyebrow').value||h.eyebrow;
  h.pgdTitle=document.getElementById('hPgdTitle').value||h.pgdTitle;
  h.pgdSub=document.getElementById('hPgdSub').value||h.pgdSub;
  h.p1=document.getElementById('hP1').value||h.p1;
  h.p2=document.getElementById('hP2').value||h.p2;
  h.p3=document.getElementById('hP3').value||h.p3;
  document.getElementById('hero-fn').textContent=h.fn;
  document.getElementById('hero-ln').textContent=h.ln;
  document.getElementById('hero-title').textContent=h.title;
  document.getElementById('hero-eyebrow-text').textContent=h.eyebrow;
  document.getElementById('hero-pgd-title').textContent=h.pgdTitle;
  document.getElementById('hero-pgd-sub').textContent=h.pgdSub;
  document.getElementById('hero-perks').innerHTML=[h.p1,h.p2,h.p3].map(p=>`<div class="perk"><span>⚡</span>${p}</div>`).join('');
  document.getElementById('nav-name').textContent=h.fn+' '+h.ln;
  showToast('✅ Hero content updated!');
}

// ══ STATS SAVE ══
function loadStatsForm(){
  document.getElementById('statsFormEl').innerHTML=DB.stats.map((s,i)=>`
    <div style="display:grid;grid-template-columns:60px 80px 1fr;gap:.5rem;margin-bottom:.6rem;align-items:center">
      <input class="ai" placeholder="Icon" value="${s.icon}" id="st_icon_${i}" style="text-align:center" maxlength="4">
      <input class="ai" placeholder="Number" value="${s.num}" id="st_num_${i}">
      <input class="ai" placeholder="Label" value="${s.lbl}" id="st_lbl_${i}">
    </div>`).join('');
}
function saveStats(){
  DB.stats=DB.stats.map((s,i)=>({icon:document.getElementById('st_icon_'+i)?.value||s.icon,num:document.getElementById('st_num_'+i)?.value||s.num,lbl:document.getElementById('st_lbl_'+i)?.value||s.lbl}));
  renderStatsBar(); showToast('✅ Stats updated!');
}

// ══ EXPERTISE SAVE ══
function loadExpertiseForm(){
  const tabs=['denim','knit','woven','dyeing'];
  document.getElementById('expertiseFormEl').innerHTML=tabs.map(tab=>`
    <div style="margin-bottom:1rem">
      <label class="al">${tab.toUpperCase()} Tab Skills (one per line, use HTML for bold)</label>
      <textarea class="ai" id="exp_${tab}" rows="5">${DB.expertise[tab].map(i=>i.i+' '+i.t.replace(/<\/?strong>/g,'')).join('\n')}</textarea>
    </div>`).join('');
}
function saveExpertise(){
  const tabs=['denim','knit','woven','dyeing'];
  tabs.forEach(tab=>{
    const v=document.getElementById('exp_'+tab)?.value||'';
    DB.expertise[tab]=v.split('\n').filter(l=>l.trim()).map(l=>{
      const icon=l.match(/^(\S+)/)?.[1]||'•';
      const text=l.replace(/^\S+\s*/,'');
      return {i:icon,t:text};
    });
  });
  showToast('✅ Expertise updated!');
}

// ══ R&D SAVE ══
function prevRndImg(url){
  const b=document.getElementById('rndImgPrevBox');
  if(url) b.innerHTML=`<img src="${url}" style="width:100%;height:100%;object-fit:cover;border-radius:6px" onerror="this.parentElement.innerHTML='<span>❌</span>'">`;
  else b.innerHTML='<span>🌿</span>';
}
function saveRnd(){
  const r=DB.rnd;
  r.title=document.getElementById('rndTitleInp').value||r.title;
  r.p1=document.getElementById('rndP1').value||r.p1;
  r.p2=document.getElementById('rndP2').value||r.p2;
  r.p3=document.getElementById('rndP3').value||r.p3;
  r.img=document.getElementById('rndImgUrl').value.trim();
  document.getElementById('rndTitle').textContent=r.title;
  document.getElementById('rndPoints').innerHTML=[r.p1,r.p2,r.p3].map(p=>`<div class="rnd-pt"><div class="rnd-dot"></div>${p}</div>`).join('');
  if(r.img){document.getElementById('rndImg').src=r.img;document.getElementById('rndImg').style.display='block';document.getElementById('rndImgPh').style.display='none';}
  else{document.getElementById('rndImg').style.display='none';document.getElementById('rndImgPh').style.display='block';}
  showToast('✅ R&D content updated!');
}

// ══ EXPERIENCE CRUD ══
let editExpId=null;
function showExpForm(){editExpId=null;document.getElementById('expFormTitle').textContent='Add Experience';['fExpRole','fExpCo','fExpDate','fExpBuyer','fExpLoc','fExpDuties'].forEach(id=>document.getElementById(id).value='');document.getElementById('expFormWrap').style.display='block';}
function editExp(id){
  const e=DB.experience.find(x=>x.id===id); if(!e) return; editExpId=id;
  document.getElementById('expFormTitle').textContent='Edit Experience';
  document.getElementById('fExpRole').value=e.role;document.getElementById('fExpCo').value=e.co;
  document.getElementById('fExpDate').value=e.date;document.getElementById('fExpBuyer').value=e.buyer||'';
  document.getElementById('fExpLoc').value=e.loc||'';document.getElementById('fExpDuties').value=e.duties||'';
  document.getElementById('expFormWrap').style.display='block';
}
function saveExp(){
  const role=document.getElementById('fExpRole').value.trim();const co=document.getElementById('fExpCo').value.trim();
  if(!role||!co){showToast('❌ Role and Company required');return;}
  const data={role,co,date:document.getElementById('fExpDate').value.trim(),buyer:document.getElementById('fExpBuyer').value.trim(),loc:document.getElementById('fExpLoc').value.trim(),duties:document.getElementById('fExpDuties').value.trim(),cur:false};
  if(editExpId) Object.assign(DB.experience.find(x=>x.id===editExpId),data);
  else DB.experience.unshift({id:DB.nextId++,...data,cur:DB.experience.length===0});
  document.getElementById('expFormWrap').style.display='none';
  renderExpTimeline();renderAdmTables();showToast('✅ Experience saved!');
}
function delExp(id){if(confirm('Delete?')){DB.experience=DB.experience.filter(x=>x.id!==id);renderExpTimeline();renderAdmTables();showToast('Deleted');}}

// ══ EDUCATION CRUD ══
let editEduId=null;
function showEduForm(){editEduId=null;['fEduDeg','fEduInst','fEduYear','fEduGpa','fEduNote'].forEach(id=>document.getElementById(id).value='');document.getElementById('eduFormWrap').style.display='block';}
function saveEdu(){
  const deg=document.getElementById('fEduDeg').value.trim();const inst=document.getElementById('fEduInst').value.trim();
  if(!deg||!inst){showToast('❌ Degree and Institution required');return;}
  const data={deg,inst,year:document.getElementById('fEduYear').value.trim(),gpa:document.getElementById('fEduGpa').value.trim(),note:document.getElementById('fEduNote').value.trim()};
  if(editEduId) Object.assign(DB.education.find(x=>x.id===editEduId),data);
  else DB.education.push({id:DB.nextId++,...data});
  document.getElementById('eduFormWrap').style.display='none';renderAdmTables();showToast('✅ Education saved!');
}
function delEdu(id){if(confirm('Delete?')){DB.education=DB.education.filter(x=>x.id!==id);renderAdmTables();showToast('Deleted');}}

// ══ CERT CRUD ══
let editCertId=null;
function showCertForm(){editCertId=null;document.getElementById('certFormTitle').textContent='Add Certificate';['fCertName','fCertOrg','fCertDesc','fCertImg','fCertIcon'].forEach(id=>document.getElementById(id).value='');document.getElementById('fCertImgPrev').innerHTML='<span id="fCertImgPh">📋</span>';document.getElementById('certFormWrap').style.display='block';}
function prevCertImg(url){const b=document.getElementById('fCertImgPrev');if(url)b.innerHTML=`<img src="${url}" style="width:100%;height:100%;object-fit:cover;border-radius:6px" onerror="this.parentElement.innerHTML='<span>❌</span>'">`;else b.innerHTML='<span>📋</span>';}
function editCert(id){
  const c=DB.certs.find(x=>x.id===id);if(!c)return;editCertId=id;
  document.getElementById('certFormTitle').textContent='Edit Certificate';
  document.getElementById('fCertName').value=c.name;document.getElementById('fCertOrg').value=c.org;
  document.getElementById('fCertDesc').value=c.desc;document.getElementById('fCertImg').value=c.img||'';
  document.getElementById('fCertIcon').value=c.icon||'🎓';
  if(c.img) document.getElementById('fCertImgPrev').innerHTML=`<img src="${c.img}" style="width:100%;height:100%;object-fit:cover;border-radius:6px">`;
  document.getElementById('certFormWrap').style.display='block';
}
function saveCert(){
  const name=document.getElementById('fCertName').value.trim();const org=document.getElementById('fCertOrg').value.trim();
  if(!name||!org){showToast('❌ Name and Organization required');return;}
  const data={name,org,desc:document.getElementById('fCertDesc').value.trim(),img:document.getElementById('fCertImg').value.trim(),icon:document.getElementById('fCertIcon').value.trim()||'🎓'};
  if(editCertId) Object.assign(DB.certs.find(x=>x.id===editCertId),data);
  else DB.certs.push({id:DB.nextId++,...data});
  document.getElementById('certFormWrap').style.display='none';
  renderCertSidebar();renderCertsGrid();renderAdmTables();renderAdmStats();showToast('✅ Certificate saved!');
}
function delCert(id){if(confirm('Delete?')){DB.certs=DB.certs.filter(x=>x.id!==id);renderCertSidebar();renderCertsGrid();renderAdmTables();renderAdmStats();showToast('Deleted');}}

// ══ PORTFOLIO CRUD ══
let editPortId=null;
function showPortForm(){editPortId=null;document.getElementById('portFormTitle').textContent='Add Portfolio Item';['fPortName','fPortTech','fPortDesc','fPortImg','fPortEmoji'].forEach(id=>document.getElementById(id).value='');document.getElementById('fPortImgPrev').innerHTML='<span id="fPortImgPh">👔</span>';document.getElementById('portFormWrap').style.display='block';}
function prevPortImg(url){const b=document.getElementById('fPortImgPrev');if(url)b.innerHTML=`<img src="${url}" style="width:100%;height:100%;object-fit:cover;border-radius:6px" onerror="this.parentElement.innerHTML='<span>❌</span>'">`;else b.innerHTML='<span>👔</span>';}
function editPort(id){
  const p=DB.portfolio.find(x=>x.id===id);if(!p)return;editPortId=id;
  document.getElementById('portFormTitle').textContent='Edit Portfolio Item';
  document.getElementById('fPortName').value=p.name;document.getElementById('fPortCat').value=p.cat;
  document.getElementById('fPortTech').value=p.tech;document.getElementById('fPortDesc').value=p.desc;
  document.getElementById('fPortImg').value=p.img||'';document.getElementById('fPortEmoji').value=p.icon||'';
  prevPortImg(p.img);document.getElementById('portFormWrap').style.display='block';
}
function savePort(){
  const name=document.getElementById('fPortName').value.trim();if(!name){showToast('❌ Title required');return;}
  const data={name,cat:document.getElementById('fPortCat').value,tech:document.getElementById('fPortTech').value.trim(),desc:document.getElementById('fPortDesc').value.trim(),img:document.getElementById('fPortImg').value.trim(),icon:document.getElementById('fPortEmoji').value.trim()||'👔'};
  if(editPortId) Object.assign(DB.portfolio.find(x=>x.id===editPortId),data);
  else DB.portfolio.push({id:DB.nextId++,...data});
  document.getElementById('portFormWrap').style.display='none';
  renderPortGrid();renderAdmTables();renderAdmStats();showToast('✅ Portfolio item saved!');
}
function delPort(id){if(confirm('Delete?')){DB.portfolio=DB.portfolio.filter(x=>x.id!==id);renderPortGrid();renderAdmTables();renderAdmStats();showToast('Deleted');}}

// ══ CASE STUDIES CRUD ══
let editCaseId=null;
function showCaseForm(){editCaseId=null;document.getElementById('caseFormTitle').textContent='Add Case Study';['fCaseBuyer','fCaseTitle','fCaseTech','fCaseMachine','fCaseChem','fCaseChall','fCaseResult'].forEach(id=>document.getElementById(id).value='');document.getElementById('caseFormWrap').style.display='block';}
function editCase(id){
  const c=DB.cases.find(x=>x.id===id);if(!c)return;editCaseId=id;
  document.getElementById('caseFormTitle').textContent='Edit Case Study';
  document.getElementById('fCaseBuyer').value=c.buyer;document.getElementById('fCaseTitle').value=c.title;
  document.getElementById('fCaseTech').value=c.tech;document.getElementById('fCaseMachine').value=c.machine||'';
  document.getElementById('fCaseChem').value=c.chem||'';document.getElementById('fCaseChall').value=c.chall||'';
  document.getElementById('fCaseResult').value=c.result;document.getElementById('caseFormWrap').style.display='block';
}
function saveCaseStudy(){
  const title=document.getElementById('fCaseTitle').value.trim();if(!title){showToast('❌ Title required');return;}
  const data={buyer:document.getElementById('fCaseBuyer').value.trim(),title,tech:document.getElementById('fCaseTech').value.trim(),machine:document.getElementById('fCaseMachine').value.trim(),chem:document.getElementById('fCaseChem').value.trim(),chall:document.getElementById('fCaseChall').value.trim(),result:document.getElementById('fCaseResult').value.trim()};
  if(editCaseId) Object.assign(DB.cases.find(x=>x.id===editCaseId),data);
  else DB.cases.push({id:DB.nextId++,...data});
  document.getElementById('caseFormWrap').style.display='none';
  renderCasesGrid();renderAdmTables();showToast('✅ Case study saved!');
}
function delCase(id){if(confirm('Delete?')){DB.cases=DB.cases.filter(x=>x.id!==id);renderCasesGrid();renderAdmTables();showToast('Deleted');}}

// ══ SKILLS CRUD ══
function showSkillForm(){document.getElementById('skillFormWrap').style.display='block';['fSkName','fSkIcon','fSkLevel'].forEach(id=>document.getElementById(id).value='');}
function saveSkill(){
  const name=document.getElementById('fSkName').value.trim();if(!name){showToast('❌ Name required');return;}
  DB.skills.push({id:DB.nextId++,name,icon:document.getElementById('fSkIcon').value.trim()||'⭐',level:parseInt(document.getElementById('fSkLevel').value)||80});
  document.getElementById('skillFormWrap').style.display='none';renderSkillsGrid();renderAdmTables();renderAdmStats();showToast('✅ Skill added!');
}
function delSkill(id){DB.skills=DB.skills.filter(x=>x.id!==id);renderSkillsGrid();renderAdmTables();renderAdmStats();showToast('Deleted');}

// ══ BUYERS CRUD ══
let editBuyerId=null;
function showBuyerForm(){editBuyerId=null;document.getElementById('buyerFormTitle').textContent='Add Buyer Project';['fBuyerName','fBuyerProj','fBuyerSpec','fBuyerBadge','fBuyerIcon','fBuyerImg'].forEach(id=>document.getElementById(id).value='');document.getElementById('fBuyerImgPrev').innerHTML='<span id="fBuyerImgPh">🏷️</span>';document.getElementById('buyerFormWrap').style.display='block';}
function prevBuyerImg(url){const b=document.getElementById('fBuyerImgPrev');if(url)b.innerHTML=`<img src="${url}" style="width:100%;height:100%;object-fit:cover;border-radius:6px" onerror="this.parentElement.innerHTML='<span>❌</span>'">`;else b.innerHTML='<span>🏷️</span>';}
function editBuyer(id){
  const b=DB.buyers.find(x=>x.id===id);if(!b)return;editBuyerId=id;
  document.getElementById('buyerFormTitle').textContent='Edit Buyer Project';
  document.getElementById('fBuyerName').value=b.name;document.getElementById('fBuyerProj').value=b.proj;
  document.getElementById('fBuyerSpec').value=b.spec;document.getElementById('fBuyerBadge').value=b.badge;
  document.getElementById('fBuyerIcon').value=b.icon||'';document.getElementById('fBuyerImg').value=b.img||'';
  prevBuyerImg(b.img);document.getElementById('buyerFormWrap').style.display='block';
}
function saveBuyer(){
  const name=document.getElementById('fBuyerName').value.trim();if(!name){showToast('❌ Name required');return;}
  const data={name,proj:document.getElementById('fBuyerProj').value.trim(),spec:document.getElementById('fBuyerSpec').value.trim(),badge:document.getElementById('fBuyerBadge').value.trim(),icon:document.getElementById('fBuyerIcon').value.trim()||'🏢',img:document.getElementById('fBuyerImg').value.trim()};
  if(editBuyerId) Object.assign(DB.buyers.find(x=>x.id===editBuyerId),data);
  else DB.buyers.push({id:DB.nextId++,...data});
  document.getElementById('buyerFormWrap').style.display='none';renderBuyersGrid();renderAdmTables();showToast('✅ Buyer project saved!');
}
function delBuyer(id){if(confirm('Delete?')){DB.buyers=DB.buyers.filter(x=>x.id!==id);renderBuyersGrid();renderAdmTables();showToast('Deleted');}}

// ══ CONTACT & SOCIAL SAVE ══
function saveContact(){
  const f=id=>document.getElementById(id)?.value.trim();
  DB.contact.name=f('cName')||DB.contact.name;DB.contact.jobTitle=f('cJobTitle')||DB.contact.jobTitle;
  DB.contact.email=f('cEmail')||DB.contact.email;DB.contact.phone=f('cPhone')||DB.contact.phone;
  DB.contact.loc=f('cLoc')||DB.contact.loc;DB.contact.company=f('cCompany')||DB.contact.company;
  renderContactInfo();renderFooterContacts();showToast('✅ Contact info updated!');
}
function saveSocial(){
  DB.social.li=document.getElementById('sLI')?.value.trim()||'';
  DB.social.yt=document.getElementById('sYT')?.value.trim()||'';
  if(DB.social.li) document.getElementById('socLI').onclick=()=>window.open(DB.social.li,'_blank');
  if(DB.social.yt) document.getElementById('socYT').onclick=()=>window.open(DB.social.yt,'_blank');
  showToast('✅ Social links updated!');
}

// ══ ADMIN TABLES ══
function renderAdmTables(){
  document.getElementById('expTbody').innerHTML=DB.experience.map(e=>`<tr><td>${e.role}</td><td style="color:var(--gold)">${e.co}</td><td>${e.date}</td><td><button class="btn-e" onclick="editExp(${e.id})">Edit</button> <button class="btn-d" onclick="delExp(${e.id})">Del</button></td></tr>`).join('');
  document.getElementById('eduTbody').innerHTML=DB.education.map(e=>`<tr><td>${e.deg}</td><td>${e.inst}</td><td>${e.year}</td><td>${e.gpa}</td><td><button class="btn-d" onclick="delEdu(${e.id})">Del</button></td></tr>`).join('');
  document.getElementById('certTbody').innerHTML=DB.certs.map(c=>`<tr><td>${c.img?`<img src="${c.img}" class="tbl-thumb" onerror="this.style.display='none'">`:`<div class="tbl-ph">${c.icon}</div>`}</td><td>${c.name}</td><td>${c.org}</td><td><button class="btn-e" onclick="editCert(${c.id})">Edit</button> <button class="btn-d" onclick="delCert(${c.id})">Del</button></td></tr>`).join('');
  document.getElementById('portTbody').innerHTML=DB.portfolio.map(p=>`<tr><td>${p.img?`<img src="${p.img}" class="tbl-thumb" onerror="this.style.display='none'">`:`<div class="tbl-ph">${p.icon}</div>`}</td><td>${p.name}</td><td>${p.cat}</td><td>${p.tech}</td><td><button class="btn-e" onclick="editPort(${p.id})">Edit</button> <button class="btn-d" onclick="delPort(${p.id})">Del</button></td></tr>`).join('');
  document.getElementById('caseTbody').innerHTML=DB.cases.map(c=>`<tr><td style="color:var(--gold)">${c.buyer}</td><td>${c.title}</td><td>${c.tech}</td><td style="font-size:.7rem">${c.result?.slice(0,40)||''}...</td><td><button class="btn-e" onclick="editCase(${c.id})">Edit</button> <button class="btn-d" onclick="delCase(${c.id})">Del</button></td></tr>`).join('');
  document.getElementById('skillTbody').innerHTML=DB.skills.map(s=>`<tr><td>${s.icon}</td><td>${s.name}</td><td>${s.level}%</td><td><button class="btn-d" onclick="delSkill(${s.id})">Del</button></td></tr>`).join('');
  document.getElementById('buyerTbody').innerHTML=DB.buyers.map(b=>`<tr><td>${b.img?`<img src="${b.img}" class="tbl-thumb">`:`<div class="tbl-ph">${b.icon}</div>`}</td><td>${b.name}</td><td>${b.proj}</td><td><button class="btn-e" onclick="editBuyer(${b.id})">Edit</button> <button class="btn-d" onclick="delBuyer(${b.id})">Del</button></td></tr>`).join('');
}
function renderAdmStats(){
  document.getElementById('admStats').innerHTML=[
    {n:DB.certs.length,l:'Certificates'},{n:DB.portfolio.length,l:'Portfolio Items'},
    {n:DB.cases.length,l:'Case Studies'},{n:DB.skills.length,l:'Skills'},
    {n:DB.experience.length,l:'Experiences'},{n:DB.buyers.length,l:'Buyer Projects'},
  ].map(s=>`<div class="adm-sc"><div class="n">${s.n}</div><div class="l">${s.l}</div></div>`).join('');
}

// ══ ADMIN NAV & LOAD FORMS ══
function admNav(panel,el){
  document.querySelectorAll('.adm-nav').forEach(n=>n.classList.remove('active'));
  if(el) el.classList.add('active');
  document.querySelectorAll('.adm-panel').forEach(p=>p.classList.remove('active'));
  document.getElementById('ap-'+panel).classList.add('active');
  const tt={dash:'Dashboard',photo:'Hero Photo',hero:'Edit Hero Content',stats:'Stats Bar',expertise:'Expertise Tabs',rnd:'R&D Project',exp:'Work Experience',edu:'Education',certs:'Certificates',port:'Washing Portfolio',cases:'Case Studies',skills:'Technical Skills',buyers:'Buyer Projects',contact:'Contact Info',social:'Social Links'};
  document.getElementById('admTitle').textContent=tt[panel]||'Admin';
  if(panel==='stats') loadStatsForm();
  if(panel==='expertise') loadExpertiseForm();
  if(panel==='hero') loadHeroForm();
  if(panel==='contact') loadContactForm();
  if(panel==='rnd') loadRndForm();
}
function loadAdmForms(){}
function loadHeroForm(){
  const h=DB.hero;
  document.getElementById('hFn').value=h.fn;document.getElementById('hLn').value=h.ln;
  document.getElementById('hTitle').value=h.title;document.getElementById('hEyebrow').value=h.eyebrow;
  document.getElementById('hPgdTitle').value=h.pgdTitle;document.getElementById('hPgdSub').value=h.pgdSub;
  document.getElementById('hP1').value=h.p1;document.getElementById('hP2').value=h.p2;document.getElementById('hP3').value=h.p3;
}
function loadContactForm(){
  const c=DB.contact;
  document.getElementById('cName').value=c.name;document.getElementById('cJobTitle').value=c.jobTitle;
  document.getElementById('cEmail').value=c.email;document.getElementById('cPhone').value=c.phone;
  document.getElementById('cLoc').value=c.loc;document.getElementById('cCompany').value=c.company;
}
function loadRndForm(){
  const r=DB.rnd;
  document.getElementById('rndTitleInp').value=r.title;document.getElementById('rndP1').value=r.p1;
  document.getElementById('rndP2').value=r.p2;document.getElementById('rndP3').value=r.p3;
  document.getElementById('rndImgUrl').value=r.img||'';
}

// ══ LOGIN ══
function showLogin_old_removed(){}
function doLogin(){
  if(document.getElementById('aUser').value==='NaimurRashid'&&document.getElementById('aPass').value==='NaiM01688@'){
    document.getElementById('loginOver').classList.remove('open');
    document.getElementById('adm-wrap').style.display='block';
    document.body.style.overflow='hidden';
    if(document.getElementById('rememberMe').checked){
      localStorage.setItem('nr_admin_session','active');
    }
  } else{document.getElementById('lErr').style.display='block';}
}
function closeAdm(){
  document.getElementById('adm-wrap').style.display='none';
  document.body.style.overflow='';
}
function checkAdminSession(){
  if(localStorage.getItem('nr_admin_session')==='active'){
    // Auto-open admin silently — just show the gear icon is active
    document.getElementById('socAdm')?.setAttribute('title','Admin (saved)');
  }
}
function showLogin(){
  if(localStorage.getItem('nr_admin_session')==='active'){
    document.getElementById('adm-wrap').style.display='block';
    document.body.style.overflow='hidden';
  } else {
    document.getElementById('loginOver').classList.add('open');
  }
}

// ══ CHAT ══
const chatKB=[
  {t:['experience','work','company','fakir','blue','career'],r:'🏭 Experience:\n▸ Executive – Washing, Fakir Apparels Ltd. (2025–Present)\n▸ Denim Washing Executive, Blue Creations Ltd. (2022–2025) – GAP Buyer Responsible'},
  {t:['denim','wash','enzyme','stone','acid','pp spray','vintage'],r:'👖 Denim Washing:\n🫧 Enzyme (92%), 🪨 Stone (93%), ⚡ Vintage (90%)\n💧 Acid Wash (85%), 🎨 PP Spray (87%), 🔵 Indigo (88%)'},
  {t:['rnd','r&d','mordant','natural','hm','zara'],r:'🔬 R&D: Natural Mordant Development\nApproved by H&M & ZARA. Uses Betel Nut, Banana Peel & Guava Leaves. 60% synthetic chemical reduction.'},
  {t:['cert','sdc','cambridge','pgd'],r:'🎓 Certifications:\n• PGD Garments Business – IBA DU\n• Sustainable Dyeing – SDC\n• Textile Care Labelling – SDC\n• Colour Management – SDC\n• Critical Thinking – Cambridge'},
  {t:['contact','email','phone','reach'],r:'📧 mdnaimurrashid752@gmail.com\n📞 +8801626282048\n📍 Dhaka, Bangladesh'},
  {t:['education','buft','cgpa'],r:'🎓 BSc Textile Eng. – BUFT (CGPA 3.6/4.0, 2023)\n📚 PGD Garments Business – IBA, DU'},
];
function cs(t){document.getElementById('chatInp').value=t;chatSend();}
function getCR(inp){const l=inp.toLowerCase();for(const k of chatKB)if(k.t.some(t=>l.includes(t)))return k.r;return "I can help with: experience, denim washing, R&D projects, certifications, education, or contact details.";}
function chatSend(){
  const inp=document.getElementById('chatInp');const txt=inp.value.trim();if(!txt)return;
  const msgs=document.getElementById('chatMsgs');
  msgs.innerHTML+=`<div class="cm user"><div class="cm-b">${txt}</div></div>`;inp.value='';
  const tp=document.createElement('div');tp.className='cm bot';tp.innerHTML='<div class="cm-b"><div class="typing"><div class="td"></div><div class="td"></div><div class="td"></div></div></div>';
  msgs.appendChild(tp);msgs.scrollTop=msgs.scrollHeight;
  setTimeout(()=>{msgs.removeChild(tp);msgs.innerHTML+=`<div class="cm bot"><div class="cm-b">${getCR(txt).replace(/\n/g,'<br>')}</div></div>`;msgs.scrollTop=msgs.scrollHeight;},800);
}

// ══ CONTACT FORM ══
function cfSubmit(){
  if(!document.getElementById('cfName').value||!document.getElementById('cfEmail').value){showToast('❌ Please fill in all fields');return;}
  showToast('✅ Message sent! Will reply within 24 hours.');['cfName','cfEmail','cfMsg'].forEach(id=>document.getElementById(id).value='');
}

// ══ SCROLL ANIM ══
const saO=new IntersectionObserver(es=>{es.forEach(e=>{if(e.isIntersecting)e.target.classList.add('vis');});},{threshold:.07});
document.querySelectorAll('.sa').forEach(el=>saO.observe(el));

// ══ TOAST ══
function showToast(msg){const t=document.getElementById('toast');t.textContent=msg;t.style.display='block';setTimeout(()=>t.style.display='none',3200);}

// ══ CV ══
function genCV(){
  const {jsPDF}=window.jspdf;const doc=new jsPDF();const w=doc.internal.pageSize.width;const h=doc.internal.pageSize.height;
  const c=DB.contact;const hero=DB.hero;
  doc.setFillColor(6,13,26);doc.rect(0,0,w,48,'F');
  doc.setFillColor(240,165,0);doc.rect(0,46,w,2,'F');
  doc.setFont('helvetica','bold');doc.setFontSize(22);doc.setTextColor(255,255,255);
  doc.text((hero.fn+' '+hero.ln).toUpperCase(),15,18);
  doc.setFontSize(10);doc.setTextColor(240,165,0);doc.text(hero.title,15,28);
  doc.setFontSize(8.5);doc.setTextColor(150,180,210);
  doc.text(`${c.email}  |  ${c.phone}  |  ${c.loc}`,15,38);
  let y=60;
  const sec=t=>{if(y>h-18){doc.addPage();y=18;}doc.setFillColor(6,13,26);doc.rect(12,y-6,w-24,8,'F');doc.setFont('helvetica','bold');doc.setFontSize(9.5);doc.setTextColor(240,165,0);doc.text(t.toUpperCase(),15,y);y+=9;};
  const bul=t=>{doc.setFont('helvetica','normal');doc.setFontSize(8.8);doc.setTextColor(50,65,85);const ls=doc.splitTextToSize('• '+t,w-35);ls.forEach(l=>{if(y>h-14){doc.addPage();y=16;}doc.text(l,18,y);y+=5.2;});};
  sec('Professional Summary');
  const s=doc.splitTextToSize('Motivated Textile Engineer with 3+ years experience in denim washing and garment finishing. Currently Executive (Washing) at Fakir Apparels Ltd. Expertise in garment washing processes, chemical application, and production optimization. Led R&D project on Natural Mordant Development approved by H&M and ZARA.',w-32);
  doc.setFont('helvetica','normal');doc.setFontSize(8.8);doc.setTextColor(50,65,85);doc.text(s,15,y);y+=s.length*5.2+4;
  sec('Work Experience');
  DB.experience.forEach(e=>{
    doc.setFont('helvetica','bold');doc.setFontSize(9.5);doc.setTextColor(6,13,26);doc.text(`${e.role} | ${e.co}`,15,y);
    doc.setFont('helvetica','italic');doc.setFontSize(8.5);doc.setTextColor(100,120,140);doc.text(`${e.date}${e.loc?' | '+e.loc:''}`,15,y+5);y+=12;
    if(e.duties)e.duties.split('\n').filter(d=>d.trim()).forEach(d=>bul(d));y+=2;
  });
  sec('Education');
  DB.education.forEach(e=>bul(`${e.deg} – ${e.inst}${e.year?' ('+e.year+')':''}${e.gpa?' CGPA: '+e.gpa:''}${e.note?' · '+e.note:''}`));y+=2;
  sec('Technical Skills');
  const groups={'Washing':DB.skills.slice(0,6).map(s=>s.name).join(', '),'Production':DB.skills.slice(6).map(s=>s.name).join(', ')};
  Object.entries(groups).forEach(([k,v])=>bul(`${k}: ${v}`));y+=2;
  sec('Certifications');
  DB.certs.forEach(c=>bul(`${c.name} – ${c.org}`));
  const pg=doc.internal.getNumberOfPages();
  for(let i=1;i<=pg;i++){doc.setPage(i);doc.setFillColor(6,13,26);doc.rect(0,h-10,w,10,'F');doc.setFont('helvetica','normal');doc.setFontSize(7.5);doc.setTextColor(100,130,160);doc.text(`${c.name}  |  ${c.email}  |  ${c.phone}`,w/2,h-3.5,{align:'center'});}
  doc.save('MD_Naimur_Rashid_CV.pdf');showToast('✅ CV downloaded!');
}

// ══ SUPABASE PERSISTENCE ══
const SB_URL  = 'https://dqpadfyqgykpuyqlqbpq.supabase.co';
const SB_KEY  = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6ImRxcGFkZnlxZ3lrcHV5cWxxYnBxIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NzI4ODgxMzEsImV4cCI6MjA4ODQ2NDEzMX0.yJbAAewX5s_IlotRxb46VIVY_NyES0oaQ7NDb2rilBI';
const SB_HDR  = {'Content-Type':'application/json','apikey':SB_KEY,'Authorization':'Bearer '+SB_KEY};

function getPayload(){
  return {
    heroPhoto:DB.heroPhoto, hero:DB.hero, stats:DB.stats, rnd:DB.rnd,
    experience:DB.experience, education:DB.education, certs:DB.certs,
    portfolio:DB.portfolio, cases:DB.cases, skills:DB.skills,
    buyers:DB.buyers, contact:DB.contact, social:DB.social, nextId:DB.nextId
  };
}

async function saveToCloud(){
  try{
    // upsert into portfolio_data where id = 'main'
    await fetch(SB_URL+'/rest/v1/portfolio_data', {
      method:'POST',
      headers:{...SB_HDR,'Prefer':'resolution=merge-duplicates'},
      body: JSON.stringify({id:'main', value: getPayload()})
    });
  }catch(e){ console.warn('Supabase save error:',e); }
}

async function loadFromCloud(){
  try{
    const r = await fetch(SB_URL+'/rest/v1/portfolio_data?id=eq.main&select=value', {headers:SB_HDR});
    const rows = await r.json();
    if(rows && rows[0] && rows[0].value && Object.keys(rows[0].value).length > 0){
      const saved = rows[0].value;
      Object.keys(saved).forEach(k=>{ if(k in DB) DB[k] = saved[k]; });
      return true;
    }
  }catch(e){ console.warn('Supabase load error:',e); }
  return false;
}

function restoreHeroPhoto(){
  if(DB.heroPhoto){
    const img = document.getElementById('heroPhotoImg');
    const ph  = document.getElementById('photoPlaceholder');
    img.setAttribute('src', DB.heroPhoto);
    img.style.cssText = 'display:block;width:100%;height:100%;object-fit:cover;object-position:top center;position:absolute;inset:0;border-radius:0;';
    ph.style.display = 'none';
  }
}

// Show saving indicator
function showSaving(){
  const t = document.getElementById('toast');
  t.textContent = '☁️ Saving to cloud...';
  t.style.display = 'block';
}

// Patch every save/delete function to also push to Supabase
(function patchSaves(){
  const names = [
    'applyHeroPhoto','saveHero','saveStats','saveRnd',
    'saveExp','saveEdu','saveCert','savePort',
    'saveCaseStudy','saveSkill','saveBuyer',
    'saveContact','saveSocial','saveExpertise',
    'delCert','delPort','delSkill','delExp',
    'delEdu','delCase','delBuyer'
  ];
  names.forEach(name=>{
    const orig = window[name];
    if(!orig) return;
    window[name] = function(...args){
      const result = orig.apply(this, args);
      saveToCloud().then(()=> showToast('✅ Saved! Everyone can see this now.'));
      return result;
    };
  });
})();

// ══ START ══
(async function start(){
  document.body.insertAdjacentHTML('beforeend',
    '<div id="loadOverlay" style="position:fixed;inset:0;background:rgba(247,244,255,.95);z-index:9999;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:1rem">' +
    '<div style="width:48px;height:48px;border:3px solid rgba(91,110,245,.2);border-top-color:#5b6ef5;border-radius:50%;animation:ring-spin 1s linear infinite"></div>' +
    '<div style="background:linear-gradient(135deg,#5b6ef5,#e0458a);-webkit-background-clip:text;-webkit-text-fill-color:transparent;font-family:Barlow Condensed,sans-serif;font-weight:700;font-size:1.1rem">Loading portfolio...</div>' +
    '</div>'
  );
  const loaded = await loadFromCloud();
  document.getElementById('loadOverlay')?.remove();
  init();
  restoreHeroPhoto();
  checkAdminSession();
  if(!loaded){ await saveToCloud(); }
})();
</script>
</body>
</html>
