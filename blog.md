---
layout: default
posts_category: blog
title:  "Blog"
group: navigation
order: 15
---

<style>
#share-buttons {display: inline-block; vertical-align: middle; }
#share-buttons:after {content: ""; display: block; clear: both;}
#share-buttons > div {
    position: relative;
    text-align: left; 
    height: 36px; 
    width: 25px; 
    float: left; 
    text-align: center;
}
div.rss:hover {cursor: pointer;}
div.rss > svg {fill: var(--bs-link-color);}
div.rss:hover > svg {fill: var(--bs-link-hover-color);}
</style>

<h1 class="mb-5"><img src="/assets/bookshelf.png" width="24px" height="auto" class="img-fluid rounded" alt="pixelated icon of a bookshelf"><span class="ps-2">Blog</span><div class="rss float-end" title="RSS" onclick="window.open('https://dingherself.com/feed.xml');"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"  width="24" height="24"><!--!Font Awesome Free v7.2.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free Copyright 2026 Fonticons, Inc.--><path d="M64 32C28.7 32 0 60.7 0 96L0 416c0 35.3 28.7 64 64 64l320 0c35.3 0 64-28.7 64-64l0-320c0-35.3-28.7-64-64-64L64 32zM96 136c0-13.3 10.7-24 24-24 137 0 248 111 248 248 0 13.3-10.7 24-24 24s-24-10.7-24-24c0-110.5-89.5-200-200-200-13.3 0-24-10.7-24-24zm0 96c0-13.3 10.7-24 24-24 83.9 0 152 68.1 152 152 0 13.3-10.7 24-24 24s-24-10.7-24-24c0-57.4-46.6-104-104-104-13.3 0-24-10.7-24-24zm0 120a32 32 0 1 1 64 0 32 32 0 1 1 -64 0z"/></svg></div></h1>

{%- if site.tags.pinned -%}
{%- include posts_list.html tag = "pinned" -%}
{%- endif -%}

{%- include posts_list.html -%}

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