# test
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我的前端页面</title>
    <style>
        /* 全局样式 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
            line-height: 1.6;
        }
        
        /* 导航栏 */
        header {
            background-color: #2c3e50;
            color: white;
            padding: 1rem 2rem;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 2rem;
        }
        
        .nav-links a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: #3498db;
        }
        
        /* 主要内容 */
        .container {
            max-width: 1200px;
            margin: 2rem auto;
            padding: 0 2rem;
        }
        
        .hero {
            text-align: center;
            padding: 4rem 0;
        }
        
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
        }
        
        .btn {
            display: inline-block;
            background-color: #3498db;
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 5px;
            text-decoration: none;
            transition: background-color 0.3s;
        }
        
        .btn:hover {
            background-color: #2980b9;
        }
        
        /* 卡片区域 */
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 3rem 0;
        }
        
        .card {
            background-color: white;
            border-radius: 8px;
            padding: 2rem;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .card:hover {
            transform: translateY(-5px);
        }
        
        .card h3 {
            margin-bottom: 1rem;
            color: #2c3e50;
        }
        
        /* 页脚 */
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 3rem;
        }
        
        /* 响应式设计 */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">我的网站</div>
            <ul class="nav-links">
                <li><a href="#">首页</a></li>
                <li><a href="#">产品</a></li>
                <li><a href="#">关于我们</a></li>
                <li><a href="#">联系我们</a></li>
            </ul>
        </nav>
    </header>
    
    <div class="container">
        <section class="hero">
            <h1>欢迎来到我的前端页面</h1>
            <p>这是一个使用HTML、CSS和JavaScript构建的响应式网页示例。您可以在此基础上进行修改和扩展。</p>
            <a href="#" class="btn">了解更多</a>
        </section>
        
        <section class="features">
            <div class="card">
                <h3>响应式设计</h3>
                <p>自动适应不同屏幕尺寸，在手机、平板和电脑上都能完美显示。</p>
            </div>
            <div class="card">
                <h3>现代化UI</h3>
                <p>简洁美观的设计风格，符合当代网页设计趋势。</p>
            </div>
            <div class="card">
                <h3>易于扩展</h3>
                <p>清晰的代码结构，方便添加新功能和组件。</p>
            </div>
        </section>
    </div>
    
    <footer>
        <p>&copy; 2023 我的网站. 保留所有权利.</p>
    </footer>
    
    <script>
        // 简单的JavaScript交互
        document.addEventListener('DOMContentLoaded', function() {
            // 卡片点击效果
            const cards = document.querySelectorAll('.card');
            cards.forEach(card => {
                card.addEventListener('click', function() {
                    alert('您点击了: ' + this.querySelector('h3').textContent);
                });
            });
            
            // 导航栏滚动效果
            window.addEventListener('scroll', function() {
                const header = document.querySelector('header');
                if (window.scrollY > 50) {
                    header.style.background = 'rgba(44, 62, 80, 0.9)';
                } else {
                    header.style.background = '#2c3e50';
                }
            });
        });
    </script>
</body>
</html>

<h1>--------------------------------------------------------------------------------------------------------</h1>
<html>
<body>
</body>
</html>
