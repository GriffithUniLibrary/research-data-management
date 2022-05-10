---
title:Library resources
nav: true
---

The management of research data is an integral part of good research practice that allows reliable verification of results, protects the intellectual and financial investment made in its creation which enables it to be shared (if possible) potentially generating new and innovative research.

Good data management practice will ensure compliance to government research codes and principles that underpin Australian research.   


![image](https://user-images.githubusercontent.com/42364968/165414539-b6d2f326-3efc-429a-9d0a-bca05315e2c5.png)

{% comment %}

    Bootstrap Card, https://getbootstrap.com/docs/4.5/components/card/

    e.g. --> {% include card.html text="Some interesting text" header="Example card" %}
    
    Options:
    - "text" = main card text, can use markdown formatting. Use a Liquid capture to add more complex content.
    - "header" = card header text (in bar above card content)
    - "title" = card title text inside card content area
    - "img" = give filename of image in your "images" folder, will create a card cap image
    - "alt" = alt text for image
    - "width" = will use responsive sizing to set the % size on desktop (will be 100% on mobile), choose from "25", "50", "75", or "100"
    - "float"  = will use responsive float utility to add float on desktop (will not float on mobile), choose from "left" or "right"
    - "centered" = give "true" to add mx-auto class on the card to center it (don't use with float!)

{%- endcomment -%}
<div class="card mb-3{% if include.float %} feature-float-{{ include.float }}{% endif %}{% if include.width %} feature-w-{{ include.width }}{% endif %}{% if include.centered %} mx-auto{% endif %}">
{% if include.img %}<img class="card-img-top" src="{{ '/images/' | append: include.img | relative_url }}" alt="{{ include.alt | default: 'Card image' }}">{% endif %}
{% if include.header %}<h5 class="card-header">{{ include.header }}</h5>{% endif %}
<div class="card-body">
{% if include.title %}<h5 class="card-title">{{ include.title }}</h5>{% endif %}
<div class="card-text">
{{ include.text | markdownify }}
</div>
</div>
</div>

### Why?

Rather than making slides for a workshop, why not make a website? 
It's easier to write, access, share, and reuse. 
GitHub and GitHub Pages makes this pretty easy.

It is a better [Open Educational Resource](https://en.wikipedia.org/wiki/Open_educational_resources) since anyone can make a copy and adapt!

## GitHub Pages 

One amazingly useful GitHub feature is [GitHub Pages](https://guides.github.com/features/pages/).
It provides free static web hosting from any repository.
Gh-pages is intended to host relatively simple sites for your GitHub portfolio, project, or documentation.
Because it is free and a valuable transferable skill, this is a great option for teaching and learning.

Many organizations are using GitHub to collaboratively create and publish public workshop websites. 
For example: 

- [Programming Historian](http://programminghistorian.org/)
- [Software Carpentry](https://software-carpentry.org/), [Data Carpentry](http://www.datacarpentry.org/), [Library Carpentry](https://librarycarpentry.org/)
- this site!

{% capture text %}Note:
There are *soft* limits and guidelines for gh-pages usage: sites should be < 1GB, use < 100GB bandwidth per month, and make < 10 builds per hour.
If your site exceeds these quotas, GitHub will send you a notice asking you to modify the repository.
All content must follow the [community guidelines](https://help.github.com/articles/github-community-guidelines/), e.g. no violence, obscene sex, or illegal stuff.{% endcapture %}
{% include alert.html text=text color=secondary %}
