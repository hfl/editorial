---
layout: post
title:  增加分页功能
date:   2025-12-20 14:59:00 +0800
categories: jekyll pagniator
---

为 Jekyll 添加分页功能。该功能在 2 版本之前是内容功能，2 版本之后分离为单独的插件公共。如果需要则要单独添加：

1. 在 `Gemfile` 文件中增加 `jekyll-paginate` 插件：
   ~~~ruby
    gem jekyll-paginate
   ~~~
2. 在 `_config.yml` 中添加插件：
   ~~~ruby
     plugins:
       - jekyll-paginate
   ~~~
3. 同时设置每页显示博客数量`paginate: 5`
4. 首页必须是 `.html` 格式，也就是首页的文件名为 `index.html`
5. 添加分页显示代码：
   ~~~ruby
     {% if paginator.total_pages > 1 %}
       <div class="pagination">
     {% if paginator.previous_page %}
       <a href="{{ paginator.previous_page_path | relative_url }}">&laquo; Prev</a>
     {% else %}
       <span>&laquo; Prev</span>
     {% endif %}
     
     {% for page in (1..paginator.total_pages) %}
     {% if page == paginator.page %}
       <em>{{ page }}</em>
     {% elsif page == 1 %}
       <a href="{{ site.paginate_path | relative_url | replace: 'page:num/', '' }}">{{ page }}</a>
     {% else %}
       <a href="{{ site.paginate_path | relative_url | replace: ':num', page }}">{{ page }}</a>
     {% endif %}
     {% endfor %}
      
     {% if paginator.next_page %}
       <a href="{{ paginator.next_page_path | relative_url }}">Next &raquo;</a>
     {% else %}
       <span>Next &raquo;</span>
     {% endif %}
      </div>
     {% endif %}
   ~~~
