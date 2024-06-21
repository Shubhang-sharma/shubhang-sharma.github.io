---
title: Art Review
layout: art
permalink: artreview/
---

<div class="myposts">
{% for post in site.posts %}
    {% if post.categories contains 'ArtReview' %}
        <div class="mypost"><h2><a class="postTitle" href="{{ post.url }}" >{{ post.title}}</a></h2>
        {{ post.excerpt }}
        <div class="right postPost"><i><span class="postTag">Creator(s): {{ post.tags }}</span></i> <br>
        <i><span class="postDate">{{ post.date | date: "%b %-d, %Y" }}</span></i>
        </div>
            <hr class="pad">    
        </div>
    {% endif %}
{% endfor %}
</div>
