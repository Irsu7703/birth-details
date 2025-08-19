<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Birth Registration Details</title>
<style>
  :root{
    --brand:#0b5cab;
    --text:#222;
    --muted:#666;
    --line:#e4e4e4;
    --card:#ffffff;
    --bg:#f7f7f7;
  }
  *{box-sizing:border-box}
  body{
    margin:0;
    font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
    background: var(--bg);
    color: var(--text);
  }

  /* Top tricolor ribbon */
  .ribbon{
    height:6px; display:flex;
  }
  .ribbon span{flex:1}
  .ribbon .saffron{background:#ff9933}
  .ribbon .white{background:#ffffff}
  .ribbon .green{background:#138808}

  /* Header */
  .header{
    background:#fff;
    border-bottom:1px solid var(--line);
    padding:14px 18px;
  }
  .hdr-wrap{
    max-width:980px; margin:0 auto; display:flex; align-items:center; gap:14px;
  }
  .logo{
    width:44px; height:44px; border-radius:50%;
    display:grid; place-items:center; font-weight:700; color:#fff; background:var(--brand);
    box-shadow:0 1px 2px rgba(0,0,0,.1);
    font-size:11px; text-align:center; line-height:1.05;
  }
  .gov{
    flex:1;
  }
  .gov h1{
    font-size:18px; margin:0; color:var(--brand); letter-spacing:.2px;
  }
  .gov p{
    margin:2px 0 0; font-size:12px; color:var(--muted);
  }

  /* Page wrap with watermark */
  .wrap{
    position:relative; min-height:calc(100vh - 120px);
    padding:28px 12px;
    overflow:hidden;
  }
  .watermark{
    position:absolute; inset:0; pointer-events:none;
    background:
      repeating-linear-gradient( -35deg,
        rgba(11,92,171,.08) 0 180px,
        rgba(0,0,0,0) 180px 360px);
    mask: radial-gradient(400px 400px at 50% 30%, rgba(0,0,0,.25), transparent 70%);
  }
  .wm-text{
    position:absolute; inset:0; display:grid; place-items:center; pointer-events:none;
    font-weight:800; font-size:64px; letter-spacing:2px; color:rgba(11,92,171,.06);
    transform:rotate(-18deg);
    text-transform:uppercase;
  }

  /* Card */
  .container{max-width:980px; margin:0 auto; position:relative}
  .title{
    text-align:center; font-size:24px; font-weight:700; margin:0 0 18px; color:#333;
  }
  .card{
    background:var(--card);
    border:1px solid var(--line);
    border-radius:10px;
    box-shadow:0 6px 28px rgba(0,0,0,.06);
    overflow:hidden;
  }
  table{width:100%; border-collapse:collapse;}
  td{
    padding:12px 14px; vertical-align:top; border-bottom:1px solid var(--line);
    font-size:15px;
  }
  tr:last-child td{border-bottom:0}
  td.key{
    width:38%; font-weight:700; background:#f4f5f7; color:#333;
  }
  td.val{color:#111}
  .muted{color:var(--muted)}
  .footer{
    max-width:980px; margin:22px auto 34px; color:var(--muted); font-size:12px; text-align:center;
  }

  /* Mobile */
  @media (max-width:640px){
    .title{font-size:20px}
    td{padding:10px 12px; font-size:14px}
    td.key{width:45%}
    .wm-text{font-size:42px}
  }
</style>
</head>
<body>

<div class="ribbon"><span class="saffron"></span><span class="white"></span><span class="green"></span></div>

<header class="header">
  <div class="hdr-wrap">
    <div class="logo">GOI</div>
    <div class="gov">
      <h1>Office of Civil Registration</h1>
      <p>Government Services Portal (Preview)</p>
    </div>
    <div class="logo">MCD</div>
  </div>
</header>

<main class="wrap">
  <div class="watermark"></div>
  <div class="wm-text">dc.crsorgi.gov.in</div>

  <div class="container">
    <h2 class="title">Birth Registration Details</h2>

    <div class="card">
      <table aria-label="Birth Registration Details">
        <tr><td class="key">Registration Number</td><td class="val">20252755661008010368</td></tr>
        <tr><td class="key">NAME</td><td class="val">MITHLESH MANJHI</td></tr>
        <tr><td class="key">GENDER</td><td class="val">Male</td></tr>
        <tr><td class="key">DOB</td><td class="val">05-11-2007</td></tr>
        <tr><td class="key">Name Of Mother</td><td class="val">SAVITA DEVI</td></tr>
        <tr><td class="key">Name Of Father</td><td class="val">RAJESH MANJHI</td></tr>
        <tr><td class="key">Place of Birth</td><td class="val">SAWLESHWAR, KANDHAR, NANDED, MAHARASHTRA, 401718</td></tr>
        <tr><td class="key">Registration Date</td><td class="val">30-12-2023</td></tr>
        <tr><td class="key">Registration Unit Name</td><td class="val">GRAMA PANCHAYAT SAWALESHWAR</td></tr>
        <tr><td class="key">Registration Unit Code</td><td class="val">20362</td></tr>
      </table>
    </div>

    <p class="muted" style="margin-top:10px;text-align:center;">
      This is a replica layout for demonstration.
    </p>
  </div>
</main>

<footer class="footer">
  © Government Services • For verification visit <strong>dc.crsorgi.gov.in</strong>
</footer>
</body>
</html>
