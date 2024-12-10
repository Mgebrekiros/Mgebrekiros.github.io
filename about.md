---
layout: default
title: "About Me"
permalink: /aboutme/
tags: [about, bio, personal]
---

<div class="post">
  <h1 class="post-title">{{ page.title }}</h1>
  <span class="post-date">{{ page.date | date_to_string }}</span>
  {{ content }}
</div>

<div class="related">
  <h2>Related Posts</h2>
  <ul class="related-posts">
    {% assign current_tags = page.tags %}
    {% for post in site.posts %}
      {% if (post.tags | intersection: current_tags).size > 0 and post.url != page.url %}
        <li>
          <h3>
            <a href="{{ post.url }}">
              {{ post.title }}
              <small>{{ post.date | date_to_string }}</small>
            </a>
          </h3>
        </li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

<!-- Optional image using Markdown (if you prefer this over HTML): -->
![A picture of me](/assets/pictures/Michale_Gebrekiros.jpg)

<!-- Inline image with styling (if you prefer HTML): -->
<img src="/assets/pictures/Michale_Gebrekiros.jpg" alt="Self" class="profile-image"/>

## About Me

Welcome to my pages! I'm Michale Gebrekiros. I have a M.Sc. in Water Resources Engineering with specialization in Engineering Hydrology and a B.Sc. degree in Meteorology Science.

## For More and Getting in Contact

You can find me on [LinkedIn](https://www.linkedin.com/pub/michale-gebrekiros/40/412/b00) or email me at [mgk169@gmail.com](mailto:mgk169@gmail.com).
