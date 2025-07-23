<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>清越科技</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', 'system-ui', sans-serif;
        }

        :root {
            --primary: #2563eb;
            --primary-light: #eff6ff;
            --dark: #1e293b;
            --light: #f8fafc;
            --gray: #94a3b8;
            --shadow: 0 4px 20px rgba(0,0,0,0.08);
        }

        body {
            background: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        /* 导航栏 */
        .navbar {
            background: white;
            padding: 1.2rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: var(--shadow);
        }

        .nav-wrap {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary);
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            gap: 2.5rem;
            list-style: none;
        }

        .nav-links a {
            color: var(--dark);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        /* 头部区域 */
        .header {
            padding: 8rem 0;
            background: var(--primary-light);
            text-align: center;
            margin-bottom: 5rem;
        }

        .header h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--dark);
        }

        .header p {
            color: var(--dark);
            opacity: 0.8;
            max-width: 600px;
            margin: 0 auto;
        }

        /* 通用区块样式 */
        .section {
            padding: 5rem 0;
            margin-bottom: 3rem;
        }

        .section-title {
            font-size: 1.8rem;
            margin-bottom: 3rem;
            position: relative;
            padding-bottom: 0.8rem;
            display: inline-block;
        }

        .section-title::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: 0;
            width: 60px;
            height: 3px;
            background: var(--primary);
        }

        /* 公司简介 */
        .about {
            background: white;
            border-radius: 12px;
            padding: 3rem;
            box-shadow: var(--shadow);
        }

        .about p {
            margin-bottom: 1.5rem;
            line-height: 1.8;
            color: var(--dark);
            opacity: 0.9;
        }

        /* 经营方向 */
        .services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .service-card {
            background: white;
            padding: 2rem;
            border-radius: 12px;
            box-shadow: var(--shadow);
            transition: transform 0.3s;
        }

        .service-card:hover {
            transform: translateY(-5px);
        }

        .service-card h3 {
            margin-bottom: 1rem;
            color: var(--primary);
        }

        /* 联系区域 */
        .contact {
            background: white;
            border-radius: 12px;
            padding: 3rem;
            box-shadow: var(--shadow);
        }

        .contact-form .form-group {
            margin-bottom: 1.5rem;
        }

        .contact-form label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 500;
        }

        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #e2e8f0;
            border-radius: 6px;
            font-size: 1rem;
        }

        .btn {
            background: var(--primary);
            color: white;
            border: none;
            padding: 0.8rem 2rem;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 500;
            transition: background 0.3s;
        }

        .btn:hover {
            background: #1d4ed8;
        }

        /* 页脚 */
        .footer {
            background: var(--dark);
            color: white;
            padding: 3rem 0;
            text-align: center;
            margin-top: 5rem;
        }

        /* 响应式调整 */
        @media (max-width: 768px) {
            .nav-links {
                gap: 1.5rem;
            }
            
            .header {
                padding: 5rem 0;
            }
            
            .section {
                padding: 3rem 0;
            }
            
            .about, .contact {
                padding: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- 导航栏 -->
    <nav class="navbar">
        <div class="container nav-wrap">
            <a href="#" class="logo">清越科技</a>
            <ul class="nav-links">
                <li><a href="#about">关于我们</a></li>
                <li><a href="#services">经营方向</a></li>
                <li><a href="#contact">联系我们</a></li>
            </ul>
        </div>
    </nav>

    <!-- 头部区域 -->
    <div class="header">
        <div class="container">
            <h1>专注于前沿科技研发与应用</h1>
            <p>以简洁高效的解决方案，助力企业数字化转型</p>
        </div>
    </div>

    <!-- 主要内容 -->
    <div class="container">
        <!-- 公司简介 -->
        <section id="about" class="section">
            <h2 class="section-title">关于我们</h2>
            <div class="about">
                <p>清越科技成立于2015年，是一家专注于企业数字化解决方案的科技公司。我们致力于通过前沿技术，为客户提供简单、高效的数字化工具。</p>
                <p>公司核心团队来自知名科技企业，拥有平均10年以上行业经验，深刻理解企业在数字化转型中的痛点与需求。</p>
                <p>我们坚持"简洁至上"的产品理念，拒绝冗余功能，专注于解决实际问题，已为超过300家企业提供服务。</p>
            </div>
        </section>

        <!-- 经营方向 -->
        <section id="services" class="section">
            <h2 class="section-title">经营方向</h2>
            <div class="services">
                <div class="service-card">
                    <h3>企业SaaS解决方案</h3>
                    <p>为中小企业提供轻量化管理软件，涵盖客户关系、项目管理、数据分析等核心功能模块，即开即用。</p>
                </div>
                <div class="service-card">
                    <h3>定制化开发服务</h3>
                    <p>根据企业特定需求，提供定制化系统开发服务，包括流程梳理、功能设计、系统实现及后期维护。</p>
                </div>
                <div class="service-card">
                    <h3>数字化咨询服务</h3>
                    <p>为企业提供数字化转型路径规划，帮助企业梳理业务流程，制定合理的数字化实施步骤与方案。</p>
                </div>
            </div>
        </section>

        <!-- 联系我们 -->
        <section id="contact" class="section">
            <h2 class="section-title">联系我们</h2>
            <div class="contact">
                <form class="contact-form">
                    <div class="form-group">
                        <label for="name">姓名</label>
                        <input type="text" id="name" placeholder="请输入您的姓名">
                    </div>
                    <div class="form-group">
                        <label for="email">邮箱</label>
                        <input type="email" id="email" placeholder="请输入您的邮箱">
                    </div>
                    <div class="form-group">
                        <label for="message">留言</label>
                        <textarea id="message" rows="4" placeholder="请输入您的需求"></textarea>
                    </div>
                    <button type="submit" class="btn">提交</button>
                </form>
            </div>
        </section>
    </div>

    <!-- 页脚 -->
    <footer class="footer">
        <div class="container">
            <p>© 2023 清越科技 版权所有</p>
        </div>
    </footer>
</body>
</html>
