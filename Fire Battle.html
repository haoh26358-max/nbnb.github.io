<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fire Battle全防</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
    }
    html {
      scroll-behavior: smooth;
    }
    body {
      color: #f5f5f5;
      line-height: 1.6;
      position: relative;
      overflow-x: hidden;
      background-color: #0a0a1a;
    }

    /* 粒子背景 + 动态效果 */
    .particle {
      position: absolute;
      border-radius: 50%;
      opacity: 0;
      pointer-events: none;
      z-index: -1;
    }
    .pink {
      background-color: rgba(255, 42, 140, 0.6);
    }
    .blue {
      background-color: rgba(0, 170, 255, 0.6);
    }
    @keyframes float {
      0% {
        transform: translate(0, 0);
        opacity: 0;
      }
      10% {
        opacity: 1;
      }
      90% {
        opacity: 1;
      }
      100% {
        transform: translate(100vw, 100vh);
        opacity: 0;
      }
    }

    /* 导航栏样式 - 透明模糊效果 */
    .navbar {
      position: sticky;
      top: 0;
      z-index: 999;
      padding: 16px 0;
      backdrop-filter: blur(10px);
      background-color: rgba(10, 10, 26, 0.7);
      border-bottom: 1px solid rgba(255, 255, 255, 0.1);
    }
    .navbar .container {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .logo {
      font-size: 1.5rem;
      font-weight: 800;
      color: #00aaff;
    }
    .nav-links {
      display: flex;
      gap: 24px;
    }
    .nav-links a {
      color: #ccc;
      text-decoration: none;
      transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
      position: relative;
    }
    .nav-links a::after {
      content: "";
      position: absolute;
      bottom: -5px;
      left: 0;
      width: 0;
      height: 2px;
      background: linear-gradient(90deg, #ff2a8c, #00aaff);
      transition: width 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    }
    .nav-links a:hover {
      color: #00aaff;
    }
    .nav-links a:hover::after {
      width: 100%;
    }

    /* 容器与横幅样式 */
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 20px;
    }
    .banner {
      padding: 100px 0;
      text-align: center;
      position: relative;
    }
    .banner h1 {
      font-size: 3.2rem;
      font-weight: 900;
      margin-bottom: 20px;
      background: linear-gradient(90deg, #ff2a8c, #00aaff, #ff2a8c);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      animation: fadeInUp 1s cubic-bezier(0.25, 0.8, 0.25, 1);
    }
    .banner p {
      font-size: 1.2rem;
      color: #ccc;
      max-width: 600px;
      margin: 0 auto 40px;
      animation: fadeInUp 1s cubic-bezier(0.25, 0.8, 0.25, 1) 0.2s both;
    }
    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    /* 按钮样式 - 透明模糊 + 灵动动画 */
    .btn-group {
      display: flex;
      justify-content: center;
      gap: 16px;
      flex-wrap: wrap;
      animation: fadeInUp 1s cubic-bezier(0.25, 0.8, 0.25, 1) 0.4s both;
    }
    .btn {
      display: inline-block;
      padding: 12px 28px;
      border: none;
      border-radius: 8px;
      font-weight: 600;
      cursor: pointer;
      text-decoration: none;
      position: relative;
      overflow: hidden;
      backdrop-filter: blur(8px);
      background-color: rgba(0, 170, 255, 0.2);
      color: #fff;
      transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
      box-shadow: 0 4px 12px rgba(0, 170, 255, 0.1);
    }
    .btn::before {
      content: "";
      position: absolute;
      top: 0;
      left: -100%;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
      transition: all 0.6s cubic-bezier(0.25, 0.8, 0.25, 1);
    }
    .btn:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 20px rgba(0, 170, 255, 0.3);
    }
    .btn:hover::before {
      left: 100%;
    }
    .btn-outline {
      background-color: transparent;
      border: 2px solid rgba(0, 170, 255, 0.5);
    }

    /* 功能区样式 */
    .features {
      padding: 80px 0;
    }
    .features h2 {
      font-size: 2.2rem;
      text-align: center;
      margin-bottom: 50px;
      background: linear-gradient(90deg, #00aaff, #ff2a8c);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }
    .features-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 30px;
    }
    .feature-card {
      background-color: rgba(18, 18, 42, 0.8);
      padding: 30px;
      border-radius: 12px;
      transition: all 0.4s cubic-bezier(0.25, 0.8, 0.25, 1);
      backdrop-filter: blur(8px);
      position: relative;
      overflow: hidden;
      cursor: pointer;
    }
    .feature-card::before {
      content: "";
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 3px;
      background: linear-gradient(90deg, #ff2a8c, #00aaff);
      transform: scaleX(0);
      transform-origin: left;
      transition: transform 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    }
    .feature-card:hover::before {
      transform: scaleX(1);
    }
    .feature-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 24px rgba(0, 170, 255, 0.15);
    }
    .feature-icon {
      font-size: 2.8rem;
      color: #00aaff;
      margin-bottom: 20px;
    }
    .feature-card h3 {
      font-size: 1.6rem;
      margin-bottom: 15px;
      color: #00aaff;
    }
    .feature-card p {
      color: #ccc;
    }

    /* 购买区样式 */
    .buy-section {
      padding: 80px 0;
      text-align: center;
    }
    .buy-section h2 {
      font-size: 2.2rem;
      margin-bottom: 30px;
      background: linear-gradient(90deg, #00aaff, #ff2a8c);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }
    .buy-grid {
      display: flex;
      flex-direction: column;
      gap: 40px;
      align-items: center;
      animation: fadeInUp 1s cubic-bezier(0.25, 0.8, 0.25, 1);
    }
    .buy-card {
      background-color: rgba(18, 18, 42, 0.8);
      padding: 30px;
      border-radius: 12px;
      width: 100%;
      max-width: 400px;
      backdrop-filter: blur(8px);
      transition: all 0.4s cubic-bezier(0.25, 0.8, 0.25, 1);
    }
    .buy-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 24px rgba(0, 170, 255, 0.15);
    }
    .buy-card h3 {
      font-size: 1.6rem;
      margin-bottom: 20px;
      color: #00aaff;
    }
    .buy-card p {
      color: #ccc;
      margin-bottom: 30px;
    }

    /* 合作项目区样式 */
    .partners {
      padding: 80px 0;
      text-align: center;
    }
    .partners h2 {
      font-size: 2.2rem;
      margin-bottom: 50px;
      background: linear-gradient(90deg, #00aaff, #ff2a8c);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }
    .partners-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 30px;
    }
    .partner-card {
      background-color: rgba(18, 18, 42, 0.8);
      padding: 30px;
      border-radius: 12px;
      transition: all 0.4s cubic-bezier(0.25, 0.8, 0.25, 1);
      backdrop-filter: blur(8px);
      cursor: pointer;
    }
    .partner-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 12px 24px rgba(0, 170, 255, 0.15);
    }
    .partner-card h3 {
      font-size: 1.6rem;
      margin-bottom: 15px;
      color: #00aaff;
    }
    .partner-card p {
      color: #ccc;
      margin-bottom: 25px;
    }
    .partner-btn {
      display: inline-block;
      padding: 8px 18px;
      border: 2px solid rgba(0, 170, 255, 0.5);
      color: #00aaff;
      border-radius: 6px;
      text-decoration: none;
      transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    }
    .partner-btn:hover {
      background-color: rgba(0, 170, 255, 0.2);
    }

    /* 响应式适配 */
    @media (max-width: 768px) {
      .features-grid, .partners-grid {
        grid-template-columns: 1fr;
      }
      .banner h1 {
        font-size: 2.5rem;
      }
      .nav-links {
        display: none;
      }
    }
  </style>
</head>
<body>
  <nav class="navbar">
    <div class="container">
      <div class="logo">Fire Battle全防</div>
      <div class="nav-links">
        <a href="#features">特性</a>
        <a href="#buy">购买</a>
        <a href="#partners">合作项目</a>
      </div>
    </div>
  </nav>

  <section class="banner">
    <div class="container">
      <h1>Fire Battle全防项目</h1>
      <p>强大的功能以及防封，为使用者提高安全以及作弊</p>
      <div class="btn-group">
        <a href="#buy" class="btn">购买密钥</a>
        <a href="#features" class="btn btn-outline">了解更多</a>
      </div>
    </div>
  </section>

  <section id="features" class="features">
    <div class="container">
      <h2>Fire Battle功能介绍</h2>
      <div class="features-grid">
        <div class="feature-card">
          <div class="feature-icon">🤺</div>
          <h3>人物动作</h3>
          <p>强大的人物动作系统，支持自定义动作序列与动态交互，提升操作灵活性。</p>
        </div>
        <div class="feature-card">
          <div class="feature-icon">⚙️</div>
          <h3>自定义修改道具</h3>
          <p>强大的自定义修改道具功能，可将任意道具转换为目标类型，满足多样化需求。</p>
        </div>
        <div class="feature-card">
          <div class="feature-icon">👥</div>
          <h3>修改敌人的召唤人物</h3>
          <p>支持修改敌人召唤的人物等级与属性，可实现从高级到低级的自由转换策略。</p>
        </div>
        <div class="feature-card">
          <div class="feature-icon">☁️</div>
          <h3>云端更新</h3>
          <p>云更新脚本机制，无需重复下载即可获取最新功能，保持系统持续迭代。</p>
        </div>
      </div>
    </div>
  </section>

  <section id="buy" class="buy-section">
    <div class="container">
      <h2>选择密钥套餐</h2>
      <div class="buy-grid">
        <div class="buy-card">
          <h3>1天密钥 - 购买页面</h3>
          <p>适合短期体验用户，提供24小时全功能访问权限。</p>
          <a href="https://shop.xm1.xyz/Q5a6d" class="btn" target="_blank">确认购买1天密钥</a>
        </div>
        <div class="buy-card">
          <h3>7天密钥 - 购买页面</h3>
          <p>7天有效期，性价比优选，支持多设备登录与专属技术支持。</p>
          <a href="https://shop.xm1.xyz/Q5a6d" class="btn" target="_blank">确认购买周卡用户组</a>
        </div>
        <div class="buy-card">
          <h3>30天密钥 - 购买页面</h3>
          <p>30天全功能权限，享优先更新与一对一客服，适合长期用户。</p>
          <a href="https://shop.xm1.xyz/Q5a6d" class="btn" target="_blank">确认购买月卡用户组</a>
        </div>
        <div class="buy-card">
          <h3>永久密钥 - 购买页面</h3>
          <p>终身使用权限，一次购买永久免费更新，终极选择。</p>
          <a href="https://shop.xm1.xyz/Q5a6d" class="btn" target="_blank">确认购买永久密钥</a>
        </div>
      </div>
    </div>
  </section>

  <section id="partners" class="partners">
    <div class="container">
      <h2>谁在使用我们的辅助</h2>
      <div class="partners-grid">
        <div class="partner-card">
          <h3>一</h3>
          <p>no</p>
          <a href=" " class="partner-btn" target="_blank"></a>
        </div>
        <div class="partner-card">
          <h3>二</h3>
          <p>no</p>
          <a href="https://www.project2.com" class="partner-btn" target="_blank"></a>
        </div>
        <div class="partner-card">
          <h3>三</h3>
          <p></p>
          <a href="https://www.project3.com" class="partner-btn" target="_blank"></a>
        </div>
        <div class="partner-card">
          <h3>四</h3>
          <p></p>
          <a href="https://www.project4.com" class="partner-btn" target="_blank"></a>
        </div>
      </div>
    </div>
  </section>

  <script>
    // 粒子背景生成逻辑
    let particles = [];
    const particleColors = ['pink', 'blue'];
    const maxParticles = 60;

    function createParticle() {
      const particle = document.createElement('div');
      const color = particleColors[Math.floor(Math.random() * particleColors.length)];
      particle.className = `particle ${color}`;
      particle.style.width = `${Math.random() * 15 + 5}px`;
      particle.style.height = particle.style.width;
      particle.style.left = `${Math.random() * 100}vw`;
      particle.style.top = `${window.scrollY + Math.random() * window.innerHeight}px`;
      particle.style.animationDelay = `${Math.random() * 10}s`;
      particle.style.animation = 'float 10s infinite linear';
      document.body.appendChild(particle);
      particles.push(particle);

      setTimeout(() => {
        particle.remove();
        particles = particles.filter(p => p !== particle);
      }, 10000);
    }

    // 初始化生成粒子
    for (let i = 0; i < 30; i++) {
      createParticle();
    }

    // 滚动时持续生成粒子
    setInterval(() => {
      if (particles.length < maxParticles) {
        createParticle();
      }
    }, 1000);

    // 平滑滚动（基于cubic-bezier曲线优化）
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
          behavior: 'smooth',
          block: 'start',
          inline: 'nearest'
        });
      });
    });
  </script>
</body>
</html>
