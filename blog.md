---
layout: default
posts_category: blog
title:  "Blog"
group: navigation
order: 15
---

<h1><img src="/assets/traffic-cone.png" width="24px" height="auto" class="img-fluid rounded" alt="traffic cone"><span class="ps-2">Blog under Construction</span></h1>

<p class="mt-5 mb-5"><button type="button" class="btn btn-outline-primary btn-sm position-relative">
  Upcoming Posts
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
    3+
    <span class="visually-hidden">upcoming posts</span>
  </span>
</button></p>

{% for teaser in site.data.teasers %}
<h2 class="mb-1" style="text-transform: none;"><span class="me-2"><a href="#">{{ teaser.title }}</a></span><small><span class="badge rounded-pill text-bg-primary px-2 me-1 align-top" style="line-height: 1.2; margin-top: 1.5pt;"><a class="link-light" href="#">{{ teaser.tag | prepend: '#' }}</a></span></small></h2>
<p class="mb-3"><small class="text-body-secondary" style="font-style: italic;">Forthcoming</small></p>
<p style="margin-bottom: 1.85rem;">{{ teaser.punchline }}</p>
{% endfor %}

<!--
{%- if site.tags.pinned -%}
{%- include posts_list.html tag = "pinned" -%}
{%- endif -%}

{%- include posts_list.html -%}
-->

<div class="fixed-bottom" style="margin-top:3rem;"><iframe align="right" width="225" height="225" scrolling="no" frameborder="no" allow="autoplay; encrypted-media" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/soundcloud%253Atracks%253A2106661458&color=%23cc000f&auto_play=true&hide_related=true&show_comments=true&show_user=true&show_reposts=false&show_teaser=false&visual=true"></iframe></div>

<!--
<script type="module" src="https://cdn.jsdelivr.net/npm/bsky-embed/dist/bsky-embed.es.js" async></script>
  <bsky-embed
    username="not.dingherself.com"
    mode="system"
    custom-styles=".max-w-screen-sm { max-width: 300px !important; float: right; font-size: 0.825rem; line-height: 1.325; }"
    limit="3"
    disable-autoplay="true"
  >
  </bsky-embed>
  -->