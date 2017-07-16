---
layout: default
title: Blog
permalink: /blog/
---

<div class="home">

  <h1 class="post-title">Posts</h1>
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <div class="post-date">
          <span class="post-meta">{{ post.date | date: "%d %B, %Y" }}</span>
        </div>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

</div>
