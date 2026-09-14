---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

My research develops communication systems, network architectures, and machine learning methods for future wireless systems. I work across optical wireless communications and LiFi, AI for communications and networks, hybrid RF–optical networks, wireless sensing, and physical-layer security.

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}
{% for post in ordered_pages %}
{% include archive-single.html type="grid" %}
{% endfor %}
