---
layout: page
title: Work
permalink: /work/
---

{% for project in site.portfolio %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h2 style="font-weight: bold">{{ project.title }}</h2>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}
<br/>
<hr/>
<br/>
<span class="contacticon center">
	<a href="mailto:christine.png@mail.utoronto.ca"><i class="fa fa-envelope-square "></i></a>
	<!-- <a href="https://github.com/chspng" target="_blank"><i class="fa fa-github-square"></i></a> -->
	<a href="https://www.linkedin.com/in/christinepng/" target="_blank"><i class="fa fa-linkedin-square"></i></a>
	<!-- <a href="http://tumblr.com" target="_blank"><i class="fa fa-tumblr-square"></i></a> -->
	<!-- <a href="https://twitter.com" target="_blank"><i class="fa fa-twitter-square"></i></a> -->
</span>

<div class="col three caption">
	<!-- You can even add a little note about which of these is the best way to reach you. -->
</div>

