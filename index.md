---
layout: default
title: NorthStack Example Blog
---

<div class="posts">
    {% for post in site.posts %}
        <article>
            {% if post.image.feature %}
                <img src="{{ post.image.feature }}" />
            {% else %}        
                <img src="http://lorempixel.com/200/100/" />
            {% endif %}    
            <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
            Published on {{ post.date | date_to_string }}
            {{ post.excerpt }}
        </article>
    {% endfor %}
</div>


ようこそ :+1:
