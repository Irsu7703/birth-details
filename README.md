<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Birth Certificate Demo</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f8f9fa;
      margin: 0;
      padding: 0;
    }
    .header {
      background: #005baa;
      color: white;
      padding: 15px;
      text-align: center;
      font-size: 20px;
      font-weight: bold;
    }
    .container {
      width: 70%;
      margin: 20px auto;
      background: white;
      padding: 20px;
      border: 2px solid #ddd;
      box-shadow: 0px 0px 10px rgba(0,0,0,0.2);
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 15px;
    }
    table, th, td {
      border: 1px solid #444;
    }
    th, td {
      padding: 10px;
      text-align: left;
    }
    .qr {
      text-align: center;
      margin-top: 20px;
    }
    .qr img {
      width: 120px;
      height: 120px;
    }
  </style>
</head>
<body>
  <div class="header">
    Government of India - Birth Certificate (Demo)
  </div>

  <div class="container">
    <h3 style="text-align:center;">Birth Certificate</h3>
    <table>
      <tr>
        <th>Registration Number</th>
        <td>20252755661008010368</td>
      </tr>
      <tr>
        <th>Name</th>
        <td>MITHLESH MANJHI</td>
      </tr>
      <tr>
        <th>Gender</th>
        <td>Male</td>
      </tr>
      <tr>
        <th>Date of Birth</th>
        <td>05-11-2007</td>
      </tr>
      <tr>
        <th>Mother's Name</th>
        <td>SAVITA</td>
      </tr>
      <tr>
        <th>Verified URL</th>
        <td><a href="https://dc.crsorgi.gov.in" target="_blank">https://dc.crsorgi.gov.in</a></td>
      </tr>
    </table>

    <div class="qr">
      <p>Scan QR to Verify</p>
      <img src="https://api.qrserver.com/v1/create-qr-code/?data=https://dc.crsorgi.gov.in&size=120x120" alt="QR Code">
    </div>
  </div>
</body>
</html>
