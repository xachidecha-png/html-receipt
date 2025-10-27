<!doctype html>
<html lang="th">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>ตัวอย่างสลิปการโอนเงิน (ข้อมูลสมมติ)</title>
<style>
  :root{ --bg:#f6f7fb; --card:#ffffff; --muted:#6b6f76; --accent:#ff6f00;}
  body{font-family: "Helvetica Neue", Arial, sans-serif; background:var(--bg); margin:0; padding:24px; display:flex; justify-content:center;}
  .receipt{width:720px; max-width:96%; background:var(--card); border-radius:12px; box-shadow:0 6px 20px rgba(20,20,40,0.08); padding:26px;}
  .brand{display:flex; align-items:center; gap:12px;}
  .logo{width:56px; height:56px; border-radius:10px; background:linear-gradient(135deg,#ffd59e,#ff8a00); display:flex; align-items:center; justify-content:center; color:#fff; font-weight:700; font-size:18px;}
  .brand h1{margin:0; font-size:20px; color:#222;}
  .amount{margin-top:18px; text-align:center;}
  .amount .b{font-size:44px; font-weight:700; color:#222;}
  .amount .txt{font-size:14px; color:var(--muted); margin-top:4px;}
  .info{display:flex; gap:18px; margin-top:22px;}
  .col{flex:1; background:linear-gradient(180deg, rgba(250,250,252,1), rgba(244,246,249,1)); padding:14px; border-radius:8px;}
  .row{display:flex; justify-content:space-between; align-items:center; margin:6px 0; border-bottom:1px dashed rgba(0,0,0,0.04); padding-bottom:8px;}
  .label{color:var(--muted); font-size:13px;}
  .value{color:#111; font-weight:600; font-size:14px;}
  .small{font-size:12px; color:var(--muted);}
  .qr{width:92px; height:92px; background:#eee; display:inline-block; border-radius:6px;}
  .footer{margin-top:16px; display:flex; justify-content:space-between; align-items:center;}
  .tid{font-size:12px; color:var(--muted);}
  .location{font-size:13px; color:var(--muted);}
  .note{margin-top:12px; font-size:13px; color:var(--muted);}
</style>
</head>
<body>
  <div class="receipt" role="document" aria-label="ตัวอย่างสลิปการโอนเงิน ข้อมูลสมมติ">
    <div class="brand">
      <div class="logo">ตัวอย่าง</div>
      <div>
        <h1>ตัวอย่างสลิปการโอนเงิน (ข้อมูลสมมติ)</h1>
        <div class="small">สำหรับการออกแบบ / การสอน — ไม่ใช่เอกสารจริง</div>
      </div>
    </div>

    <div class="amount" aria-hidden="false">
      <div class="b">฿ 100.00</div>
      <div class="txt">ยอดชำระ (ตัวอย่าง)</div>
    </div>

    <div class="info" style="margin-top:20px;">
      <div class="col">
        <div class="row">
          <div>
            <div class="label">ผู้ส่ง</div>
            <div class="value">อานนท์ ดาว****</div>
            <div class="small">บัญชีทรูมันนี่ 09*-***-4823</div>
          </div>
        </div>

        <div class="row">
          <div>
            <div class="label">ผู้รับ</div>
            <div class="value">เบญจมินทร์ ตริกตรอง</div>
            <div class="small">บัญชีทรูมันนี่ 09*-***-4161</div>
          </div>
        </div>

        <div class="row" style="border-bottom:none;">
          <div>
            <div class="label">วันที่ทำรายการ</div>
            <div class="value">27 ต.ค. 2568 19:50:57</div>
          </div>
        </div>
      </div>

      <div style="width:200px; display:flex; flex-direction:column; justify-content:space-between; align-items:flex-end;">
        <div style="text-align:right;">
          <div class="label">หมายเลขรายการ</div>
          <div class="value tid">50047186561037</div>
        </div>

        <div style="text-align:right; margin-top:10px;">
          <div class="label">สถานที่</div>
          <div class="small location">Chang Wat Nakhon Si Thammarat, ประเทศไทย</div>
        </div>

        <div style="margin-top:12px;">
          <div class="qr" aria-hidden="true"></div>
        </div>
      </div>
    </div>

    <div class="note">
      สแกนคิวอาร์โค้ดนี้ด้วยแอปที่รองรับเพื่อตรวจสอบรายการ (คิวอาร์โค้ดตัวอย่าง — ข้อมูลสมมติ)
    </div>
  </div>
</body>
</html>
