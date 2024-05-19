---
title: Bundle 
layout: default
permalink: bundle/
---

<div class="myposts">
{% for post in site.posts %}
    {% if post.categories contains 'Bundle' %}
        <div class="mypost"><h2><a class="postTitle" href="{{ post.url }}" >{{ post.title}}</a></h2>
        {{ post.excerpt }}
        <div class="right"><i><span class="postTag">{{ post.tags }}</span></i> <br>
        <i><span class="postDate">{{ post.date | date: "%b %-d, %Y" }}</span></i>
        </div>
            <hr class="pad">    
        </div>
    {% endif %}
{% endfor %}
</div>