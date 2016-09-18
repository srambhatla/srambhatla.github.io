---
layout: post
title: Blog
date:   2015-10-16 04:36:43
permalink: /blog/
weight : 1
---
<div>
 <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span> 
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}"> <span class="post-link">{{ post.title }}  </span></a> 
        </h2>
      </li>
    {% endfor %}
  </ul>
  </div>