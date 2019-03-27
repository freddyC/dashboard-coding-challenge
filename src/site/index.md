---
title: Team Dash
subtitle: A place for the iFit Dashboard Team to have fun with coding challenges and making fun stuff.
layout: layouts/base.njk
---


## Challenges

The pages found in in the posts

<ul class="listing">
{%- for page in collections.post -%}
  <li>
    <a href="{{ page.url }}">{{ page.data.title }}</a> -
    <time datetime="{{ page.date }}">{{ page.date | dateDisplay("LLL d, y") }}</time>
  </li>
{%- endfor -%}
</ul>

<!-- ## Links from an external data source

These links were sourced from [hawksworx.com](https://www.hawksworx.com/feed.json) at build time.

<ul class="listing">
{%- for item in hawksworx.entries.slice(0,5) -%}
  <li>
    <a href="{{ item.link }}">{{ item.title }}</a>
  </li>
{%- endfor -%}
</ul> -->


<!-- The data can be stashed locally by running:

```
yarn run seed
```

It will then be available locally for building with:

```
yarn start
```


 -->
