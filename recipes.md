---
layout: default
title: Jekyll recipes
---

{% for recipes in site.recipes %}


<a href="{{ recipes.url | prepend: site.baseurl }}">
        <h2>{{ recipes.title }}</h2>
</a>

<p class="post-excerpt">{{ recipes.description | truncate: 160 }}</p>

{% endfor %}   