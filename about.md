
---
layout: default
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

<!--
	![A picture of me](/assets/pictures/Michale Gebrekiros.jpg)
-->

<img src="/assets/pictures/Michale Gebrekiros.jpg" alt="Self" style="width: 300px;"/>


Welcome to my pages! I'm Michale Gebrekiros. I have a M.Sc. in Water Resources Engineering with specialization in Engineering Hydrology and B.Sc. degree in Meteorology Science.


##  For more and getting in contact

I'm at [LinkedIn](https://www.linkedin.com/pub/michale-gebrekiros/40/412/b00)
Email: mgk169@gmail.com
