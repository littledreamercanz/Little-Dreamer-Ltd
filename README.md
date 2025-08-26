<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Little Dreamer Limited - Chartered Accountants</title>
  <link rel="stylesheet" href="assets/style.css">
</head>
<body>
  <!-- Header -->
  <header class="header">
    <img src="assets/logo.png" alt="Company Logo" class="logo">
    <h1>Little Dreamer Limited</h1>
    <p>New Zealand & Australia Chartered Accountants | CPA | Tax Agents</p>
    <button id="lang-toggle">中文 / English</button>
  </header>

  <!-- About -->
  <section class="about">
    <h2>About Us</h2>
    <p id="about-text">We are Chartered Accountants and Tax Agents in New Zealand & Australia, providing professional accounting, tax, and business advisory services for individuals and SMEs.</p>
  </section>

  <!-- Services -->
  <section class="services">
    <h2>Our Services</h2>
    <ul>
      <li>GST Return Filing</li>
      <li>Income Tax & PAYE</li>
      <li>Company Formation & Maintenance</li>
      <li>Trust Annual Return</li>
      <li>Rental Property Tax</li>
      <li>Business Advisory</li>
    </ul>
  </section>

  <!-- Pricing -->
  <section class="pricing">
    <h2>Pricing</h2>
    <table>
      <tr><th>Service</th><th>Price (NZD)</th></tr>
      <tr><td>GST Return Filing</td><td>From $150</td></tr>
      <tr><td>Company Annual Return</td><td>$300</td></tr>
      <tr><td>Individual Tax Return</td><td>From $200</td></tr>
      <tr><td>Business Advisory</td><td>$150 / hr</td></tr>
    </table>
  </section>

  <!-- Testimonials -->
  <section class="testimonials">
    <h2>What Our Clients Say</h2>
    <blockquote>“Harry is very professional and always provides clear financial advice.”</blockquote>
    <blockquote>“Reliable, efficient, and highly recommended for SMEs.”</blockquote>
  </section>

  <!-- FAQ -->
  <section class="faq">
    <h2>FAQ</h2>
    <p><strong>Q:</strong> Do you provide services online?<br><strong>A:</strong> Yes, we support remote services across New Zealand and Australia.</p>
    <p><strong>Q:</strong> Do you handle property investment tax?<br><strong>A:</strong> Yes, we specialize in rental property and trust taxation.</p>
  </section>

  <!-- Contact -->
  <section class="contact">
    <h2>Contact Us</h2>
    <p>Email: info@littledreamer.co.nz</p>
    <p>Phone: 0210308628</p>
    <p>WeChat: harrylemon</p>
    <img src="assets/wechat-qr.png" alt="WeChat QR Code" class="qr">
    <button onclick="window.open('https://calendar.google.com','_blank')">Book a Meeting</button>
  </section>

  <footer>
    <p>© 2025 Little Dreamer Limited. All Rights Reserved.</p>
  </footer>

  <script src="assets/script.js"></script>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Little Dreamer Limited - Chartered Accountants</title>
  <style>
    /* === 全局样式 === */
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      color: #2c3e50; /* 深蓝色文字，更专业 */
      margin: 0;
      padding: 0;
      /* 添加优雅的背景 */
      background: linear-gradient(rgba(248, 249, 250, 0.9), rgba(248, 249, 250, 0.9)), 
                  url('/images/background.jpg') no-repeat center center fixed;
      background-size: cover;
    }

    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px;
    }

    /* === 页头样式 - 已添加Logo === */
    .header {
      text-align: center;
      padding: 3rem 2rem;
      background: rgba(255, 255, 255, 0.95); /* 半透明白色背景 */
      border-radius: 15px;
      margin-bottom: 2.5rem;
      box-shadow: 0 5px 25px rgba(0,0,0,0.1);
      border: 1px solid rgba(52, 152, 219, 0.2);
    }
    .logo {
      height: 100px; /* 调整Logo大小 */
      width: auto;
      margin: 0 auto 1.5rem;
      display: block;
    }
    .header h1 {
      color: #2c3e50;
      margin-bottom: 0.5rem;
      font-size: 2.5rem;
    }
    .header p {
      color: #7f8c8d;
      margin-bottom: 1.5rem;
      font-size: 1.1rem;
    }
    #lang-toggle {
      background: #3498db;
      border: none;
      color: white;
      padding: 0.8rem 1.5rem;
      border-radius: 50px;
      cursor: pointer;
      font-weight: 600;
      transition: all 0.3s ease;
      box-shadow: 0 4px 15px rgba(52, 152, 219, 0.3);
    }
    #lang-toggle:hover {
      background: #2980b9;
      transform: translateY(-2px);
    }

    /* === 内容区块样式 === */
    section {
      background: rgba(255, 255, 255, 0.95);
      padding: 2.5rem;
      margin-bottom: 2.5rem;
      border-radius: 15px;
      box-shadow: 0 5px 20px rgba(0,0,0,0.08);
      border: 1px solid rgba(52, 152, 219, 0.1);
    }
    h2 {
      color: #2c3e50;
      margin-bottom: 1.8rem;
      padding-bottom: 0.8rem;
      border-bottom: 3px solid #3498db;
      font-size: 1.8rem;
    }

    /* === 关于我们 - 添加照片 === */
    .about-content {
      display: flex;
      align-items: center;
      gap: 2.5rem;
    }
    @media (max-width: 768px) {
      .about-content { flex-direction: column; }
    }
    .profile-photo {
      width: 280px;
      height: 280px;
      border-radius: 50%;
      object-fit: cover;
      border: 5px solid #ecf0f1;
      box-shadow: 0 8px 25px rgba(0,0,0,0.15);
      flex-shrink: 0;
    }
    .about-text {
      flex: 1;
    }

    /* === 服务列表样式 === */
    .services ul {
      list-style: none;
      padding: 0;
      columns: 2;
    }
    @media (max-width: 600px) {
      .services ul { columns: 1; }
    }
    .services li {
      padding: 0.8rem 0;
      position: relative;
      padding-left: 1.8rem;
    }
    .services li:before {
      content: "✓";
      color: #27ae60;
      font-weight: bold;
      position: absolute;
      left: 0;
    }

    /* === 价格表样式 === */
    .pricing table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 1.2rem;
    }
    .pricing th {
      background: linear-gradient(135deg, #3498db, #2980b9);
      color: white;
      padding: 1.2rem;
      text-align: left;
    }
    .pricing td {
      padding: 1.2rem;
      border-bottom: 1px solid #ecf0f1;
    }
    .pricing tr:nth-child(even) {
      background-color: #f8f9fa;
    }
    .pricing tr:hover {
      background-color: #e8f4fc;
    }

    /* === 联系区块样式 - 已添加QR码 === */
    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 2rem;
      align-items: center;
    }
    @media (max-width: 768px) {
      .contact-grid { grid-template-columns: 1fr; }
    }
    .qr-code {
      width: 200px;
      border: 1px solid #ddd;
      padding: 10px;
      background: white;
      border-radius: 10px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
      justify-self: center;
    }

    /* === 按钮样式 === */
    .btn-primary {
      background: linear-gradient(135deg, #3498db, #2980b9);
      color: white;
      border: none;
      padding: 1rem 2rem;
      border-radius: 50px;
      cursor: pointer;
      font-size: 1.1rem;
      font-weight: 600;
      transition: all 0.3s ease;
      box-shadow: 0 5px 15px rgba(52, 152, 219, 0.3);
      display: inline-block;
      margin: 0.5rem;
      text-decoration: none;
    }
    .btn-primary:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 25px rgba(52, 152, 219, 0.4);
    }

    /* === 页脚样式 === */
    footer {
      text-align: center;
      padding: 2.5rem;
      color: #7f8c8d;
      margin-top: 3rem;
      background: rgba(255, 255, 255, 0.9);
      border-radius: 15px;
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- 页头 - 已添加Logo -->
    <header class="header">
      <img src="/images/logo.png" alt="Little Dreamer Limited Logo" class="logo">
      <h1>Little Dreamer Limited</h1>
      <p>New Zealand & Australia Chartered Accountants | CPA | Tax Agents</p>
      <button id="lang-toggle">中文 / English</button>
    </header>

    <!-- 关于我们 - 已添加个人照片 -->
    <section class="about">
      <h2>About Us</h2>
      <div class="about-content">
        <img src="/images/harry-photo.jpg" alt="Harry Hu - Chartered Accountant" class="profile-photo">
        <div class="about-text">
          <p id="about-text">We are Chartered Accountants and Tax Agents in New Zealand & Australia, providing professional accounting, tax, and business advisory services for individuals and SMEs. With over 15 years of experience, we help our clients navigate complex financial landscapes with ease and confidence.</p>
          <p><strong>Director:</strong> Harry Hu, CA, CPA</p>
          <p><strong>Specializations:</strong> SME Taxation, Business Advisory, Xero/MYOB Consulting</p>
        </div>
      </div>
    </section>

    <!-- 服务 -->
    <section class="services">
      <h2>Our Services</h2>
      <ul>
        <li>GST Return Filing & BAS Preparation</li>
        <li>Income Tax Returns (Individual & Company)</li>
        <li>PAYE & Payroll Services</li>
        <li>Company Formation & ASIC Compliance</li>
        <li>Trust & Estate Tax Returns</li>
        <li>Rental Property Investment Tax</li>
        <li>Business Advisory & Financial Planning</li>
        <li>Xero & MYOB Setup, Training & Support</li>
        <li>Financial Statements Preparation</li>
        <li>Cash Flow Management & Forecasting</li>
      </ul>
    </section>

    <!-- 价格 -->
    <section class="pricing">
      <h2>Pricing Packages</h2>
      <table>
        <tr><th>Service</th><th>Price (NZD)</th><th>Price (AUD)</th></tr>
        <tr><td>Basic GST Return</td><td>From $150 + GST</td><td>From $140 + GST</td></tr>
        <tr><td>Individual Tax Return</td><td>From $200 + GST</td><td>From $190 + GST</td></tr>
        <tr><td>Company Tax Return</td><td>From $300 + GST</td><td>From $280 + GST</td></tr>
        <tr><td>Business Advisory</td><td>$150 / hour + GST</td><td>$140 / hour + GST</td></tr>
        <tr><td>Xero/MYOB Setup</td><td>$250 + GST</td><td>$230 + GST</td></tr>
      </table>
      <p style="margin-top: 1rem; font-style: italic; color: #7f8c8d;">* All prices are indicative. Contact us for a fixed-price quote tailored to your specific needs.</p>
    </section>

    <!-- 联系方式 - 已添加QR码 -->
    <section class="contact">
      <h2>Contact Us Today</h2>
      <div class="contact-grid">
        <div>
          <p><strong>Email:</strong> info@littledreamer.co.nz</p>
          <p><strong>Phone NZ:</strong> 021 030 8628</p>
          <p><strong>Phone AU:</strong> +61 XXX XXX XXX</p>
          <p><strong>WeChat:</strong> harrylemon</p>
          <p><strong>Address:</strong> 62b Sartors Avenue, Browns Bay, Auckland 0630, NZ</p>
          
          <div style="margin-top: 1.5rem;">
            <a href="mailto:info@littledreamer.co.nz" class="btn-primary">Email Us</a>
            <a href="tel:+64210308628" class="btn-primary">Call Now</a>
          </div>
        </div>
        
        <div>
          <img src="/images/wechat-qr.png" alt="Scan WeChat QR Code" class="qr-code">
          <p style="text-align: center; margin-top: 0.5rem;">Scan to add on WeChat</p>
        </div>
      </div>
    </section>

    <footer>
      <p>© 2025 Little Dreamer Limited. Chartered Accountants serving New Zealand & Australia. All Rights Reserved.</p>
      <p>Liability limited by a scheme approved under Professional Standards Legislation</p>
    </footer>
  </div>

  <script>
    // 语言切换功能
    document.getElementById('lang-toggle').addEventListener('click', function() {
      const aboutText = document.getElementById('about-text');
      const currentLang = aboutText.innerText;
      
      if (currentLang.includes('New Zealand')) {
        aboutText.innerText = '我们是新西兰和澳大利亚的特许会计师和税务代理，为个人和中小企业提供专业的会计、税务和商业咨询服务。拥有超过15年的经验，我们帮助客户轻松自信地应对复杂的财务环境。';
        this.innerText = 'English / 中文';
        
        // 可以在这里添加更多元素的翻译
        document.querySelector('.about h2').textContent = '关于我们';
        document.querySelector('.services h2').textContent = '我们的服务';
        document.querySelector('.pricing h2').textContent = '服务价格';
        document.querySelector('.contact h2').textContent = '联系我们';
        
      } else {
        aboutText.innerText = 'We are Chartered Accountants and Tax Agents in New Zealand & Australia, providing professional accounting, tax, and business advisory services for individuals and SMEs. With over 15 years of experience, we help our clients navigate complex financial landscapes with ease and confidence.';
        this.innerText = '中文 / English';
        
        // 恢复英文
        document.querySelector('.about h2').textContent = 'About Us';
        document.querySelector('.services h2').textContent = 'Our Services';
        document.querySelector('.pricing h2').textContent = 'Pricing Packages';
        document.querySelector('.contact h2').textContent = 'Contact Us Today';
      }
    });
  </script>
</body>
</html>
