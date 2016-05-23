---
layout: post
title: Full-text search without plugins in Jekyll
categories: [tutorial]
tags: [Jekyll, search, Json]
---

Adding simple search functionality to your website can sometimes make your work more easily especially when you get more and more contents in your website. Two simple ways I found to implement search function are:

> 1. [lunr.js](http://lunrjs.com)
> 2. [Jekyll-search](https://github.com/mathaywarduk/jekyll-search)

I prefer the second ways, since [lunr.js](http://lunrjs.com) don't support Chinese search. [Jekyll-search](https://github.com/mathaywarduk/jekyll-search), however, is more flexible. It seems that it support most of the languages.

### Procedures to add search functionality

- add the following json code in your root


{% highlight html %}
{% raw %}

---
layout: null
---
{% assign first = true %}
[

{% for post in site.posts %}
    {% if post.title != null and post.title != empty %}
    {% unless first %},{% endunless %}{
        "title": {{post.title | jsonify}},
        "content": {{post.content | markdownify | strip_html | jsonify}},
        "link": "{{ site.baseurl }}{{ post.url }}",
        "date": "{{ post.date | date:"%Y-%m-%d" }}",
        "category" : "{{ post.categories | array_to_sentence_string }}" ,
        "tags": "{{ post.tags  | array_to_sentence_string }}" ,
        "search_omit": "{{ post.search_omit }}"
    }
    {% assign first = false %}
    {% endif %}
{% endfor %}

{% for page in site.pages %}
    {% if page.title != null and page.title != empty %}
    {% unless first %},{% endunless %}{
        "title": {{page.title | jsonify}},
        "content": {{page.content | strip_html | jsonify}},
        "link": "{{ site.baseurl }}{{ page.url | replace: 'index.html', '' }}",
        "date": {{ page.date | jsonify }},
        "search_omit": "{{ page.search_omit }}"
    }
    {% assign first = false %}
    {% endif %}
{% endfor %}
]

{% endraw %}
{% endhighlight %}

- add `search.js` to your js folder

- add corresponding scripts

For `lunr.js` tutorial, please refer to this [link](http://jekyll.tips/tutorials/search/)
