---
layout: default
title: Blog
permalink: /blog/
---
<section>

<div class="columns is-multiline is-centered m-4">

{% for post in site.posts %}

<div class="column is-one-third">

 <article class="post">

    <header class="titles">
    <h2 class="title has-text-centered"><a class="post-link has-text-weight-light is-size-4" href="{{ post.url | relative_url }}">
    {{ post.title | escape }}
    </a>
    </h2>
    </header>

    <div class="post-content">
    {{ post.excerpt }}
    </div>

</article>

</div>
{% endfor %}
</div>


</section>
