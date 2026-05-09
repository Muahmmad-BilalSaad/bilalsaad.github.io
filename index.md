---
layout: default
title: Home
---

<div class="hero">
  <div class="hero-tag">Available for Work</div>
  <h1>Muhammad<br><em>Bilal Saad.</em></h1>
  <p>Web Developer & University Student from Pakistan. I build clean, fast websites and share my journey through writing.</p>
  <div class="hero-btns">
    <a href="/about" class="btn btn-primary">About Me →</a>
    <a href="/contact" class="btn btn-outline">Contact</a>
  </div>
  <div class="hero-stats">
    <div>
      <div class="stat-num">15<span>+</span></div>
      <div class="stat-label">Projects</div>
    </div>
    <div>
      <div class="stat-num">2<span>+</span></div>
      <div class="stat-label">Years Exp.</div>
    </div>
    <div>
      <div class="stat-num">10<span>+</span></div>
      <div class="stat-label">Clients</div>
    </div>
  </div>
</div>

<div class="section-label">Latest Posts</div>
<h2>From the Blog</h2>

<div class="posts-list">
  {% for post in site.posts %}
  <a class="post-item" href="{{ post.url | relative_url }}">
    <div>
      <div class="post-item-title">{{ post.title }}</div>
      <div class="post-excerpt">{{ post.excerpt | strip_html | truncate: 100 }}</div>
    </div>
    <div class="post-item-date">{{ post.date | date: "%b %d, %Y" }}</div>
  </a>
  {% endfor %}
</div>
