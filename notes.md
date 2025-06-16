---
title: Notes 
layout: default
permalink: notes/
---

<div class="myposts">
{% for post in site.posts %}
    {% if post.categories contains 'Notes' %}
        <div class="mypost"><h2><a class="postTitle" href="{{ post.url }}" >{{ post.title}}</a></h2>
        {{ post.excerpt }}
        <div class="right postPost"><i><span class="postTag">{{ post.tags }}</span></i> <br>
        <span class="postDate">{{ post.date | date: "%b %-d, %Y" }}</span>
        </div>
            <hr class="pad">    
        </div>
    {% endif %}
{% endfor %}
</div>
