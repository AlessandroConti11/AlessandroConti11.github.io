---
layout: page
permalink: /skills/
title: skills
description: The programming languages, frameworks, applications, and operating systems I know how to use.
nav: true
nav_order: 4
---

{% if site.data.skills.programming_language %}

## Programming Language
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for skill in site.data.skills.programming_language %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>

{% endif %}

---

## Framework

---

## Applications

---

## Operating System

---
