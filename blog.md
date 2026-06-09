---
layout: default
posts_category: blog
title:  "Blog, or: I Have Things to Say But Don’t Want a Substack"
group: navigation
order: 15
---

<style>
div.rss:hover {cursor: pointer;}
div.rss > svg {fill: var(--bs-link-color);}
div.rss > span {color: var(--bs-link-color);}
div.rss:hover > svg {fill: var(--bs-link-hover-color);}
div.rss:hover > span {color: var(--bs-link-hover-color);}
</style>

<!--
<h1 class="mb-5"><img src="/assets/bookshelf.png" width="24px" height="auto" class="img-fluid rounded" alt="pixelated icon of a bookshelf"><span class="ps-2">Blog, or: I Have Things to Say But Don’t Want a Substack</span><div class="rss float-end" title="RSS" onclick="window.open('https://dingherself.com/feed.xml');"><span class="fs-6 pe-1">RSS</span><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-rss" viewBox="0 0 16 16"><path d="M14 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1zM2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2z"/><path d="M5.5 12a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0m-3-8.5a1 1 0 0 1 1-1c5.523 0 10 4.477 10 10a1 1 0 1 1-2 0 8 8 0 0 0-8-8 1 1 0 0 1-1-1m0 4a1 1 0 0 1 1-1 6 6 0 0 1 6 6 1 1 0 1 1-2 0 4 4 0 0 0-4-4 1 1 0 0 1-1-1"/></svg></div></h1>
-->

<h1><img src="/assets/traffic-cone.png" width="24px" height="auto" class="img-fluid rounded" alt="traffic cone"><span class="ps-2">Blog in Progress, or: I Have Things to Say But Don’t Want a Substack</span><div class="rss float-end" title="RSS" onclick="window.open('https://dingherself.com/feed.xml');"><span class="fs-6 pe-1">RSS</span><svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-rss" viewBox="0 0 16 16"><path d="M14 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1zM2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2z"/><path d="M5.5 12a1.5 1.5 0 1 1-3 0 1.5 1.5 0 0 1 3 0m-3-8.5a1 1 0 0 1 1-1c5.523 0 10 4.477 10 10a1 1 0 1 1-2 0 8 8 0 0 0-8-8 1 1 0 0 1-1-1m0 4a1 1 0 0 1 1-1 6 6 0 0 1 6 6 1 1 0 1 1-2 0 4 4 0 0 0-4-4 1 1 0 0 1-1-1"/></svg></div></h1>

<p class="fst-italic">Remember when we just wrote <a href="https://raw.githubusercontent.com/radtransfem/radtransfem.github.io/refs/heads/master/blog.md">our own <span class="sc">HTML</span> code</a>? The good ol’ days.</p>

<p style="margin-top: 1.25rem; margin-bottom: 1.75rem;"><button type="button" class="btn btn-outline-primary btn-sm position-relative" data-bs-toggle="modal" data-bs-target="#teaserModal">
  Upcoming Posts
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
    4+
    <span class="visually-hidden">upcoming posts</span>
  </span>
</button></p>

<!-- Modal -->
<div class="modal fade" id="teaserModal" tabindex="-1" aria-labelledby="teaserModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h1 class="modal-title fs-3" id="teaserModalLabel">Surprising no one, this turned out to be more of a summer project than an end-of-semester distraction</h1>
        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
      </div>
      <div class="modal-body">
        <p style="fs-4">Check back later! Nudge me if you have to!!</p>
      </div>
      <div class="modal-footer">
        <a href="https://dingherself.com/feed.xml" type="button" class="btn btn-primary btm-sm" role="button">Copy RSS Link</a>
        <button type="button" class="btn btn-outline-secondary btm-sm " data-bs-dismiss="modal">Close</button>
      </div>
    </div>
  </div>
</div>


{% for teaser in site.data.teasers %}
<h2 class="mb-1" style="text-transform: none;"><span class="me-2">{{ teaser.title }}</span><small><span class="badge rounded-pill text-bg-primary px-2 me-1 align-top" style="line-height: 1.2; margin-top: 1.5pt;"><a class="link-light" href="#">{{ teaser.tag | prepend: '#' }}</a></span></small></h2>
<p class="mb-3"><small class="text-body-secondary" style="font-style: italic;">Forthcoming</small></p>
<p style="margin-bottom: 1.85rem;">{{ teaser.punchline }}</p>
{% endfor %}

<!--
{%- if site.tags.pinned -%}
{%- include posts_list.html tag = "pinned" -%}
{%- endif -%}

{%- include posts_list.html -%}
-->

<div style="margin-bottom: 10rem;"></div>

<div class="fixed-bottom"><iframe align="right" width="225" height="225" scrolling="no" frameborder="no" allow="autoplay; encrypted-media" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/soundcloud%253Atracks%253A2106661458&color=%23cc000f&auto_play=true&hide_related=true&show_comments=true&show_user=true&show_reposts=false&show_teaser=false&visual=true"></iframe></div>

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
