
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>魔法冒险服务器 | 我的世界网易版</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: "Microsoft YaHei", sans-serif;
      color: #fff;
      text-align: center;
      overflow-x: hidden;
    }
    body::before {
      content: "";
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: url('content://bin.mt.plus.fp/storage/emulated/0/Pictures/file_00000000e0347207b525133b2eba89b8%20(2).png') center/cover no-repeat;
      z-index: -2;
      filter: brightness(0.6);
      animation: moveBg 40s linear infinite;
    }
    @keyframes moveBg {
      0% { background-position: 0 0; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0 0; }
    }
    body::after {
      content: "";
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0, 0, 0, 0.45);
      z-index: -1;
    }
    header {
      background: rgba(0, 0, 0, 0.5);
      padding: 25px 0;
      font-size: 28px;
      letter-spacing: 2px;
      font-weight: bold;
      text-shadow: 2px 2px 5px black;
    }
    main { padding: 50px 20px; }
    .server-info {
      background: rgba(255, 255, 255, 0.15);
      border-radius: 15px;
      padding: 30px;
      max-width: 720px;
      margin: 0 auto 50px;
      backdrop-filter: blur(5px);
      box-shadow: 0 5px 25px rgba(0, 0, 0, 0.4);
      animation: float 3s ease-in-out infinite;
    }
    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
    }
    h2 {
      color: #ffeb3b;
      text-shadow: 2px 2px 6px #000;
      margin-bottom: 20px;
    }
    p {
      line-height: 1.8;
      font-size: 17px;
      color: #f5f5f5;
      text-shadow: 1px 1px 3px #000;
    }
    .btn {
      display: inline-block;
      background: linear-gradient(90deg, #00c6ff, #0072ff);
      color: #fff;
      font-size: 20px;
      font-weight: bold;
      padding: 15px 40px;
      border-radius: 12px;
      text-decoration: none;
      margin-top: 25px;
      box-shadow: 0 0 20px #00c6ff;
      transition: 0.3s;
    }
    .btn:hover {
      box-shadow: 0 0 35px #00c6ff, 0 0 50px #0072ff;
      transform: scale(1.08);
    }
    footer {
      margin-top: 60px;
      color: #eee;
      background: rgba(0, 0, 0, 0.5);
      padding: 15px 0;
      font-size: 14px;
    }
    /* 弹窗样式 */
    .modal {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0,0,0,0.6);
      justify-content: center;
      align-items: center;
      z-index: 10;
    }
    .modal-content {
      background: #222;
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 0 25px rgba(0,0,0,0.5);
      max-width: 300px;
      text-align: center;
    }
    .modal-content img {
      width: 250px;
      border-radius: 10px;
      margin-bottom: 15px;
    }
    .close {
      background: #ff4444;
      color: white;
      border: none;
      border-radius: 10px;
      padding: 8px 20px;
      cursor: pointer;
      font-size: 16px;
    }
    .close:hover { background: #dd2222; }
  </style>
</head>
<body>
  <header>
    ⚔️ 魔法冒险服务器 | 我的世界网易版 ⚔️
  </header>

  <main>
    <div class="server-info">
      <h2>✨ 欢迎加入魔法冒险 ✨</h2>
      <p>这里充满魔法与冒险的奇幻大陆！<br>
      挑战副本、探索遗迹、创造属于你的冒险故事！</p>
      <p><b>服务器号：</b>668352250<br>
      <b>版本：</b>我的世界网易版（最新）</p>

      <a class="btn" href="https://qm.qq.com/q/CfJyFn5c9U" target="_blank">💬 一键申请加入交流群</a><br>
      <a class="btn" href="javascript:void(0)" onclick="openModal()">💖 赞助腐竹</a>
    </div>
  </main>

  <!-- 弹窗 -->
  <div id="sponsorModal" class="modal">
    <div class="modal-content">
      <h3>一分一毛都是对我的支持！感谢大家！</h3>
      <img src="content://bin.mt.plus.fp/storage/emulated/0/my_website/weixin_qr.png" alt="微信赞助二维码">
      <button class="close" onclick="closeModal()">关闭</button>
    </div>
  </div>

  <footer>
    © 2025 魔法冒险服务器 | 玩家共创服务器
  </footer>

  <script>
    function openModal() {
      document.getElementById('sponsorModal').style.display = 'flex';
    }
    function closeModal() {
      document.getElementById('sponsorModal').style.display = 'none';
    }
  </script>
</body>
</html>
