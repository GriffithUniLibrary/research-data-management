---
title: Home
layout: default
---

# Griffith Library Workshop Template

{% include figure.html img="university-drive.jpg" alt="Students on University Drive, Gold Coast Campus" caption="University Drive" width="75%" %}

A minimal Jekyll theme with Bootstrap for creating Griffith workshop websites. Customised from Evan Will's original Workshop-Template-B to include Griffith Library author and analytics info. 

*Add your workshop abstract here!*

{% capture whatsdifferent %}
This template has been 'Griffithised' in the following ways: 

 - Library Google Analytics ID added
 - Publication year updated
 - Content author set as Griffith Uni Library
 - Griffith campus feature photo added
 - Griffith favicon added

{% include alert.html text="That's fantastic!" color="info" %}

{% endcapture %}
{% include card.html header="What's been changed?" text=whatsdifferent %}

*See also:* [workshop-template](https://evanwill.github.io/workshop-template/), original minimal version.

{% include toc.html %}

Published by [Griffith University Library](http://www.griffith.edu.au/library/), {{ site.pub_year }}.

------

{% include template/credits.html %}
