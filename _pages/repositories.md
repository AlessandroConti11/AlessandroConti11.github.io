---
layout: page
permalink: /repositories/
title: repositories
description: My Github profile and my repositories.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_users %}

## GitHub users

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.liquid username=user %}
  {% endfor %}
</div>

{% endif %}

---


{% if site.data.repositories.github_repos_master_fp %} 

## GitHub Repositories of the Master's Degree Final Project

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos_master_fp %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>

{% endif %}

---


{% if site.data.repositories.github_repos_bachelor_fp %}

## GitHub Repositories of the Bachelor's Degree Final Project

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos_bachelor_fp %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>

{% endif %}

---


{% if site.data.repositories.github_repos_polimi_course %}

## GitHub Repositories of Course-Required Projects at PoliMI

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos_polimi_course %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>

{% endif %}

---


{% if site.data.repositories.github_repos_for_fun %}

## GitHub Repositories of Projects Developed For Fun

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos_for_fun %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>

{% endif %}

---
