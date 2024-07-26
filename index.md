<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>{{ site.title }}</title>
    <link rel="stylesheet" href="{{ '/_style/news.css' | relative_url }}">
</head>
<body>
    <header style="background-image: url('{{ site.header }}'); height: 200px;">
        <h1>{{ site.title }}</h1>
        <p>{{ site.subtitle }}</p>
    </header>
    
    <div class="content">
        <h2>新闻</h2>
        <div class="news-grid">
            {% assign news_items = site.news | limit: 6 %}
            {% for news in news_items %}
                <div class="news-item">
                    <a href="{{ news.url }}">
                        <h3>{{ news.title }}</h3>
                        <p>{{ news.date | date: "%Y-%m-%d" }}</p>
                    </a>
                </div>
            {% endfor %}
        </div>
    </div>

    <footer style="background-image: url('{{ site.footer }}'); height: 100px;">
        <p>© 2024 天行 test</p>
    </footer>
</body>
</html>
