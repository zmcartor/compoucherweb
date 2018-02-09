---
title : blah
---
<!DOCTYPE html>
<html lang="en">
<head>
  <title>{{ site.env}}</title>
<meta name="description" content="Compoucher, Zach McArtor digital products">
  <meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=Edge">
<meta name="author" content="@zmcartor">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://unpkg.com/tachyons/css/tachyons.min.css">
</head>
<body class="w-100 sans-serif bg-white">
  <header class="cf ph3 ph5-ns pv3 w-50-ns pr4-ns">
    <h1 class="mt2 lh-title fw9 f2">{{ page.title }}</h1>
  
    {% include nav.html %}

  </header>
 {{ content }}
 <footer class="pv4 ph3 ph5-m ph6-l mid-gray cb">
  <small class="f6 db tc">© All the years <b class="ttu">Compoucher LLC</b></small>
  <div class="tc mt3">
    <a href="/terms.html"   title="Terms" class="f6 dib ph2 link mid-gray dim">Terms of Use</a>
    <a href="/privacy.html"  title="Privacy" class="f6 dib ph2 link mid-gray dim">Privacy</a>
  </div>
</footer>
</body>
</html>
