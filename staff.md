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

{% assign former_student = site.staffers | where: 'role', 'former_student' %}
{% assign num_former_student = former_student | size %}
{% if num_former_student != 0 %}

## Former Students

{% for staffer in former_student %}
{{ staffer }}
{% endfor %}
{% endif %}
