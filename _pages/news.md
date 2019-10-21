---
layout: archive
title: "News"
permalink: /news/
# author_profile: true
---

{% include base_path %}


<!-- <h2>Publications</h2>
 {% for post in site.pages %}
  {% include archive-single.html %}
{% endfor %} 
{% for post in site.publications limit:2 reversed %}
  {% include archive-single.html %}
{% endfor %}

<h2>Attendance and Talks</h2>
{% for post in site.talks limit:2 reversed %}
  {% include archive-single.html %}
{% endfor %} -->

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
{% unless collection.output == false or collection.label == "posts" %}
  {% capture label %}{{ collection.label }}{% endcapture %}
  {% if label != written_label %}
  <!-- <h1>{{ label }}</h1> -->
  {% capture written_label %}{{ label }}{% endcapture %}
  {% endif %}
{% endunless %}
{% for post in collection.docs limit:2 reversed %}
  {% unless collection.output == false or collection.label == "posts" %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
{% endfor %}
