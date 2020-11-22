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
  <article class="monkey column is-6-desktop is-6-tablet is-12-mobile has-background-light">

    <div class=" container has-text-centered ">


<p class="is-family-serif is-size-3 has-text-primary is-marginless"> &#167;</p>
</div>
<div class="container ">
    <p class="title is-size-4 has-text-centered has-text-weight-light "><a class="has-text-weight-light has-text-grey-dark" href="{{ post.url | relative_url }}">
    {{ post.title}}</a> <br /><span class="is-size-5 is-family-sans-serif has-text-weight-medium has-text-primary"> {{ post.author }}</span></p>

    </div>

  </article>

  {% endfor %}
</div>



</div>
</div>


</section>
