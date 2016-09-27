---
layout: page
title: Results
permalink: /results/
---

<p>Below are links to the failure reports of the 25 subject web pages in our most recent study.</p>
  <ul class="post-list">
    {% for post in site.posts reversed %}
      <li>
        <!-- <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span> -->
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>