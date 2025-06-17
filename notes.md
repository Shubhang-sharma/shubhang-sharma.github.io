---
title: Notes 
layout: default
permalink: notes/
---


- [AdS/CFT Correspondence and Geometry](..\assets\docs\2011106_MSc_Thesis.pdf) - Master's  thesis.
- [Introduction to Manifolds](..\assets\docs\dg_notes.pdf) - Lecture Notes. Under preparation.
- [Quantum Electrodynamics](..\assets\docs\qed.djvu) - Part of the Lectures notes on a second course in Quantum Field Theory.
- [Renormalization](..\assets\docs\renormalization.djvu) - Part of the Lectures notes on a second course in Quantum Field Theory



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


