---
layout: page
title: Hello World!
tagline: Supporting tagline
---
{% include JB/setup %}

## Update Author Attributes

In `_config.yml` remember to specify your own data:
	title : My Blog =)
	
	author :
	  name : Name Lastname
	  email : blah@email.test
	  github : username
	  twitter : username


<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
