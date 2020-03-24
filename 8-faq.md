---
layout: default
title: FAQ
description: FAQ
css-add: accordion
---

**FAQ**. This is the list of the most frequently asked questions.

<section class="faq">
	{% for item in site.faq %}
	  <button class="accordion">{{ item.description }}</button>
	  <div class="panel">
	    {{ item.content | markdownify }}
	  </div>
	{% endfor %}
</section>
