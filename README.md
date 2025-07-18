<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Cổng thanh toán by HtechLab Media</title>
  <style>
    :root {
      --bg-color: #1e293b;
      --text-color: white;
      --note-bg: #334155;
    }

    body.light {
      --bg-color: #f1f5f9;
      --text-color: #0f172a;
      --note-bg: #e2e8f0;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      color: var(--text-color);
      transition: all 0.3s ease;
    }
    .container {
      background: var(--bg-color);
      border-radius: 20px;
      padding: 2rem;
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
      display: flex;
      gap: 2rem;
      align-items: center;
      flex-wrap: wrap;
    }
    .qr-image {
      width: 250px;
      height: 250px;
      border-radius: 16px;
      border: 4px solid #38bdf8;
    }
    .title {
      font-size: 1.8rem;
      font-weight: bold;
      margin-bottom: 1rem;
    }
    .note {
      font-size: 1rem;
      background-color: var(--note-bg);
      padding: 1rem;
      border-radius: 12px;
      border-left: 5px solid #38bdf8;
      box-shadow: 0 0 10px rgba(56, 189, 248, 0.4);
      margin-bottom: 1rem;
    }
    .copy-btn, .theme-btn, .zalo-btn {
      margin-top: 0.5rem;
      padding: 0.5rem 1rem;
      background-color: #38bdf8;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
      margin-right: 0.5rem;
    }
    .zalo-btn {
      background-color: #0068ff;
    }
  </style>
</head>
<body>
  <div class="container">
    <img
      src="https://i.ibb.co/q3rYznj8/blob.jpg"
      alt="QR Code"
      class="qr-image"
    />
    <div>
      <div class="title">Cổng thanh toán by HtechLab Media</div>
      <div class="note">
        💬 <strong>Lưu ý:</strong> Sau khi chuyển tiền xong, vui lòng liên hệ admin để xác nhận.
      </div>
      <button class="copy-btn" onclick="copyText()">📋 Sao chép nội dung chuyển khoản</button>
      <button class="theme-btn" onclick="toggleTheme()">🌓 Chuyển chế độ sáng/tối</button>
      <a href="https://zalo.me/0973550349" target="_blank">
        <button class="zalo-btn">💬 Liên hệ qua Zalo</button>
      </a>
    </div>
  </div>

  <script>
    function copyText() {
      const text = "Nguyen Van A - 0123456789 - Cổng HtechLab"; // nội dung mẫu
      navigator.clipboard.writeText(text);
      alert("✔️ Đã sao chép nội dung chuyển khoản!");
    }

    function toggleTheme() {
      document.body.classList.toggle('light');
    }
  </script>
</body>
</html>
