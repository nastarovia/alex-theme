---
layout: default
title: Blog
permalink: /blog/
---
<section>

<div class="columns is-centered m-4">
<div class="column is-8 is-centered ">


<div class="columns is-centered is-multiline">


{% for post in site.posts %}
  <article class="column is-6-desktop is-6-tablet is-1-mobile">

    <div class="content has-text-centered">

    <p class="title is-size-4 has-text-centered has-text-weight-light "><a class="has-text-weight-light has-text-grey-dark" href="{{ post.url | relative_url }}">
    {{ post.title}}</a> <br /><span class="is-size-6 is-family-sans-serif has-text-weight-bold has-text-primary"> {{ post.author }}</span></p>
    </div>
<hr />
  </article>

  {% endfor %}
</div>



</div>
</div>


</section>
