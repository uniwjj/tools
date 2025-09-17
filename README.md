<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>开发者工具箱</title>
    <style>
        :root {
            --primary-color: #4361ee;
            --secondary-color: #3a0ca3;
            --accent-color: #7209b7;
            --light-color: #f8f9fa;
            --dark-color: #212529;
            --success-color: #4cc9f0;
            --card-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            min-height: 100vh;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        header {
            text-align: center;
            margin: 30px 0;
            color: var(--dark-color);
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            background: linear-gradient(to right, var(--primary-color), var(--accent-color));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .subtitle {
            font-size: 1.2rem;
            color: #6c757d;
            max-width: 600px;
        }
        
        .tools-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
            max-width: 1200px;
            margin: 20px 0 50px;
        }
        
        .tool-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            width: 300px;
            box-shadow: var(--card-shadow);
            transition: var(--transition);
            display: flex;
            flex-direction: column;
        }
        
        .tool-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }
        
        .tool-header {
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            color: white;
            padding: 20px;
            text-align: center;
        }
        
        .tool-icon {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }
        
        .tool-title {
            font-size: 1.5rem;
            margin-bottom: 5px;
        }
        
        .tool-content {
            padding: 20px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }
        
        .tool-description {
            color: #6c757d;
            margin-bottom: 20px;
            line-height: 1.5;
        }
        
        .tool-link {
            display: block;
            background: var(--primary-color);
            color: white;
            text-align: center;
            padding: 12px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            margin-top: auto;
            transition: var(--transition);
        }
        
        .tool-link:hover {
            background: var(--secondary-color);
        }
        
        footer {
            text-align: center;
            margin-top: auto;
            padding: 20px;
            color: #6c757d;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .tools-container {
                flex-direction: column;
                align-items: center;
            }
            
            .tool-card {
                width: 100%;
                max-width: 350px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>开发者工具箱</h1>
        <p class="subtitle">精心挑选的开发工具，帮助您提高工作效率和代码质量</p>
    </header>
    
    <div class="tools-container">
        <div class="tool-card">
            <div class="tool-header">
                <div class="tool-icon">⇄</div>
                <h2 class="tool-title">文本比对工具</h2>
            </div>
            <div class="tool-content">
                <p class="tool-description">快速比较两个文本文件或代码片段之间的差异，高亮显示新增、删除和修改的内容，支持多种输出格式。</p>
                <a href="html/diff.html" class="tool-link">使用工具</a>
            </div>
        </div>
        
        <div class="tool-card">
            <div class="tool-header">
                <div class="tool-icon">{ }</div>
                <h2 class="tool-title">JSON格式化工具</h2>
            </div>
            <div class="tool-content">
                <p class="tool-description">将压缩的JSON数据格式化并美化，使其更易于阅读和调试，支持语法高亮和错误检查功能。</p>
                <a href="html/json.html" class="tool-link">使用工具</a>
            </div>
        </div>
    </div>
    
    <footer>
        <p>© 2025 开发者工具箱 | 为您提供便捷的开发体验</p>
    </footer>
</body>
</html>


