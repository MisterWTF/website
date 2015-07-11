---
layout: home
headline: Answering your digital WTF's
title: Sahil Saini - Answering your digital WTF's
excerpt: "A simple and clean responsive Jekyll theme for words and photos."
search_omit: true
image:
  feature: 'sahil.png'
---

##People ask me questions, I answer them and then I write about everything. I do this to save my time and yours. I am just a helpful fucking soul.  

{% include mailchimp.html %}

## Latest Posts

<ul class="post-list">
{% for post in site.posts limit:3 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
