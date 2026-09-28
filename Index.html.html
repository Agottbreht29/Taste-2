<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Perfect Taste — prototype</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Unbounded:wght@500;600;700;800&family=DM+Sans:opsz,wght@9..40,400;9..40,500;9..40,600;9..40,700&display=swap" rel="stylesheet">
<style>
  :root{
    --paper:#F1EAFB; --card:#FFFFFF; --ink:#221A2E; --muted:#7C7288; --faint:#ADA4B6;
    --line:rgba(34,26,46,0.09); --line-strong:rgba(34,26,46,0.16);
    --pink:#8FE6EB; --pink-ink:#086A72; --pink-fill:#D3F5F7;
    --brand:#8FE6EB; --brand-ink:#086A72; --brand-fill:#D3F5F7;
    --grape:#6D28D9; --grape-2:#8B45E8;
    --tang:#FF7A1A; --sun:#FFC01E; --teal:#0FB5A6;
    --green:#12A150; --green-fill:#DEF5E7; --green-ink:#0B6B38;
    --amber:#F59E0B; --amber-fill:#FFF0D6;
    --coral:#F0463C; --coral-fill:#FFE6E1;
    --shadow:0 2px 4px rgba(34,26,46,.05), 0 14px 32px rgba(34,26,46,.10);
    --sans:'DM Sans',system-ui,sans-serif; --serif:'Unbounded','DM Sans',sans-serif;
  }
  *{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
  html,body{margin:0;height:100%}
  body{
    background:#D9C9F2; font-family:var(--sans); color:var(--ink);
    display:flex; align-items:center; justify-content:center; padding:20px;
    background-image:radial-gradient(circle at 50% -8%, #ECE1FF 0%, #DED0F6 46%, #C6E8F1 100%);
  }
  /* ---------- phone frame ---------- */
  .phone{
    width:390px; max-width:100%; height:800px; max-height:94vh;
    background:var(--paper); border-radius:46px; position:relative; overflow:hidden;
    box-shadow:0 0 0 11px #1a1113, 0 0 0 13px #33232c, 0 34px 64px rgba(70,20,40,.32);
    display:flex; flex-direction:column;
  }
  .notch{position:absolute;top:12px;left:50%;transform:translateX(-50%);width:120px;height:26px;background:#1a1113;border-radius:0 0 16px 16px;z-index:60}
  .statusbar{height:46px;flex:none;display:flex;align-items:flex-end;justify-content:space-between;padding:0 26px 6px;font-size:13px;font-weight:600;color:var(--ink)}
  .screen{flex:1;position:relative;overflow:hidden}
  .view{position:absolute;inset:0;display:flex;flex-direction:column;overflow-y:auto;overflow-x:hidden;background:var(--paper);
    transition:transform .34s cubic-bezier(.32,.72,0,1), opacity .28s ease;}
  .view::-webkit-scrollbar{display:none}
  .view.stack-hidden{transform:translateX(28px);opacity:0;pointer-events:none}
  .view.stack-back{transform:translateX(-28px);opacity:0;pointer-events:none}
  @media (prefers-reduced-motion:reduce){.view{transition:opacity .2s ease}.view.stack-hidden,.view.stack-back{transform:none}}

  .pad{padding:0 22px}
  .topbar{display:flex;align-items:center;gap:14px;padding:8px 22px 4px;min-height:44px}
  .back{width:36px;height:36px;flex:none;border:1.5px solid var(--line-strong);border-radius:12px;background:var(--card);display:flex;align-items:center;justify-content:center;cursor:pointer;color:var(--ink);font-size:18px;font-weight:700}
  .back:active{background:var(--pink-fill);border-color:var(--pink)}
  .kicker{font-size:12px;font-weight:700;letter-spacing:.01em;color:var(--pink-ink)}
  h1.t{font-family:var(--serif);font-weight:700;font-size:26px;line-height:1.1;letter-spacing:-.03em;margin:8px 0 4px}
  .sub{font-size:14px;color:var(--muted);line-height:1.5;margin:0}

  /* ---------- logo ---------- */
  .logo{display:flex;align-items:center;gap:9px}
  .logo .dial{width:31px;height:31px;flex:none}
  .wm{font-family:var(--serif);font-weight:800;font-size:22px;letter-spacing:-.05em;color:var(--ink)}
  .wm b{color:var(--ink);font-weight:800}

  /* ---------- home ---------- */
  .sectlabel{font-size:13px;font-weight:700;color:var(--muted);margin:22px 22px 12px}

  /* ---------- dish list ---------- */
  .search{margin:12px 22px 6px;position:relative}
  .search input{width:100%;height:50px;border:1.5px solid var(--line-strong);border-radius:15px;background:var(--card);padding:0 16px 0 42px;font-family:var(--sans);font-size:15px;font-weight:500;color:var(--ink);outline:none}
  .search input:focus{border-color:var(--pink);box-shadow:0 0 0 3px rgba(18,196,206,.14)}
  .search .mag{position:absolute;left:15px;top:50%;transform:translateY(-50%);color:var(--brand-ink);font-size:16px}
  .dishlist{padding:8px 22px 0}
  .drow{display:flex;align-items:center;gap:14px;padding:15px 4px;border-bottom:1px solid var(--line);cursor:pointer}
  .drow:active{opacity:.55}
  .drow .dico{width:44px;height:44px;flex:none;border-radius:14px;background:var(--pink-fill);display:flex;align-items:center;justify-content:center;font-family:var(--serif);font-size:17px;color:var(--pink-ink);font-weight:700}
  .drow .dn{font-weight:600;font-size:15.5px}
  .drow .dm{font-size:12.5px;color:var(--faint);margin-top:1px}
  .addrow{margin:16px 22px 22px;border:1.5px dashed var(--line-strong);border-radius:16px;padding:15px;display:flex;align-items:center;gap:12px;cursor:pointer;background:transparent}
  .addrow:active{background:var(--pink-fill)}
  .addrow .plus{width:36px;height:36px;flex:none;border-radius:12px;background:var(--pink);color:#04353A;display:flex;align-items:center;justify-content:center;font-size:21px;font-weight:700}
  .addrow .an{font-weight:600;font-size:14.5px}
  .addrow .as{font-size:12px;color:var(--muted);margin-top:1px}

  /* ---------- manual + classify ---------- */
  .field{margin:18px 22px 0}
  .field label{display:block;font-size:13px;font-weight:700;color:var(--muted);margin-bottom:8px}
  .field input{width:100%;height:54px;border:1.5px solid var(--line-strong);border-radius:15px;background:var(--card);padding:0 16px;font-family:var(--serif);font-size:18px;font-weight:600;color:var(--ink);outline:none}
  .field input:focus{border-color:var(--pink);box-shadow:0 0 0 3px rgba(18,196,206,.14)}
  .hint{font-size:12.5px;color:var(--faint);margin:10px 22px 0;line-height:1.5}
  .suggest{margin:12px 22px 0}
  .suggest .sg{display:flex;align-items:center;gap:10px;background:var(--amber-fill);border:1px solid rgba(245,158,11,.3);border-radius:13px;padding:11px 13px;font-size:13.5px;color:#8A5A06;cursor:pointer}
  .suggest .sg b{font-weight:700}

  .thinking{margin:26px 22px 0;display:flex;flex-direction:column;align-items:center;text-align:center;gap:16px;padding-top:16px}
  .pulse{width:64px;height:64px;border-radius:50%;border:3px solid var(--pink);position:relative;display:flex;align-items:center;justify-content:center;font-family:var(--serif);font-weight:800;font-size:15px;color:var(--pink)}
  .pulse::after{content:"";position:absolute;inset:-3px;border-radius:50%;border:3px solid var(--pink);animation:ring 1.3s ease-out infinite}
  @keyframes ring{0%{transform:scale(1);opacity:.5}100%{transform:scale(1.5);opacity:0}}
  .thinking .tt{font-family:var(--serif);font-size:18px;font-weight:700}
  .thinking .ts{font-size:13.5px;color:var(--muted)}
  .dots span{display:inline-block;width:6px;height:6px;border-radius:50%;background:var(--pink);margin:0 2px;animation:bob 1s infinite}
  .dots span:nth-child(2){animation-delay:.15s}.dots span:nth-child(3){animation-delay:.3s}
  @keyframes bob{0%,60%,100%{transform:translateY(0);opacity:.4}30%{transform:translateY(-5px);opacity:1}}

  .idcard{margin:20px 22px 0;background:var(--card);border:1px solid var(--line);border-radius:20px;padding:20px;box-shadow:var(--shadow)}
  .idcard .found{font-size:12.5px;font-weight:700;color:var(--green);display:flex;align-items:center;gap:6px}
  .idcard .dishname{font-family:var(--serif);font-size:23px;font-weight:700;margin:9px 0 3px;letter-spacing:-.03em}
  .idcard .typeline{font-size:13.5px;color:var(--muted)}
  .idcard .divider{height:1px;background:var(--line);margin:16px 0}
  .idcard .scalelabel{font-size:12px;font-weight:700;color:var(--muted);margin-bottom:10px}
  .pills{display:flex;flex-wrap:wrap;gap:7px}
  .pill{font-size:12.5px;font-weight:600;padding:6px 11px;border-radius:999px;background:var(--grape);color:#fff}
  .catgrid{display:flex;flex-wrap:wrap;gap:9px;padding:6px 22px 0}
  .catchip{font-size:13.5px;font-weight:700;background:var(--card);border:1.5px solid var(--line-strong);border-radius:14px;padding:11px 14px;cursor:pointer;color:var(--ink)}
  .catchip:active{background:var(--brand-fill);border-color:var(--brand)}
  .selfnote{margin:14px 22px 0;font-size:12px;color:var(--faint);line-height:1.5;display:flex;gap:8px}
  .selfnote i{color:var(--pink);font-style:normal}

  /* ---------- rating ---------- */
  .dishhead{padding:4px 22px 6px}
  .dishhead .place{font-size:12.5px;color:var(--muted);display:flex;align-items:center;gap:6px;margin-bottom:5px}
  .dishhead .place .pin{width:6px;height:6px;border-radius:50%;background:var(--brand-ink)}
  .dishhead h2{font-family:var(--serif);font-weight:700;font-size:24px;margin:2px 0 0;letter-spacing:-.03em}
  .dishhead .instr{font-size:13px;color:var(--muted);margin:8px 0 0;line-height:1.45}
  .sliders{padding:6px 22px 4px}
  .srow{padding:17px 0;border-bottom:1px solid var(--line)}
  .srow .shead{display:flex;justify-content:space-between;align-items:baseline;margin-bottom:12px}
  .srow .sname{font-weight:700;font-size:15px}
  .srow .sverdict{font-size:12.5px;font-weight:700}
  .track{position:relative;height:36px;display:flex;align-items:center}
  .track .grad{position:absolute;left:0;right:0;height:10px;border-radius:6px;
    background:linear-gradient(90deg,var(--coral) 0%,var(--amber) 26%,var(--green) 50%,var(--amber) 74%,var(--coral) 100%);opacity:.6}
  .track .mid{position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);width:2px;height:18px;background:var(--ink);opacity:.4;border-radius:2px}
  .track input[type=range]{position:relative;-webkit-appearance:none;appearance:none;width:100%;height:36px;background:transparent;margin:0;cursor:pointer}
  .track input[type=range]::-webkit-slider-thumb{-webkit-appearance:none;appearance:none;width:28px;height:28px;border-radius:50%;background:var(--card);border:4px solid var(--tc,var(--green));box-shadow:0 3px 8px rgba(34,26,46,.24);cursor:grab}
  .track input[type=range]::-moz-range-thumb{width:28px;height:28px;border-radius:50%;background:var(--card);border:4px solid var(--tc,var(--green));box-shadow:0 3px 8px rgba(34,26,46,.24);cursor:grab}
  .ends{display:flex;justify-content:space-between;margin-top:5px;font-size:11.5px;color:var(--faint)}
  .ends .mididx{color:var(--muted);font-weight:600}

  .scorebar{position:sticky;bottom:0;background:linear-gradient(180deg,rgba(241,234,251,0) 0%,var(--paper) 24%);padding:14px 22px 20px;margin-top:4px}
  .scorecard{background:var(--grape);border-radius:18px;padding:16px 18px;display:flex;align-items:center;justify-content:space-between}
  .scorecard .slab{font-size:12.5px;color:rgba(255,255,255,.72)}
  .scorecard .sval{font-family:var(--serif);font-size:32px;font-weight:800;line-height:1;color:#fff}
  .verdictpill{font-size:12.5px;font-weight:700;padding:8px 14px;border-radius:999px}
  .cta{width:100%;height:54px;margin-top:12px;border:none;border-radius:16px;background:var(--pink);color:#04353A;font-family:var(--sans);font-size:16px;font-weight:700;cursor:pointer}
  .cta:active{transform:scale(.985)}
  .cta.ghost{background:transparent;color:var(--ink);border:1.5px solid var(--line-strong)}
  .cta.ghost:active{background:var(--pink-fill)}

  /* ---------- trend button + sort + pills ---------- */
  .trendbtn{flex:none;font-family:var(--sans);font-size:11.5px;font-weight:700;color:var(--grape);background:#EFE6FF;border:none;border-radius:10px;padding:8px 11px;cursor:pointer}
  .trendbtn:active{opacity:.7}
  .segwrap{display:flex;gap:4px;margin:12px 22px 2px;background:rgba(34,26,46,.06);border-radius:14px;padding:4px}
  .seg{flex:1;text-align:center;font-family:var(--sans);font-size:12.5px;font-weight:700;padding:10px 6px;border-radius:10px;color:var(--muted);cursor:pointer;border:none;background:transparent}
  .seg.on{background:var(--card);color:var(--ink);box-shadow:0 1px 3px rgba(34,26,46,.12)}
  .sortcap{font-size:11.5px;color:var(--faint);line-height:1.45;margin:8px 22px 0}
  .cutecap{display:flex;align-items:center;justify-content:center;gap:8px;text-align:center;margin:16px 22px 6px;background:var(--brand-fill);color:var(--brand-ink);border-radius:999px;padding:10px 16px;font-size:12.5px;font-weight:700;line-height:1.25}
  .cutecap svg{width:19px;height:16px;flex:none}
  .scorepill{flex:none;min-width:40px;text-align:center;font-family:var(--serif);font-size:14px;font-weight:800;padding:7px 9px;border-radius:12px}
  .rankno{flex:none;width:26px;text-align:center;font-family:var(--serif);font-weight:800;font-size:17px;color:var(--brand-ink)}
  .schead{border-bottom:none;cursor:default;padding-top:8px;padding-bottom:0}
  .schead:active{opacity:1}
  .ahdr{font-size:10.5px;font-weight:700;letter-spacing:.02em;color:var(--faint);white-space:nowrap;text-align:right}

  /* ---------- discovery ---------- */
  .hero{margin:8px 22px 0;background:var(--grape);border-radius:24px;padding:20px 18px 18px;position:relative;overflow:hidden}
  .hero::before{content:"";position:absolute;top:-34px;right:-24px;width:120px;height:120px;border-radius:50%;background:var(--grape-2)}
  .hero::after{content:"";position:absolute;bottom:-40px;left:-20px;width:96px;height:96px;border-radius:50%;background:rgba(18,196,206,.26)}
  .hero .hl{position:relative;font-family:var(--serif);font-weight:700;font-size:20px;letter-spacing:-.03em;color:#fff;margin-bottom:14px;line-height:1.16}
  .dsearch{position:relative}
  .dsearch input{width:100%;height:48px;border:1.5px solid rgba(255,255,255,.28);border-radius:13px;background:rgba(255,255,255,.14);padding:0 16px 0 40px;font-family:var(--sans);font-size:15px;font-weight:500;color:#fff;outline:none}
  .dsearch input::placeholder{color:rgba(255,255,255,.7)}
  .dsearch input:focus{border-color:var(--pink);background:rgba(255,255,255,.2)}
  .dsearch .mag{position:absolute;left:14px;top:50%;transform:translateY(-50%);color:var(--pink);font-size:16px}
  .chips{display:flex;flex-wrap:wrap;gap:8px;margin-top:13px;position:relative}
  .chip{font-size:12.5px;font-weight:700;border:none;border-radius:999px;padding:9px 14px;cursor:pointer}
  .chip:active{transform:scale(.95)}
  .orline{display:flex;align-items:center;gap:12px;margin:24px 22px 0;color:var(--ink);font-size:12.5px;font-weight:700}
  .orline::before,.orline::after{content:"";flex:1;height:1px;background:var(--line)}
  .rrow{display:flex;align-items:center;gap:13px;padding:15px 4px;border-bottom:1px solid var(--line);cursor:pointer}
  .rrow:active{opacity:.6}
  .rname{font-weight:700;font-size:15px}
  .rmeta{font-size:12px;color:var(--faint);margin-top:2px}
  .rverdict{font-size:12px;margin-top:4px;font-weight:700}
  .rright{margin-left:auto;display:flex;flex-direction:column;align-items:flex-end;gap:4px}
  .rn{font-size:10.5px;color:var(--faint)}
  .rlink{color:var(--brand-ink);font-weight:700;cursor:pointer;text-decoration:underline;text-underline-offset:2px}
  .rchev{color:var(--grape);font-size:22px;font-weight:700;flex:none;margin-left:2px}
  .inlink{color:var(--grape);font-weight:700;cursor:pointer;white-space:nowrap}
  .detcard{margin:12px 22px 0;background:var(--pink);border:none;border-radius:16px;padding:12px 15px;display:flex;align-items:center;gap:11px;cursor:pointer}
  .detcard:active{background:#0FB2BC}
  .detcard .dot{width:8px;height:8px;border-radius:50%;background:var(--grape);flex:none;box-shadow:0 0 0 3px rgba(109,40,217,.20)}
  .detcard .dinfo b{font-family:var(--sans);font-size:14.5px;font-weight:700;color:#04353A}
  .detcard .dmeta{font-size:11.5px;color:rgba(4,53,58,.7);margin-top:2px}
  .detcard .chev{margin-left:auto;color:var(--grape);font-size:21px;font-weight:700}
  .otherlink{display:block;text-align:center;margin:14px 22px 0;font-size:13px;color:var(--pink-ink);font-weight:700;cursor:pointer}

  /* ---------- publish / compare payoff ---------- */
  .pubhead{padding:16px 22px 2px;text-align:center}
  .pubhead .check{width:66px;height:66px;border-radius:50%;background:var(--pink);display:flex;align-items:center;justify-content:center;color:#04353A;font-size:32px;margin:6px auto 13px;animation:pop .4s cubic-bezier(.2,1.4,.4,1)}
  @keyframes pop{0%{transform:scale(0)}100%{transform:scale(1)}}
  .pubhead h2{font-family:var(--serif);font-weight:800;font-size:23px;margin:0;letter-spacing:-.03em}
  .pubhead p{font-size:13px;color:var(--muted);margin:7px 0 0;line-height:1.5}
  .cmplist{padding:6px 22px 0}
  .cmprow{padding:15px 0;border-bottom:1px solid var(--line)}
  .cmprow .cn{display:flex;justify-content:space-between;align-items:baseline}
  .cmprow .cn .nm{font-weight:700;font-size:14.5px}
  .agchip{font-size:11px;font-weight:700;padding:3px 9px;border-radius:999px;margin-left:8px}
  .agchip.ag{background:var(--green-fill);color:var(--green-ink)}
  .agchip.out{background:var(--amber-fill);color:#8A5A06}
  .cbarwrap{position:relative;height:16px;margin:12px 0 8px}
  .cbar{position:absolute;inset:4px 0;border-radius:5px;background:linear-gradient(90deg,var(--coral),var(--amber) 26%,var(--green) 50%,var(--amber) 74%,var(--coral));opacity:.6}
  .cmed{position:absolute;top:-1px;width:2px;height:18px;background:var(--ink);opacity:.55;border-radius:2px;transform:translateX(-1px)}
  .cyou{position:absolute;top:-1px;width:18px;height:18px;border-radius:50%;background:var(--card);border:4px solid var(--tc,var(--green));transform:translate(-50%,0);box-shadow:0 2px 5px rgba(34,26,46,.24)}
  .ccap{font-size:12px;color:var(--muted);line-height:1.5}
  .ccap b{color:var(--ink);font-weight:700}
  .legendrow{display:flex;gap:16px;justify-content:center;padding:10px 22px 2px;font-size:11.5px;color:var(--faint)}
  .legendrow i{font-style:normal;display:inline-flex;align-items:center;gap:5px}
  .lgmed{width:2px;height:12px;background:var(--ink);opacity:.55;display:inline-block}
  .lgyou{width:12px;height:12px;border-radius:50%;background:var(--card);border:3px solid var(--green);display:inline-block}

  /* ---------- trend page ---------- */
  .trendcard{margin:14px 22px 4px;background:var(--card);border:1px solid var(--line);border-radius:22px;padding:19px 20px;box-shadow:var(--shadow)}
  .trendcard .tk{font-size:12px;font-weight:700;color:var(--pink-ink);display:flex;align-items:center;gap:6px}
  .trendcard .tdn{font-family:var(--serif);font-size:24px;font-weight:800;margin:8px 0 2px;letter-spacing:-.03em}
  .trendcard .tpl{font-size:13px;color:var(--muted)}
  .trendcard .tstats{display:flex;gap:20px;margin-top:16px;padding-top:16px;border-top:1px solid var(--line)}
  .trendcard .tstat .sv{font-family:var(--serif);font-size:22px;font-weight:800;line-height:1}
  .trendcard .tstat .sl{font-size:11.5px;color:var(--muted);margin-top:4px}
  .trendcard .thl{margin-top:15px;font-size:13.5px;color:var(--grape);background:#F1E9FF;border-radius:12px;padding:12px 14px;line-height:1.45}
  .trendcard .thl b{color:var(--grape);font-weight:700}
  .disttip{font-size:12px;color:var(--faint);text-align:center;line-height:1.5;padding:14px 26px 4px}
  .dists{padding:4px 22px 0}
  .dscale{padding:16px 0;border-bottom:1px solid var(--line)}
  .dscale .dhead{display:flex;justify-content:space-between;align-items:baseline;margin-bottom:2px}
  .dscale .dname{font-weight:700;font-size:14.5px}
  .dscale .dverdict{font-size:12.5px;font-weight:700}
  .histo{position:relative;height:58px;display:flex;align-items:flex-end;gap:5px;padding-top:22px}
  .histo .hb{flex:1;border-radius:5px 5px 0 0;min-height:5px}
  .youpin{position:absolute;top:0;transform:translateX(-50%);display:flex;flex-direction:column;align-items:center;z-index:2}
  .youpin span{background:var(--ink);color:#fff;font-size:10px;font-weight:700;padding:2px 7px;border-radius:6px;white-space:nowrap}
  .youpin::after{content:"";width:0;height:0;border-left:4px solid transparent;border-right:4px solid transparent;border-top:5px solid var(--ink);margin-top:1px}
  .dscale .dends{display:flex;justify-content:space-between;margin-top:6px;font-size:11px;color:var(--faint)}
  .dscale .dcap{font-size:12.5px;color:var(--muted);margin-top:8px;display:flex;align-items:center;flex-wrap:wrap}
</style>
</head>
<body>
<div class="phone">
  <div class="notch"></div>
  <div class="statusbar"><span>9:41</span><span>Perfect Taste</span><span>&#9679;&#9679;&#9679; &#9723;</span></div>
  <div class="screen" id="screen"></div>
</div>

<script>
/* ---------------- data model ---------------- */
const SLIDERS = {
  salt:   {name:"Saltiness",     l:"Needs salt",       r:"Too salty",        vl:"under-salted", vr:"salty"},
  season: {name:"Seasoning",     l:"Bland",            r:"Overpowering",     vl:"bland",        vr:"over-seasoned"},
  portion:{name:"Portion",       l:"Too small",        r:"Too much",         vl:"small",        vr:"oversized"},
  temp:   {name:"Temperature",   l:"Too cold",         r:"Too hot",          vl:"cold",         vr:"hot"},
  sauce:  {name:"Sauciness",     l:"Too dry",          r:"Drowning",         vl:"dry",          vr:"saucy"},
  sweet:  {name:"Sweetness",     l:"Not sweet enough", r:"Too sweet",        vl:"under-sweet",  vr:"sweet"},
  acid:   {name:"Acidity",       l:"Flat",             r:"Too sour",         vl:"flat",         vr:"sour"},
  spice:  {name:"Spiciness",     l:"Too mild",         r:"Too hot",          vl:"mild",         vr:"spicy"},
  done:   {name:"Doneness",      l:"Undercooked",      r:"Overcooked",       vl:"underdone",    vr:"overdone"},
  crisp:  {name:"Crispiness",    l:"Soggy",            r:"Burnt",            vl:"soggy",        vr:"over-crisp"},
  tender: {name:"Tenderness",    l:"Tough",            r:"Mushy",            vl:"tough",        vr:"soft"},
  rich:   {name:"Richness",      l:"Too lean",         r:"Too heavy",        vl:"lean",         vr:"heavy"},
};
const TYPES = {
  burger:  {label:"burger",              keys:["salt","done","sauce","rich","portion"]},
  pasta:   {label:"pasta",               keys:["salt","sauce","done","rich","portion"]},
  pizza:   {label:"pizza",               keys:["salt","sauce","crisp","rich","portion"]},
  salad:   {label:"salad",               keys:["salt","sauce","acid","crisp","portion"]},
  steak:   {label:"steak / grilled meat",keys:["salt","done","tender","rich","temp"]},
  curry:   {label:"curry",               keys:["salt","spice","rich","sauce","portion"]},
  noodle:  {label:"stir-fried noodles",  keys:["salt","sauce","sweet","spice","portion"]},
  soup:    {label:"soup / broth dish",   keys:["salt","spice","rich","temp","portion"]},
  taco:    {label:"taco / wrap",         keys:["salt","spice","acid","sauce","portion"]},
  sushi:   {label:"sushi",               keys:["salt","temp","acid","portion"]},
  fried:   {label:"fried dish",          keys:["salt","crisp","rich","portion","temp"]},
  dessert: {label:"dessert",             keys:["sweet","rich","portion","temp"]},
  wings:   {label:"saucy wings",         keys:["salt","sauce","spice","crisp","portion"]},
  generic: {label:"we'll start with the basics",keys:["salt","season","portion","temp"]},
};
const CUISINES = [
  {id:"thai", name:"Thai", em:"T", dishes:[
    {n:"Pad Thai",t:"noodle"},{n:"Green Curry",t:"curry"},{n:"Pad See Ew",t:"noodle"},
    {n:"Tom Yum Soup",t:"soup"},{n:"Mango Sticky Rice",t:"dessert"}]},
  {id:"mex", name:"Mexican", em:"M", dishes:[
    {n:"Tacos al Pastor",t:"taco"},{n:"Chicken Burrito",t:"taco"},{n:"Enchiladas",t:"curry"},
    {n:"Quesadilla",t:"fried"},{n:"Elote",t:"generic"}]},
  {id:"ital", name:"Italian", em:"I", dishes:[
    {n:"Spaghetti Carbonara",t:"pasta"},{n:"Margherita Pizza",t:"pizza"},{n:"Lasagna",t:"pasta"},
    {n:"Cacio e Pepe",t:"pasta"},{n:"Tiramisu",t:"dessert"}]},
  {id:"amer", name:"American", em:"A", dishes:[
    {n:"Cheeseburger",t:"burger"},{n:"Caesar Salad",t:"salad"},{n:"Buffalo Wings",t:"wings"},
    {n:"Mac and Cheese",t:"pasta"},{n:"BBQ Ribs",t:"steak"}]},
  {id:"jpn", name:"Japanese", em:"J", dishes:[
    {n:"Salmon Nigiri",t:"sushi"},{n:"Tonkotsu Ramen",t:"soup"},{n:"Chicken Katsu",t:"fried"},
    {n:"Gyoza",t:"fried"},{n:"California Roll",t:"sushi"}]},
  {id:"ind", name:"Indian", em:"In", dishes:[
    {n:"Butter Chicken",t:"curry"},{n:"Chicken Biryani",t:"generic"},{n:"Samosa",t:"fried"},
    {n:"Palak Paneer",t:"curry"},{n:"Garlic Naan",t:"generic"}]},
];
/* the "AI classifier" — long-tail dishes it recognizes by name */
const KNOWN = {
  "khao soi":{disp:"Khao Soi",t:"curry",say:"a Northern Thai curry noodle soup"},
  "larb gai":{disp:"Larb Gai",t:"salad",say:"a Thai minced-chicken salad"},
  "larb":{disp:"Larb",t:"salad",say:"a Thai minced-meat salad"},
  "banh mi":{disp:"Banh Mi",t:"taco",say:"a Vietnamese baguette sandwich"},
  "pho":{disp:"Pho",t:"soup",say:"a Vietnamese noodle soup"},
  "bibimbap":{disp:"Bibimbap",t:"generic",say:"a Korean rice bowl"},
  "shakshuka":{disp:"Shakshuka",t:"curry",say:"eggs poached in a spiced tomato sauce"},
  "poke bowl":{disp:"Poke Bowl",t:"sushi",say:"a Hawaiian raw-fish rice bowl"},
  "massaman curry":{disp:"Massaman Curry",t:"curry",say:"a rich Thai curry"},
  "birria tacos":{disp:"Birria Tacos",t:"taco",say:"braised-beef tacos with consommé"},
};

/* ---------------- crowd data engine (deterministic fake data) ---------------- */
function hashStr(s){let h=2166136261;for(let i=0;i<s.length;i++){h^=s.charCodeAt(i);h=Math.imul(h,16777619);}return h>>>0;}
function mulberry32(a){return function(){a|=0;a=a+0x6D2B79F5|0;let t=Math.imul(a^a>>>15,1|a);t=t+Math.imul(t^t>>>7,61|t)^t;return((t^t>>>14)>>>0)/4294967296;};}
function crowd(name,key){
  const rng=mulberry32(hashStr(name+"|"+key));
  const skew=(rng()*2-1);
  const amp=Math.pow(rng(),1.4)*2.7;          // usually small, occasionally large
  const mu=Math.min(5.7,Math.max(0.3, 3 + skew*amp)); // center of mass, bucket 0..6
  const sig=0.5+rng()*1.35;                    // some tight (consensus), some wide (divided)
  const N=45+Math.floor(rng()*520);            // number of ratings
  let b=[],tot=0;
  for(let i=0;i<7;i++){const w=Math.exp(-((i-mu)*(i-mu))/(2*sig*sig))+rng()*0.04;b.push(w);tot+=w;}
  const counts=b.map(w=>Math.max(0,Math.round(w/tot*N)));
  const cN=counts.reduce((a,c)=>a+c,0)||1;
  const leftPct=Math.round((counts[0]+counts[1]+counts[2])/cN*100);
  const rightPct=Math.round((counts[4]+counts[5]+counts[6])/cN*100);
  const midPct=Math.round(counts[3]/cN*100);
  const side= mu>3.35?'r': mu<2.65?'l':'mid';
  return {counts,N:cN,mu,muPos:mu/6*100,leftPct,rightPct,midPct,side};
}
function youSide(v){const yb=Math.round(v/100*6);return yb<3?'l':yb>3?'r':'mid';}
/* "perfect taste" score. For each scale we take the average distance of every
   rating from dead-center, normalised. Because it uses ABSOLUTE distance, a
   split crowd (half "too salty", half "needs salt") scores low — it does NOT
   cancel to a fake middle the way averaging raw positions would. */
function scaleScore(name,key){
  const c=crowd(name,key);
  const N=c.counts.reduce((a,x)=>a+x,0)||1;
  let dist=0; for(let i=0;i<7;i++) dist+=c.counts[i]*Math.abs(i-3);
  const meanDist=(dist/N)/3;           // 0 (all perfect) .. 1 (all at an extreme)
  return Math.max(0,1-meanDist);       // 1 = perfect consensus
}
function ptScore(name,keys){
  let sum=0; keys.forEach(k=>sum+=scaleScore(name,k));
  return Math.round(sum/keys.length*100);
}
function dishScore(d){ return ptScore(d.n, TYPES[d.t].keys); }

/* ---------------- restaurants + discovery ---------------- */
const RESTAURANTS = [
  {name:"Osteria Lupo",     cuisines:["ital"], area:"North End",   dist:0.4},
  {name:"Trattoria Bianca", cuisines:["ital"], area:"Midtown",     dist:1.2},
  {name:"Nonna's Table",    cuisines:["ital"], area:"Riverside",   dist:2.1},
  {name:"Bangkok Orchid",   cuisines:["thai"], area:"Chinatown",   dist:0.6},
  {name:"Thai Basil House", cuisines:["thai"], area:"Eastside",    dist:1.5},
  {name:"Chiang Mai Corner",cuisines:["thai"], area:"Uptown",      dist:2.4},
  {name:"Casa Verde",       cuisines:["mex"],  area:"Mission",     dist:0.5},
  {name:"El Farolito",      cuisines:["mex"],  area:"Downtown",    dist:1.1},
  {name:"Tacos El Sol",     cuisines:["mex"],  area:"Southside",   dist:1.9},
  {name:"The Copper Skillet",cuisines:["amer"],area:"Downtown",    dist:0.7, versatile:true},
  {name:"Grindhouse Diner", cuisines:["amer"], area:"Midtown",     dist:1.3, versatile:true},
  {name:"Habit & Co.",      cuisines:["amer"], area:"Warehouse",   dist:1.8, versatile:true},
  {name:"Ippudo Row",       cuisines:["jpn"],  area:"Little Tokyo",dist:0.9},
  {name:"Menya Jiro",       cuisines:["jpn"],  area:"Little Tokyo",dist:1.1},
  {name:"Sakura Ramen Bar", cuisines:["jpn"],  area:"Eastside",    dist:1.6},
  {name:"Saffron Grove",    cuisines:["ind"],  area:"Curry Hill",  dist:1.0},
  {name:"Curry Leaf",       cuisines:["ind"],  area:"Eastside",    dist:1.4},
  {name:"Delhi Junction",   cuisines:["ind"],  area:"Uptown",      dist:2.2},
];
const CUISINE_LABEL = {ital:"Italian",thai:"Thai",mex:"Mexican",amer:"American",jpn:"Japanese",ind:"Indian"};
const DETECTED = {name:"Verde Kitchen", cuisineId:"mex", area:"Mission", dist:0.3};
function seedFor(dishName){ return (state.restaurant?state.restaurant.name:"Verde Kitchen")+"|"+dishName; }
const ACCENTS=[["#D3F5F7","#086A72"],["#EBE0FF","#5B21B6"]];
function accentFor(i){ return ACCENTS[i%ACCENTS.length]; }
const DISH_CATALOG = {
  "carbonara":{disp:"Spaghetti Carbonara",type:"pasta",cuisine:"ital"},
  "spaghetti carbonara":{disp:"Spaghetti Carbonara",type:"pasta",cuisine:"ital"},
  "lasagna":{disp:"Lasagna",type:"pasta",cuisine:"ital"},
  "cacio e pepe":{disp:"Cacio e Pepe",type:"pasta",cuisine:"ital"},
  "margherita pizza":{disp:"Margherita Pizza",type:"pizza",cuisine:"ital"},
  "pizza":{disp:"Margherita Pizza",type:"pizza",cuisine:"ital"},
  "tiramisu":{disp:"Tiramisu",type:"dessert",cuisine:"ital"},
  "pad thai":{disp:"Pad Thai",type:"noodle",cuisine:"thai"},
  "green curry":{disp:"Green Curry",type:"curry",cuisine:"thai"},
  "pad see ew":{disp:"Pad See Ew",type:"noodle",cuisine:"thai"},
  "tom yum":{disp:"Tom Yum Soup",type:"soup",cuisine:"thai"},
  "cheeseburger":{disp:"Cheeseburger",type:"burger",cuisine:"amer"},
  "burger":{disp:"Cheeseburger",type:"burger",cuisine:"amer"},
  "caesar salad":{disp:"Caesar Salad",type:"salad",cuisine:"amer"},
  "buffalo wings":{disp:"Buffalo Wings",type:"wings",cuisine:"amer"},
  "wings":{disp:"Buffalo Wings",type:"wings",cuisine:"amer"},
  "mac and cheese":{disp:"Mac and Cheese",type:"pasta",cuisine:"amer"},
  "ramen":{disp:"Tonkotsu Ramen",type:"soup",cuisine:"jpn"},
  "tonkotsu ramen":{disp:"Tonkotsu Ramen",type:"soup",cuisine:"jpn"},
  "gyoza":{disp:"Gyoza",type:"fried",cuisine:"jpn"},
  "katsu":{disp:"Chicken Katsu",type:"fried",cuisine:"jpn"},
  "tacos":{disp:"Tacos al Pastor",type:"taco",cuisine:"mex"},
  "tacos al pastor":{disp:"Tacos al Pastor",type:"taco",cuisine:"mex"},
  "al pastor":{disp:"Tacos al Pastor",type:"taco",cuisine:"mex"},
  "burrito":{disp:"Chicken Burrito",type:"taco",cuisine:"mex"},
  "butter chicken":{disp:"Butter Chicken",type:"curry",cuisine:"ind"},
  "biryani":{disp:"Chicken Biryani",type:"generic",cuisine:"ind"},
  "samosa":{disp:"Samosa",type:"fried",cuisine:"ind"},
  "palak paneer":{disp:"Palak Paneer",type:"curry",cuisine:"ind"},
};
const KNOWN_CUISINE = {"khao soi":"thai","larb gai":"thai","larb":"thai","massaman curry":"thai","birria tacos":"mex","poke bowl":"jpn"};
function resolveDish(q){
  q=q.trim().toLowerCase();
  if(DISH_CATALOG[q]) return DISH_CATALOG[q];
  if(KNOWN[q]) return {disp:KNOWN[q].disp,type:KNOWN[q].t,cuisine:KNOWN_CUISINE[q]||null};
  for(const k in DISH_CATALOG){ if(k.includes(q)||q.includes(k)) return DISH_CATALOG[k]; }
  return {disp:q.replace(/\b\w/g,m=>m.toUpperCase()),type:"generic",cuisine:null};
}
function restaurantsFor(cuisine){
  let list = cuisine ? RESTAURANTS.filter(r=>r.cuisines.includes(cuisine)) : [];
  if(list.length<3){ RESTAURANTS.filter(r=>r.versatile&&!list.includes(r)).forEach(r=>{ if(list.length<5) list.push(r); }); }
  return list;
}
function crowdSummary(seed,keys){
  let N=0,worst=null,worstLean=-1;
  keys.forEach(k=>{const c=crowd(seed,k);N=Math.max(N,c.N);const lean=Math.abs(c.mu-3);if(c.side!=='mid'&&lean>worstLean){worstLean=lean;worst={k,c};}});
  return {N, score:ptScore(seed,keys),
    verdict: worst? 'Runs '+(worst.c.side==='r'?SLIDERS[worst.k].vr:SLIDERS[worst.k].vl):'Dialed in',
    vcolor: worst? 'var(--coral)':'var(--green)'};
}

/* ---------------- state ---------------- */
let state = {cuisine:null, dish:null, ratings:{}, sort:'menu', query:'', discover:null, restaurant:null};
const screen = document.getElementById("screen");

function go(html){
  const old = screen.querySelector(".view");
  const v = document.createElement("div");
  v.className = "view stack-hidden";
  v.innerHTML = html;
  screen.appendChild(v);
  requestAnimationFrame(()=>{ requestAnimationFrame(()=>{
    v.classList.remove("stack-hidden");
    if(old){ old.classList.add("stack-back"); setTimeout(()=>old.remove(),360); }
  });});
  return v;
}
function goBack(html){
  const old = screen.querySelector(".view");
  const v = document.createElement("div");
  v.className = "view stack-back"; v.innerHTML = html;
  screen.appendChild(v);
  requestAnimationFrame(()=>{ requestAnimationFrame(()=>{
    v.classList.remove("stack-back");
    if(old){ old.classList.add("stack-hidden"); setTimeout(()=>old.remove(),360); }
  });});
  return v;
}

/* ---------------- screen 1: cuisine ---------------- */
function homeHTML(){
  const chips = ["Carbonara","Pad Thai","Cheeseburger","Ramen","Tacos","Butter Chicken"]
    .map(d=>`<span class="chip" style="background:#8FE6EB;color:#04353A" onclick="runDiscover('${d}')">${d}</span>`).join("");
  return `
    <div class="pad" style="padding-top:8px"><div class="logo">
      <svg class="dial" viewBox="0 0 40 34" aria-hidden="true">
        <path d="M7 13 Q20 31 33 13" fill="none" stroke="#C2185B" stroke-width="4.5" stroke-linecap="round"/>
        <path d="M26 22 C34 20 34 8 28 8 C24 8 24 15 26 22 Z" fill="#C2185B"/>
      </svg>
      <span class="wm">Perfect <b>Taste</b></span>
    </div></div>
    <div class="hero">
      <div class="hl">Find the best version of any dish near you</div>
      <div class="dsearch"><span class="mag">&#9906;</span>
        <input id="discInput" placeholder="Try “carbonara” or “khao soi”…" autocomplete="off"
          onkeydown="if(event.key==='Enter'){runDiscover(this.value)}"></div>
      <div class="chips">${chips}</div>
    </div>
    <div class="orline">or — already at a restaurant?</div>
    <div class="detcard" onclick="enterDetected()">
      <span class="dot"></span>
      <div class="dinfo"><b>Rate what you're eating now</b>
        <div class="dmeta">Verde Kitchen &middot; Mexican &middot; ${DETECTED.dist} mi</div></div>
      <span class="chev">&rsaquo;</span>
    </div>
    <div class="otherlink" onclick="scrPlaces()">Not at ${DETECTED.name}? Pick another spot</div>
    <div style="height:24px"></div>`;
}
function scrCuisine(){ go(homeHTML()); }
function enterRestaurant(rest){
  const cid = rest.cuisineId || (rest.cuisines && rest.cuisines[0]);
  state.restaurant = {name:rest.name, area:rest.area, dist:rest.dist, cuisineId:cid};
  state.cuisine = CUISINES.find(c=>c.id===cid);
  scrDishes();
}
function enterDetected(){ state.menuBack='home'; enterRestaurant(DETECTED); }
function gotoRestaurant(name){
  const rest = (name===DETECTED.name) ? DETECTED : RESTAURANTS.find(r=>r.name===name);
  if(!rest) return;
  state.menuBack='browse';
  enterRestaurant(rest);
}
function scrPlaces(){
  const seen={}; const list=[DETECTED,...RESTAURANTS].filter(r=>{const k=r.name;if(seen[k])return false;seen[k]=1;return true;})
    .sort((a,b)=>a.dist-b.dist);
  state._places=list;
  go(`
    <div class="topbar"><button class="back" onclick="backHome()">&lsaquo;</button>
      <div class="kicker">Nearby</div></div>
    <div class="pad"><h1 class="t">Where are you eating?</h1>
      <p class="sub">Tap your spot — the app already knows its cuisine and menu, so there's nothing to set up.</p></div>
    <div class="dishlist" style="padding-top:6px">${list.map((r,i)=>{
      const cid=r.cuisineId||r.cuisines[0];
      return `<div class="rrow" onclick="pickPlace(${i})">
        <div class="dico" style="background:${accentFor(i)[0]};color:${accentFor(i)[1]}">${r.name[0]}</div>
        <div style="flex:1;min-width:0"><div class="rname">${r.name}</div>
        <div class="rmeta">${CUISINE_LABEL[cid]} &middot; ${r.area} &middot; ${r.dist} mi</div></div>
        <div style="color:var(--faint);font-size:20px">&rsaquo;</div>
      </div>`;}).join("")}</div>
    <div style="height:20px"></div>`);
}
function pickPlace(i){ state.menuBack='home'; enterRestaurant(state._places[i]); }

/* ---------------- discovery: best [dish] near me ---------------- */
function runDiscover(q){
  q=(q||"").trim(); if(!q) return;
  state.discover = resolveDish(q);
  scrDiscover(true);
}
function scrDiscover(fwd){
  const dd = state.discover;
  const keys = TYPES[dd.type].keys;
  const cands = restaurantsFor(dd.cuisine);
  let items = cands.map(r=>{
    const seed = r.name+"|"+dd.disp;
    return {r, seed, ...crowdSummary(seed,keys)};
  }).sort((a,b)=>b.score-a.score);
  const rows = items.length ? items.map((x,i)=>{
    const bg = x.score>=70?'var(--green-fill)':x.score>=58?'var(--amber-fill)':'var(--coral-fill)';
    const fg = x.score>=70?'var(--green-ink)':x.score>=58?'#8A5A06':'#A5291F';
    return `<div class="rrow">
      <div class="rankno">${i+1}</div>
      <div style="flex:1;min-width:0" onclick="openRestaurant(${i})">
        <div class="rname">${x.r.name} &rsaquo;</div>
        <div class="rmeta">${CUISINE_LABEL[x.r.cuisines[0]]} &middot; ${x.r.area} &middot; ${x.r.dist} mi</div>
        <div class="rverdict" style="color:${x.vcolor}">${x.verdict} &middot; ${x.N} ratings</div>
      </div>
      <div class="scorepill" style="background:${bg};color:${fg}">${x.score}</div>
      <button class="trendbtn" onclick="openDishAt(${i})">trend &rsaquo;</button>
    </div>`;
  }).join("") : `<div style="padding:26px 4px;color:var(--muted);font-size:14px">No nearby spots are logged for this yet — be the first to rate it and put it on the map.</div>`;
  state._discItems = items;
  const render = fwd ? go : goBack;
  render(`
    <div class="topbar"><button class="back" onclick="backHome()">&lsaquo;</button>
      <div class="kicker">Best near you</div></div>
    <div class="pad"><h1 class="t">${dd.disp}</h1>
      <p class="sub">${items.length} place${items.length===1?'':'s'} within 3 mi, ranked by score. Tap a restaurant's name to see all its dishes; “trend” shows this dish's detail.</p></div>
    <div class="dishlist" style="padding-top:6px">${rows}</div>
    <div style="height:20px"></div>`);
}
function scrDiscoverBack(){ scrDiscover(false); }
function backHome(){ go(homeHTML()); }
function openRestaurant(i){ state.menuBack='discovery'; enterRestaurant(state._discItems[i].r); }
function openDishAt(i){
  const x = state._discItems[i], dd = state.discover;
  state.cuisine = null;
  state.dish = {name:dd.disp, type:dd.type, seed:x.seed, place:x.r.name,
    cuisineName:CUISINE_LABEL[x.r.cuisines[0]], area:x.r.area, dist:x.r.dist, origin:'discover'};
  scrTrend({showYou:false, back:'discovery'});
}

/* ---------------- screen 2: dishes ---------------- */
function scrDishes(){
  const c = state.cuisine;
  state.query = "";
  const fromDisc = state.menuBack==='discovery';
  const showName = state.menuBack!=='home';
  const rname = state.restaurant.name;
  const rlink = `<span class="rlink" onclick="gotoRestaurant('${rname.replace(/'/g,"")}')">${rname}</span>`;
  const kicker = showName ? `${c.name} &middot; ${state.restaurant.dist} mi` : `${c.name} &middot; ${rlink}`;
  go(`
    <div class="topbar"><button class="back" onclick="${fromDisc?'scrDiscoverBack()':'scrCuisineBack()'}">&lsaquo;</button>
      <div><div class="kicker">${kicker}</div></div></div>
    <div class="pad"><h1 class="t">${showName? rname : 'What did you order?'}</h1></div>
    <div class="search"><span class="mag">&#9906;</span>
      <input id="dsearch" placeholder="Search this menu…" oninput="filterDishes(this.value)" autocomplete="off"></div>
    <div class="cutecap">
      <svg viewBox="0 0 40 34" aria-hidden="true"><path d="M7 13 Q20 31 33 13" fill="none" stroke="#C2185B" stroke-width="4.5" stroke-linecap="round"/><path d="M26 22 C34 20 34 8 28 8 C24 8 24 15 26 22 Z" fill="#C2185B"/></svg>
      Sorted by average score, based on people like you!
    </div>
    <div class="dishlist" id="dishlist">${dishRowsHTML("")}</div>
    <div class="addrow" onclick="scrManual('')">
      <div class="plus">+</div>
      <div><div class="an">Can't find it? Add it yourself</div>
      <div class="as">We'll figure out how to rate it</div></div>
    </div>
  `);
}
function dishRowsHTML(query){
  const c=state.cuisine;
  let items=c.dishes.map((d,i)=>({d,i,score:ptScore(seedFor(d.n),TYPES[d.t].keys)}));
  if(query){const q=query.toLowerCase(); items=items.filter(x=>x.d.n.toLowerCase().includes(q));}
  items.sort((a,b)=>b.score-a.score);
  if(!items.length) return `<div style="padding:22px 4px;color:var(--muted);font-size:14px">No match on this menu — <a style="color:var(--green);font-weight:600;cursor:pointer" onclick="scrManual('${(query||'').replace(/'/g,'')}')">add &ldquo;${query}&rdquo; yourself</a></div>`;
  return items.map((x)=>{
    const d=x.d, i=x.i;
    const bg = x.score>=75?'var(--green-fill)':x.score>=58?'var(--amber-fill)':'var(--coral-fill)';
    const fg = x.score>=75?'var(--green-ink)':x.score>=58?'#8A5A06':'#A5291F';
    return `<div class="drow">
      <div style="flex:1;min-width:0" onclick="pickDish(${i})"><div class="dn">${d.n}</div><div class="dm">${TYPES[d.t].label}</div></div>
      <div class="scorepill" style="background:${bg};color:${fg}">${x.score}</div>
      <button class="trendbtn" onclick="openTrend('${d.n.replace(/'/g,"")}','${d.t}')">trend &rsaquo;</button>
    </div>`;
  }).join("");
}
function scrCuisineBack(){ scrCuisineB(); }
function scrCuisineB(){ goBack(homeHTML()); }
function filterDishes(q){
  state.query=q.trim();
  document.getElementById("dishlist").innerHTML=dishRowsHTML(state.query);
}
function pickDish(i){
  const d = state.cuisine.dishes[i];
  state.dish = {name:d.n, type:d.t, seed:seedFor(d.n), place:state.restaurant.name, cuisineName:state.cuisine.name, origin:"menu"};
  scrRate();
}

/* ---------------- screen 2b: manual entry ---------------- */
function scrManual(prefill){
  goBack(`
    <div class="topbar"><button class="back" onclick="scrDishes()">&lsaquo;</button>
      <div class="kicker">${state.cuisine.name} &middot; add a dish</div></div>
    <div class="pad"><h1 class="t">What's it called?</h1>
      <p class="sub">Type the dish name — we'll work out what it is and how to rate it.</p></div>
    <div class="field"><label>Dish name</label>
      <input id="mname" placeholder="e.g. Khao Soi" value="${prefill||''}" autocomplete="off" oninput="checkSuggest(this.value)"></div>
    <div class="suggest" id="suggest"></div>
    <div class="hint">Tip: try <b>Khao Soi</b>, <b>Larb Gai</b>, <b>Banh Mi</b>, or <b>Shakshuka</b> to see the classifier in action.</div>
    <div class="pad" style="margin-top:auto;padding-bottom:20px">
      <button class="cta" onclick="classify()">Identify this dish</button></div>
  `);
  setTimeout(()=>{const el=document.getElementById("mname"); if(el&&!prefill) el.focus();},380);
}
function checkSuggest(v){
  const box=document.getElementById("suggest"); v=v.trim().toLowerCase();
  const near=state.cuisine.dishes.find(d=>v.length>2 && d.n.toLowerCase().startsWith(v.slice(0,3)) && d.n.toLowerCase()!==v);
  box.innerHTML = near
    ? `<div class="sg" onclick="pickByName('${near.n}')">&#8635;&nbsp; Did you mean <b>&nbsp;${near.n}</b>? &nbsp;It's already on the menu.</div>`
    : "";
}
function pickByName(n){
  const d=state.cuisine.dishes.find(x=>x.n===n);
  state.dish={name:d.n,type:d.t}; scrRate();
}
function classify(){
  const raw=(document.getElementById("mname").value||"").trim();
  if(!raw){ const el=document.getElementById("mname"); el.style.borderColor="var(--coral)"; el.placeholder="Type a dish name first"; return; }
  const key=raw.toLowerCase();
  const hit=KNOWN[key];
  // thinking screen
  goBack(`
    <div class="topbar"><button class="back" onclick="scrManual('${raw.replace(/'/g,'')}')">&lsaquo;</button>
      <div class="kicker">Reading the dish</div></div>
    <div class="thinking">
      <div class="pulse">PT</div>
      <div class="tt">Figuring out “${raw}”…</div>
      <div class="ts">Matching it to a taste profile</div>
      <div class="dots"><span></span><span></span><span></span></div>
    </div>`);
  setTimeout(()=>revealClassification(raw,hit),1500);
}
function revealClassification(raw,hit){
  const disp = hit? hit.disp : raw.replace(/\b\w/g,m=>m.toUpperCase());
  if(!hit){ scrCategory(disp, raw); return; }   // app unsure -> let the user tell us
  const type = hit.t, say = hit.say;
  state.dish = {name:disp, type:type, isNew:true, seed:seedFor(disp), place:state.restaurant.name, cuisineName:state.cuisine.name, origin:"manual"};
  const keys = TYPES[type].keys;
  const pills = keys.map(k=>`<span class="pill">${SLIDERS[k].name}</span>`).join("");
  goBack(`
    <div class="topbar"><button class="back" onclick="scrManual('${raw.replace(/'/g,'')}')">&lsaquo;</button>
      <div class="kicker">Identified</div></div>
    <div class="idcard">
      <div class="found">&#10003;&nbsp; Looks like ${TYPES[type].label}</div>
      <div class="dishname">${disp}</div>
      <div class="typeline">Classified as ${say}.</div>
      <div class="divider"></div>
      <div class="scalelabel">We'll rate it on these ${keys.length} scales</div>
      <div class="pills">${pills}</div>
    </div>
    <div class="selfnote"><i>&#9733;</i><div>Now that it's classified, <b>${disp}</b> joins the ${state.cuisine.name} list — the next person just taps it, no typing.</div></div>
    <div class="pad" style="margin-top:auto;padding:16px 22px 20px">
      <button class="cta" onclick="scrRate()">These look right — rate it</button>
      <button class="cta ghost" style="margin-top:8px" onclick="scrCategory('${disp.replace(/'/g,'')}','${raw.replace(/'/g,'')}')">Not the right type? Pick it</button>
    </div>`);
}
const CATEGORY_PICKER=[
  {label:"Soup or broth",type:"soup"},{label:"Curry",type:"curry"},{label:"Pasta",type:"pasta"},
  {label:"Stir-fried noodles",type:"noodle"},{label:"Salad",type:"salad"},{label:"Sandwich or wrap",type:"taco"},
  {label:"Burger",type:"burger"},{label:"Grilled meat / steak",type:"steak"},{label:"Fried food",type:"fried"},
  {label:"Wings",type:"wings"},{label:"Pizza",type:"pizza"},{label:"Sushi or raw",type:"sushi"},
  {label:"Dessert",type:"dessert"},{label:"Just the basics",type:"generic"},
];
function scrCategory(disp, raw){
  const chips=CATEGORY_PICKER.map(c=>`<div class="catchip" onclick="pickCategory('${c.type}','${disp.replace(/'/g,'')}')">${c.label}</div>`).join("");
  goBack(`
    <div class="topbar"><button class="back" onclick="scrManual('${(raw||disp).replace(/'/g,'')}')">&lsaquo;</button>
      <div class="kicker">Help us rate it right</div></div>
    <div class="pad"><h1 class="t">What kind of dish is ${disp}?</h1>
      <p class="sub">We couldn't quite place it. Pick the closest match so we use the right taste scales — like &ldquo;soup&rdquo; for Tom Yum.</p></div>
    <div class="catgrid">${chips}</div>
    <div style="height:24px"></div>`);
}
function pickCategory(type, disp){
  state.dish={name:disp, type:type, isNew:true, seed:seedFor(disp), place:state.restaurant.name, cuisineName:state.cuisine.name, origin:"manual"};
  scrRate();
}

/* ---------------- screen 3: rating ---------------- */
function verdictFor(d){ // distance from center 0..50
  if(d<=8) return {t:"on point",c:"var(--green)"};
  if(d<=22) return {t:"a touch off",c:"var(--amber)"};
  return {t:"off",c:"var(--coral)"};
}
function thumbColor(d){ return d<=8?"var(--green)":d<=22?"var(--amber)":"var(--coral)"; }
function scrRate(){
  const keys = TYPES[state.dish.type].keys;
  state.ratings = {};
  const rows = keys.map(k=>{
    const s=SLIDERS[k];
    return `<div class="srow" data-k="${k}">
      <div class="shead"><span class="sname">${s.name}</span>
        <span class="sverdict" style="color:var(--green)">on point</span></div>
      <div class="track">
        <div class="grad"></div><div class="mid"></div>
        <input type="range" min="0" max="100" step="1" value="50" style="--tc:var(--green)"
          oninput="onSlide('${k}',this)">
      </div>
      <div class="ends"><span>${s.l}</span><span class="mididx">just right</span><span>${s.r}</span></div>
    </div>`;
  }).join("");
  const place = state.dish.place || "Verde Kitchen";
  const cuisineName = state.dish.cuisineName || (state.cuisine && state.cuisine.name) || "";
  const backTo = state.dish.origin==='manual' ? "scrManual('')"
    : state.dish.origin==='discover' ? "scrTrend({showYou:false,back:'discovery'})"
    : "scrDishes()";
  go(`
    <div class="topbar"><button class="back" onclick="${backTo}">&lsaquo;</button>
      <div class="kicker">Rating &middot; <span class="rlink" onclick="gotoRestaurant('${place.replace(/'/g,"")}')">${place}</span></div></div>
    <div class="dishhead">
      <div class="place"><span class="pin"></span>${cuisineName?cuisineName+' &middot; ':''}<span class="rlink" onclick="gotoRestaurant('${place.replace(/'/g,"")}')">${place}</span></div>
      <h2>${state.dish.name}</h2>
      <p class="instr">Slide each toward the center for perfect. Your rating joins the public trend for this dish.</p>
    </div>
    <div class="sliders">${rows}</div>
    <div class="scorebar">
      <div class="scorecard">
        <div><div class="slab">Taste balance</div><div class="sval" id="scoreval">100</div></div>
        <div class="verdictpill" id="vpill" style="background:var(--green-fill);color:var(--green-ink)">Perfect taste</div>
      </div>
      <button class="cta" onclick="scrPublish()">Publish my rating</button>
    </div>`);
  keys.forEach(k=>state.ratings[k]=50);
}
function onSlide(k,el){
  const v=+el.value; state.ratings[k]=v;
  const d=Math.abs(v-50);
  const ver=verdictFor(d);
  el.style.setProperty("--tc",thumbColor(d));
  const row=el.closest(".srow");
  const vd=row.querySelector(".sverdict"); vd.textContent=ver.t; vd.style.color=ver.c;
  updateScore();
}
function updateScore(){
  const vals=Object.values(state.ratings);
  const tot=vals.reduce((a,v)=>a+Math.abs(v-50),0);
  const score=Math.round(100-(tot/(vals.length*50))*100);
  document.getElementById("scoreval").textContent=score;
  const p=document.getElementById("vpill");
  if(score>=85){p.textContent="Perfect taste";p.style.background="var(--green-fill)";p.style.color="var(--green-ink)";}
  else if(score>=60){p.textContent="Close, needs tweaks";p.style.background="var(--amber-fill)";p.style.color="#8A5A06";}
  else{p.textContent="Off balance";p.style.background="var(--coral-fill)";p.style.color="#A5291F";}
}

/* ---------------- screen 4: publish + community compare ---------------- */
function scrPublish(){
  const keys=TYPES[state.dish.type].keys;
  const SEED=state.dish.seed||state.dish.name;
  // your score
  const yvals=keys.map(k=>state.ratings[k]);
  const yscore=Math.round(100-(yvals.reduce((a,v)=>a+Math.abs(v-50),0)/(yvals.length*50))*100);
  const rows=keys.map(k=>{
    const s=SLIDERS[k], c=crowd(SEED,k), v=state.ratings[k];
    const ys=youSide(v);
    const yourTxt= ys==='mid'?'just right':(ys==='r'?s.r.toLowerCase():s.l.toLowerCase());
    const crowdTxt= c.side==='mid'?'call it dialed in':'lean '+(c.side==='r'?s.vr:s.vl);
    const crowdPct= c.side==='mid'?c.midPct:(c.side==='r'?c.rightPct:c.leftPct);
    const agree= ys===c.side?'<span class="agchip ag">you agree</span>':'<span class="agchip out">minority view</span>';
    const d=Math.abs(v-50); const tc=d<=8?'var(--green)':d<=22?'var(--amber)':'var(--coral)';
    return `<div class="cmprow">
      <div class="cn"><span class="nm">${s.name}</span>${agree}</div>
      <div class="cbarwrap"><div class="cbar"></div>
        <div class="cmed" style="left:${c.muPos.toFixed(0)}%"></div>
        <div class="cyou" style="left:${v}%;--tc:${tc}"></div></div>
      <div class="ccap">You: <b>${yourTxt}</b> &middot; ${crowdPct}% of ${c.N} diners ${crowdTxt}</div>
    </div>`;
  }).join("");
  go(`
    <div class="pubhead">
      <div class="check">&#10003;</div>
      <h2>Rating published</h2>
      <p>It's live on the public trend for ${state.dish.name}, and saved to your log. Here's how your take compares.</p>
    </div>
    <div class="legendrow">
      <i><span class="lgmed"></span> where the crowd centers</i>
      <i><span class="lgyou"></span> you</i>
    </div>
    <div class="cmplist">${rows}</div>
    <div class="pad" style="padding:16px 22px 22px">
      <button class="cta" onclick="scrTrend({showYou:true,back:'scrPublish'})">See the full trend for this dish</button>
      <button class="cta ghost" style="margin-top:8px" onclick="restart()">Rate another dish</button>
    </div>`);
}

/* ---------------- screen 5: public dish trend ---------------- */
function renderDist(name,key,showYou){
  const s=SLIDERS[key], c=crowd(name,key);
  const max=Math.max(...c.counts,1);
  const bars=c.counts.map((n,i)=>{
    const h=Math.round(6+ n/max*30);
    const d=Math.abs(i-3);
    const col=d===0?'var(--green)':d===1?'#5FAE3A':d===2?'var(--amber)':'var(--coral)';
    return `<div class="hb" style="height:${h}px;background:${col}"></div>`;
  }).join("");
  let youMark="";
  if(showYou && state.ratings[key]!=null){
    const yb=Math.round(state.ratings[key]/100*6);
    const left=((yb+0.5)/7*100);
    youMark=`<div class="youpin" style="left:${left.toFixed(1)}%"><span>you</span></div>`;
  }
  const word= c.side==='mid'?'Dialed in':'Runs '+(c.side==='r'?s.vr:s.vl);
  const wcol= c.side==='mid'?'var(--green)':'var(--coral)';
  const cap= c.side==='mid'
      ? `${c.midPct}% call it just right`
      : `${c.side==='r'?c.rightPct:c.leftPct}% say &ldquo;${c.side==='r'?s.r:s.l}&rdquo;`;
  let agree="";
  if(showYou && state.ratings[key]!=null){
    agree = youSide(state.ratings[key])===c.side
      ? ` &middot; <span class="agchip ag">you agree</span>`
      : ` &middot; <span class="agchip out">you're an outlier</span>`;
  }
  return `<div class="dscale">
    <div class="dhead"><span class="dname">${s.name}</span><span class="dverdict" style="color:${wcol}">${word}</span></div>
    <div class="histo">${bars}${youMark}</div>
    <div class="dends"><span>${s.l}</span><span>${s.r}</span></div>
    <div class="dcap">${cap}${agree}</div>
  </div>`;
}
function scrTrend(opts){
  opts=opts||{}; const showYou=!!opts.showYou; const back=opts.back||'scrDishes';
  const d=state.dish, keys=TYPES[d.type].keys;
  const SEED=d.seed||d.name;
  const place=d.place||"Verde Kitchen";
  const cuisineName=d.cuisineName||(state.cuisine&&state.cuisine.name)||"";
  let N=0,worst=null,worstLean=-1;
  keys.forEach(k=>{
    const c=crowd(SEED,k); N=Math.max(N,c.N);
    const lean=Math.abs(c.mu-3);
    if(c.side!=='mid'&&lean>worstLean){worstLean=lean;worst={k,c};}
  });
  const bal=ptScore(SEED,keys);
  const headline= worst
    ? `Well-liked overall, but the crowd says it runs <b>${worst.c.side==='r'?SLIDERS[worst.k].vr:SLIDERS[worst.k].vl}</b>.`
    : `Remarkably dialed in — no strong complaints across the board.`;
  const dists=keys.map(k=>renderDist(SEED,k,showYou)).join("");
  const backCall= back==='scrPublish'?'scrPublish()': back==='discovery'?'scrDiscoverBack()':'scrDishes()';
  const footer= showYou
    ? `<button class="cta ghost" onclick="restart()">Rate another dish</button>`
    : `<button class="cta" onclick="scrRate()">Rate this dish yourself</button>`;
  go(`
    <div class="topbar"><button class="back" onclick="${backCall}">&lsaquo;</button>
      <div class="kicker">Public dish trend</div></div>
    <div class="trendcard">
      <div class="tk">&#9679; Live &middot; updates with every rating</div>
      <div class="tdn">${d.name}</div>
      <div class="tpl">${cuisineName?cuisineName+' &middot; ':''}<span class="rlink" onclick="gotoRestaurant('${place.replace(/'/g,"")}')">${place}</span>${d.dist?' &middot; '+d.dist+' mi':''}</div>
      <div class="tstats">
        <div class="tstat"><div class="sv">${N.toLocaleString()}</div><div class="sl">ratings</div></div>
        <div class="tstat"><div class="sv">${bal}</div><div class="sl">average score</div></div>
      </div>
      <div class="thl">${headline}</div>
    </div>
    <div class="disttip">Each bar shows how many diners landed there &mdash; no averages, because &ldquo;too salty&rdquo; and &ldquo;needs salt&rdquo; would cancel to a meaningless middle.</div>
    <div class="dists">${dists}</div>
    <div class="pad" style="padding:16px 22px 24px">${footer}</div>`);
}
function openTrend(name,type){
  state.dish={name:name,type:type,seed:seedFor(name),place:state.restaurant.name,cuisineName:state.cuisine.name,origin:"menu"};
  scrTrend({showYou:false,back:'scrDishes'});
}

function restart(){ state={cuisine:null,dish:null,ratings:{},sort:'menu',query:'',discover:null,restaurant:null}; backHome(); }

/* boot */
scrCuisine();
</script>
</body>
</html>
