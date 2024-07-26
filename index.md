---
layout: news
title: 新闻
---

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
