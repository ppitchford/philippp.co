---
layout: default
title: Home
id: home
redirect_from: "/en"
permalink: /
---

<div>
  <div>
    <h1 style="margin: 1em 0 0;">
      Philipp Pitchford
    </h1>

    <p>
      Welcome! I'm Philipp, a Boston-based program manager working at <a target="blank" rel="noopener" href="https://www.pennfoster.edu/">Penn Foster</a>. I care about empowering teams and building products that improve education at scale. Areas of interest include data, productivity, product development, and sustainability.
    </p>

    <p>
      I recently started a newsletter on Substack named <a title="Culinary Notes" rel="noopener" target="blank" href="https://culinarynotes.substack.com/">Culinary Notes</a>, where I write about history of food, one dish at a time.
    </p>
    <p>
      I'm active on <a title="LinkedIn" rel="noopener" target="blank" href="https://www.linkedin.com/in/philipppitchford/">LinkedIn</a> and <a title="Twitter" rel="noopener" target="blank" href="https://twitter.com/plpitchford">Twitter</a> — feel free to connect, follow, or message me there.
    </p>
    <p>
      While you're here, consider taking a few minutes to <a href="/guestbook" class="internal-link">sign the guestbook</a>.
    </p>
  </div>

  <div>
    <div class="grid-element">
      <h2>Blog posts</h2>
      {% assign post_limit = 7 %}
      {% for post in site.posts limit: post_limit %}
      <div class="list-entry">
        <div><a class="internal-link" href="{{ post.url }}">{{ post.title }}</a> <span class="faded">({{ post.date | date: "%Y-%m-%d" }})</span></div>
        <div>{{ post.excerpt }}</div>
      </div>
      {% endfor %}
      <p>
        <a class="internal-link" href="/blog">I wrote {{ site.posts.size | minus: post_limit }} more posts</a>.
        This blog is also available as <a class="internal-link" target="_blank" href="/rss.xml">RSS</a> and <a class="internal-link" target="_blank" href="/feed.json">JSON</a> feeds.
      </p>
    </div>
  </div>
</div>
