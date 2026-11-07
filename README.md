# Sorry-babu-
<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <title>For Teena Ji ❤️</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      background: #0f111a;
      color: #fff;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 20px 15px;
    }
    .wrapper {
      max-width: 550px;
      width: 100%;
      background: #171b26;
      border: 2px solid #e0a96d;
      border-radius: 20px;
      padding: 30px 20px;
      text-align: center;
      box-shadow: 0 10px 40px rgba(0,0,0,0.8);
    }
    h1 {
      font-size: 26px;
      color: #e0a96d;
      margin-bottom: 10px;
    }
    p {
      color: #a4abb9;
      font-size: 15px;
      line-height: 1.6;
      margin-bottom: 20px;
    }

    /* 3D Gift Box */
    .gift-box-area {
      width: 140px;
      height: 130px;
      margin: 20px auto 30px;
      position: relative;
      cursor: pointer;
    }
    .box-lid {
      width: 150px;
      height: 32px;
      background: #e75480;
      border-radius: 6px;
      position: absolute;
      top: 0;
      left: -5px;
      z-index: 2;
      border: 2px solid #fff;
      transition: all 0.5s ease;
    }
    .box-lid::before {
      content: "🎀";
      position: absolute;
      top: -24px;
      left: 55px;
      font-size: 28px;
    }
    .box-body {
      width: 140px;
      height: 95px;
      background: #ad2850;
      border-radius: 0 0 10px 10px;
      position: absolute;
      bottom: 0;
      left: 0;
      border: 2px solid #fff;
    }
    .box-ribbon {
      width: 25px;
      height: 100%;
      background: #e0a96d;
      margin: 0 auto;
    }

    /* Button */
    .btn-open {
      background: #e0a96d;
      color: #0f111a;
      border: none;
      padding: 14px 30px;
      font-size: 16px;
      font-weight: bold;
      border-radius: 50px;
      cursor: pointer;
      box-shadow: 0 5px 15px rgba(224, 169, 109, 0.4);
      margin-bottom: 15px;
    }
    .btn-open:active {
      transform: scale(0.95);
    }

    /* Secret Gifts Screen (Hidden by default) */
    #gift-content {
      display: none;
      text-align: left;
      margin-top: 10px;
    }
    .gift-item {
      background: #202636;
      border: 1px solid rgba(224, 169, 109, 0.3);
      padding: 16px;
      border-radius: 12px;
      margin-bottom: 14px;
    }
    .gift-item h3 {
      font-size: 17px;
      color: #e0a96d;
      margin-bottom: 6px;
    }
    .gift-item p {
      color: #cbd5e1;
      font-size: 14px;
      margin-bottom: 0;
    }

    /* Gussa Meter */
    .meter-box {
      background: #202636;
      padding: 15px;
      border-radius: 12px;
      margin-top: 20px;
      border: 1px dashed #e0a96d;
    }
    .meter-box input {
      width: 100%;
      margin: 12px 0;
    }
    #meter-text {
      color: #f28b9f;
      font-weight: bold;
      font-size: 15px;
      text-align: center;
    }
  </style>
</head>
<body>

  <div class="wrapper">
    
    <!-- Stage 1: Closed Gift Box -->
    <div id="closed-screen">
      <h1>Teena Ji, Meri Jaan ❤️</h1>
      <p>Maine chaar baar aapka dil dukhaya aur aapko second priority feel karwaya. Mere paas koi excuse nahi hai. Bas ek choti si sincere koshish hai aapko manane ki.</p>
      
      <div class="gift-box-area" onclick="openBoxNow()">
        <div class="box-lid" id="lid">
          <div class="box-ribbon" style="height: 32px;"></div>
        </div>
        <div class="box-body">
          <div class="box-ribbon"></div>
        </div>
      </div>

      <button class="btn-open" onclick="openBoxNow()">OPEN YOUR GIFT 🎁</button>
      <br>
      <small style="color: #667085;">(Box ya button par tap karein)</small>
    </div>

    <!-- Stage 2: Revealed Gifts -->
    <div id="gift-content">
      <h2 style="color: #fff; font-size: 22px; margin-bottom: 15px; text-align: center;">Dil Se Sorry, Teena Ji 🥺</h2>

      <!-- Gift 1: Teddy -->
      <div class="gift-item">
        <h3>🧸 1. A Warm Virtual Hug</h3>
        <p>"Agar main aapke paas hota, toh bas chupchaap aapko gale laga leta jab tak aapke aansu tham na jaate."</p>
      </div>

      <!-- Gift 2: Real Apology Letter -->
      <div class="gift-item">
        <h3>💌 2. My Honest Apology</h3>
        <p>"Aap meri partner hain. Aapko meri life mein apni priority prove karne ke liye ladna nahi padna chahiye. 4 baar same galti karna meri bahut badi na-samjhi thi. Main aage se apne actions se dikhaunga ki aap mere liye sabse pehle hain."</p>
      </div>

      <!-- Gift 3: Lifetime Coupon -->
      <div class="gift-item">
        <h3>🎟️ 3. Royal Peace Pass</h3>
        <p>"Unlimited pyaar, zero argument, aur har call/message par 100% pehla haq Teena ji ka. No expiry date!"</p>
      </div>

      <!-- Gussa Meter -->
      <div class="meter-box">
        <div style="display: flex; justify-content: space-between; font-weight: bold;">
          <span>Aapka Gussa:</span>
          <span id="meter-val" style="color: #e0a96d;">100%</span>
        </div>
        <input type="range" min="0" max="100" value="100" oninput="updateGussa(this.value)">
        <div id="meter-text">"Aapka 100% naraz hona bilkul sahi hai. Main wait karunga jab tak aap theek na hon."</div>
      </div>

      <p style="text-align: center; margin-top: 25px; color: #a4abb9; font-size: 13px;">
        Take all your time. Main yahin hoon aur hamesha rahunga ❤️
      </p>
    </div>

  </div>

  <script>
    function openBoxNow() {
      // 1. Animate Lid
      document.getElementById("lid").style.transform = "translateY(-40px) rotate(-15deg)";
      
      // 2. Switch Screen
      setTimeout(function() {
        document.getElementById("closed-screen").style.display = "none";
        document.getElementById("gift-content").style.display = "block";
      }, 400);
    }

    function updateGussa(val) {
      document.getElementById("meter-val").innerText = val + "%";
      var t = document.getElementById("meter-text");
      if (val > 70) {
        t.innerText = '"Aapka naraz hona bilkul haqeeqat hai... take your time."';
      } else if (val > 30) {
        t.innerText = '"Gussa thoda kam hua... I am truly sorry, meri jaan."';
      } else if (val > 0) {
        t.innerText = '"Aapki ek smile mere liye poori duniya hai ❤️"';
      } else {
        t.innerText = '"0% gussa! Ab please mujhe ek baar call kar lijiye 🥺"';
      }
    }
  </script>

</body>
</html>
