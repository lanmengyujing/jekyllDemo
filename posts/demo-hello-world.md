---
layout: default
title: Jekyll Demo
---

## Usage
RUI has been written in a modular way so that you can just use the pieces you want, or grab it all in one request.

We also provide some combined packages that could be handy in different situations:

- [**rui-all.css**](../css/rui-all.css): Great for new projects who just want one file to rule them all.
- [**rui-font-and-icons.css**](../css/rui-font-and-icons.css): Used more by existing projects (think DS) who aren't quite ready for the full RUI greatness.

Original and a minified versions are supplied for each CSS file.

## How do I get this RUI goodness?
### CDN
Using the REA CDN to directly link to the files you need (recommended)

#### Just give it to me!
{% highlight html %}
<link rel="stylesheet" type="text/css" href="http://s1.rui.au.reastatic.net/rui-0.2.3-187/css/rui-all.min.css">
<script src="http://s1.rui.au.reastatic.net/rui-0.2.3-187/js/rui-all.min.js"></script>
{% endhighlight %}

#### Actually I want to cherry pick components...
Just change the extension to **.min.js** if you want that!
{% highlight html %}
<link rel="stylesheet" type="text/css" href="http://s1.rui.au.reastatic.net/rui-0.2.3-187/css/rui-advertorial.css">
<script src="http://s1.rui.au.reastatic.net/rui-0.2.3-187/js/rui-advertorial.js"></script>
{% endhighlight %}

## RUI Components
<dl class="list-rui">
{% for page in site.pages %}
    {% if page.include_in_toc %}
    <dt><a href=".{{ page.url }}">{{ page.title }}</a></dt>
    <dd>{{ page.description }}</dd>
    {% endif %}
{% endfor %}
</dl>

