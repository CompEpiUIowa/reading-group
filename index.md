---
layout: home
title: Just the Class
nav_exclude: true
seo:
  type: Course
  name: Just the Class
---

# {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

{% if site.announcements %}
{{ site.announcements.last }}
[Announcements](announcements.md){: .btn .btn-outline .fs-3 }
{% endif %}

## About the reading group

In this reading group, we meet weekly to discuss techniques from algorithms, data mining, and machine learning that can be applied to problems related to the spread of infections. Our plan is to study a mixture of the latest papers and tutorial-style material on methods that could be useful to us. For example, one week we might study a paper from ICML 2021 and the next two weeks we might run a tutorial on submodular function optimization.

