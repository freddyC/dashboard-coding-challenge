---
layout: layouts/base.njk
pageClass: challenges
templateEngineOverride: njk, md
---
<p class="date">
  Posted on <time datetime="{{ date }}">{{ date | dateDisplay }}</time>
</p>
<main>
  {{ content | safe }}
</main>