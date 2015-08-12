---
layout: home
headline: Answering your digital WTF's
title: Sahil Saini - Answering your digital WTF's
excerpt: "A simple and clean responsive Jekyll theme for words and photos."
search_omit: true
image:
  feature: 'sahil.png'
---

<div class="home-welcome">
	<p class="home-text">My name is Sahil. Some days I am a developer, some a web consultant, but most days I am a digital messiah, bearing the weight of saving you from daily digital What The F#@ks. </p>
</div>
<div class="home-sahil">
	<img src="{{ site.url }}/images/{{ page.image.feature }}" class="entry-feature-image" alt="{{ page.title }}" style="margin-top:0;">
</div>

<div class="clear"></div>

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur rem, quaerat accusantium doloremque ut, voluptate corporis molestiae similique praesentium sunt animi natus esse unde eius neque obcaecati eaque, voluptates fuga.

<p><a class="btn askwtf" href="/contact">Ask Me</a></p>

{% include mailchimp.html %}

## Latest Articles

<ul class="post-list">
{% for post in site.posts limit:3 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
