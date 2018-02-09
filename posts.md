---
title : All Posts
layout : page
---

<section class="mw8 ph3 ph5-ns">
  <h2 class="f2 ph3 ph0-l">Latest</h2>
  
  <article class="pv4 bt bb b--black-10 ph3 ph0-l">
    <a href="{{ site.posts[0].url }}" class="dim pointer link black">
    <div class="flex flex-column flex-row-ns">
      <div class="w-100 w-60-ns pr3-ns order-2 order-1-ns">
        <h1 class="f3 mt0 lh-title"> {{ site.posts[0].title }} </h1>
        <p class="f5 f4-l lh-copy">
         {{ site.posts[0].description }}
        </p>
      </div>
      <div class="pl3-ns order-1 order-2-ns mb4 mb0-ns w-100 w-40-ns">
       <img src="/images/{{ site.posts[0].image }}" alt="post image" class="db">
      </div>
    </div>
    </a>
    <time class="f6 db gray">{{ site.posts[0].pubDate }}</time>
  </article>

   <article class="pv4 bt bb b--black-10 ph3 ph0-l">
    <a href="{{ site.posts[1].url }}" class="dim pointer link black">

    <div class="flex flex-column flex-row-ns">
      <div class="w-100 w-60-ns pr3-ns order-2 order-1-ns">
        <h1 class="f3 mt0 lh-title"> {{ site.posts[1].title }}</h1>
        <p class="f5 f4-l lh-copy">
         {{ site.posts[1].description }}
        </p>
      </div>
      <div class="pl3-ns order-1 order-2-ns mb4 mb0-ns w-100 w-40-ns">
       <img src="/images/{{ site.posts[1].image }}" alt="post image" class="db">
      </div>
    </div>
    </a>
    <time class="f6 db gray">{{ site.posts[1].pubDate }}</time>
  </article>

</section>


<section class="mw8 ph3 ph5-ns mt6">
  <h2 class="f2 ph3 ph0-l">The Rest</h2>
{% for post in site.posts offset:3 %}
 <article class="pv4 bt bb b--black-10 ph3 ph0-l">
  <a href="{{post.url }}" class="dim pointer link black">
    <div class="flex flex-column flex-row-ns"> 
      <div class="w-100 w-60-ns pr3-ns order-2 order-1-ns">
        <h1 class="f3 mt0 lh-title"> {{ post.title }} </h1>
        <p class="f5 f4-l lh-copy">
         {{ post.description }}
        </p>
      </div>
      <div class="pl3-ns order-1 order-2-ns mb4 mb0-ns w-100 w-40-ns">
       <img src="/images/{{ post.image }}" alt="post image" class="db">
      </div>
    </div>
    </a>
    <time class="f6 db gray">{{ post.pubDate }}</time>
  </article>
 
 {% endfor %}
</section>
