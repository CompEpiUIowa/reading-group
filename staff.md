---
layout: page
title: Members
description: Members of the reading group
---

# Members

<!--Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.-->

## Professors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign student = site.staffers | where: 'role', 'student' %}
{% assign num_student = student | size %}
{% if num_student != 0 %}

## Students

{% for staffer in student %}
{{ staffer }}
{% endfor %}
{% endif %}
