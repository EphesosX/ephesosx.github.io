---
layout: page
title: Teaching
published: true
---

###### Current Courses
{% for course in site.teaching reversed %}
{% if course.layout == 'course_info' %}
{% if course.quarter == site.quarter %}

* [{% include course_listing.md %}]({{ site.baseurl }}{{ course.url }})
{% endif %}

{% endif %}
{% endfor %}

###### Past Courses
{% for course in site.teaching reversed %}
{% if course.quarter != site.quarter %}
{% if course.layout == 'course_info' %}

* {% include course_listing.md %}

{% endif %}
{% endif %}
{% endfor %}

PIC 10B: Intermediate Programming (F'16) <br>
Math 151B: Applied Numerical Analysis (S'17, S'18) <br>
PIC 10A: Introduction to Programming (W'18, S'18) <br>
PIC 16: Python with Applications (F'17, W'18) <br>
PIC 40A: Introduction to Programming for Internet (F'18)
