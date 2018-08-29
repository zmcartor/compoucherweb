---
title : blah
---
<!DOCTYPE html>
<html lang="en">
<head>
  <title>{{ page.title }}</title>
<meta name="description" content="Compoucher, Zach McArtor digital products">
  <meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=Edge">
<meta name="author" content="@zmcartor">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://unpkg.com/tachyons/css/tachyons.min.css">

 <!-- Google Analytics -->
    <script>
    (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
    (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
    m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
    })(window,document,'script','https://www.google-analytics.com/analytics.js','ga');

    ga('create', 'UA-113909515-1', 'auto');
	ga('send', 'pageview', { 'page': location.pathname + location.search + location.hash});
	ga('set', 'anonymizeIp', false);
    </script>
    <!-- End Google Analytics -->

{% include css-fonts.css %}

</head>
<body class="w-100 sans-serif bg-white">
  <header class="cf ph3 ph5-ns pv3 w-50-ns pr4-ns">
    {% include nav.html %}
  </header>
 
 <article class="pa3 pa5-ns lh-copy">
  <h4 class="f2 f-subheadline-l lh-solid">{{ page.title }}</h4>
  <p class="measure lh-copy">
    {{ content }}
  </p>
</article>

 
 <footer class="pv4 ph3 ph5-m ph6-l mid-gray cb">
  <small class="f6 db tc">© All the years <b class="ttu">Compoucher LLC</b></small>
  <div class="tc mt3">
    <a href="/terms.html"    title="Terms" class="f6 dib ph2 link mid-gray dim">Terms of Use</a>
    <a href="/privacy.html"  title="Privacy" class="f6 dib ph2 link mid-gray dim">Privacy</a>
  </div>
</footer>
</body>
</html>
