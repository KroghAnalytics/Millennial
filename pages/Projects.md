---
layout: misc
title: Projects
---

Millennial is a minimalist Jekyll theme. The purpose of this theme is to provide a simple, clean, content-focused publishing platform for your publication site or blog. You can find everything you need to get started under documentation. For more information on how to install and use this theme, check out [the documentation]({{ site.github.url }}{% post_url 2016-10-10-getting-started %}).

{% for post in site.categories.sample %}
  <a href="{{ site.github.url }}{{ post.url }}">
    <div class="featured-posts" {% if post.image %}style="background-image:url({{ site.github.url }}/assets/img/{{ post.image }})"{% endif %}>
      <h2><span>{{ post.title }}</span></h2>
    </div>
  </a>
{% endfor %}
