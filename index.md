---
layout: default
title: Home
---


# Welcome to My Jekyll Site

<div class="hero">
  <img src="{{ site.baseurl }}/assets/images/hero-image.jpg" alt="Hero Image">
</div>

<div class="intro">
  <h1>Welcome to My Jekyll Site</h1>
  <p>This is a sample Jekyll site.</p>
</div>

<div class="latest-posts">
  <h2>Latest Posts</h2>
  <ul>
    {% for post in site.posts limit:3 %}
      <li>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
        <span>{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  </ul>
</div>
