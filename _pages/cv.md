---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

{% assign cv_experience = site.data.cv.experience %}
{% assign cv_education = site.data.cv.education %}
<!-- {% assign cv_projects = site.data.cv.projects %} -->
{% assign cv_skills = site.data.cv.skills %}
<!-- {% assign cv_recognitions = site.data.cv.recognitions %} -->
{% assign cv_associations = site.data.cv.associations %}
<!-- {% assign cv_interests = site.data.cv.interests %} -->
<!-- {% assign cv_links = site.data.cv.links %} -->

{% if cv_education and cv_education.size > 0 %}
<h2 class="cv-section-heading">Education</h2>

<div class="cv-section">
  <ul class="cv-list">
    {% for education in cv_education %}
    <li class="cv-item">
      <div class="cv-item-top-block">
        {% if education.image %}
        <img src="{{ base_path }}{{ education.image }}" alt="{{ education.image_alt | default: education.uni }}" class="cv-item-image">
        {% endif %}
        <div class="cv-item-body">
          <div class="cv-item-header">
            <div class="cv-item-title">{{ education.uni }}</div>
            <div class="cv-item-date">{{ education.year }}</div>
          </div>
          <div class="cv-item-subtitle">{{ education.degree }}</div>
        </div>
      </div>
      {% if education.award %}
      <div class="cv-item-summary">{{ education.award | markdownify }}</div>
      {% endif %}
      {% if education.awards and education.awards.size > 0 %}
      <ul class="cv-item-highlights">
        {% for award in education.awards %}
        <li>{{ award.award }}</li>
        {% endfor %}
      </ul>
      {% endif %}
      {% if education.summary %}
      <div class="cv-item-summary">{{ education.summary | markdownify }}</div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

{% if cv_experience and cv_experience.size > 0 %}
<h2 class="cv-section-heading">Experience</h2>

<div class="cv-section">
  <ul class="cv-list">
    {% for job in cv_experience %}
    <li class="cv-item">
      <div class="cv-item-top-block">
        {% if job.image %}
        <img src="{{ base_path }}{{ job.image }}" alt="{{ job.image_alt | default: job.company }}" class="cv-item-image">
        {% endif %}
        <div class="cv-item-body">
          <div class="cv-item-header">
            <div class="cv-item-title">{{ job.company }}</div>
            <div class="cv-item-date">{{ job.duration }}</div>
          </div>
          <div class="cv-item-subtitle">{{ job.position }}</div>
        </div>
      </div>
      {% if job.summary %}
      <div class="cv-item-summary">{{ job.summary | markdownify }}</div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

<!--
{% if cv_projects and cv_projects.size > 0 %}
<h2 class="cv-section-heading">Projects</h2>

<div class="cv-section">
  <ul class="cv-list">
    {% for project in cv_projects %}
    <li class="cv-item">
      <div class="cv-item-top-block">
        {% if project.image %}
        <img src="{{ base_path }}{{ project.image }}" alt="{{ project.image_alt | default: project.project }}" class="cv-item-image">
        {% endif %}
        <div class="cv-item-body">
          <div class="cv-item-header">
            <div class="cv-item-title">
              {% if project.url %}<a href="{{ project.url }}">{{ project.project }}</a>{% else %}{{ project.project }}{% endif %}
            </div>
            <div class="cv-item-date">{{ project.duration }}</div>
          </div>
          <div class="cv-item-subtitle">{{ project.role }}</div>
        </div>
      </div>
      {% if project.description %}
      <div class="cv-item-summary">{{ project.description | markdownify }}</div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %} -->

{% if cv_skills and cv_skills.size > 0 %}
<h2 class="cv-section-heading">Skills</h2>

<div class="cv-section">
  {% for skill in cv_skills %}
    {% if skill.keywords %}
    <div class="cv-item-summary">{{ skill.keywords | markdownify }}</div>
    {% endif %}
  {% endfor %}
</div>
{% endif %}
<!--
{% if cv_recognitions and cv_recognitions.size > 0 %}
<h2 class="cv-section-heading">Recognition</h2>

<div class="cv-section">
  <ul class="cv-list">
    {% for recognition in cv_recognitions %}
    <li class="cv-item">
      <div class="cv-item-top-block">
        {% if recognition.image %}
        <img src="{{ base_path }}{{ recognition.image }}" alt="{{ recognition.image_alt | default: recognition.award }}" class="cv-item-image">
        {% endif %}
        <div class="cv-item-body">
          <div class="cv-item-header">
            <div class="cv-item-title">{{ recognition.award }}</div>
            <div class="cv-item-date">{{ recognition.year }}</div>
          </div>
          <div class="cv-item-subtitle">{{ recognition.organization }}</div>
        </div>
      </div>
      {% if recognition.summary %}
      <div class="cv-item-summary">{{ recognition.summary | markdownify }}</div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %} -->

{% if cv_associations and cv_associations.size > 0 %}
<h2 class="cv-section-heading">Associations</h2>

<div class="cv-section">
  <ul class="cv-list">
    {% for association in cv_associations %}
    <li class="cv-item">
      <div class="cv-item-top-block">
        {% if association.image %}
        <img src="{{ base_path }}{{ association.image }}" alt="{{ association.image_alt | default: association.organization }}" class="cv-item-image">
        {% endif %}
        <div class="cv-item-body">
          <div class="cv-item-header">
            <div class="cv-item-title">
              {% if association.url %}<a href="{{ association.url }}">{{ association.organization }}</a>{% else %}{{ association.organization }}{% endif %}
            </div>
            <div class="cv-item-date">{{ association.year }}</div>
          </div>
          <div class="cv-item-subtitle">{{ association.role }}</div>
        </div>
      </div>
      {% if association.summary %}
      <div class="cv-item-summary">{{ association.summary | markdownify }}</div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}
<!--
{% if cv_interests and cv_interests.size > 0 %}
<h2 class="cv-section-heading">Outside Interests</h2>

<div class="cv-section">
  <ul class="cv-item-highlights">
    {% for interest in cv_interests %}
    <li>{{ interest.description }}</li>
    {% endfor %}
  </ul>
</div>
{% endif %}

{% if cv_links and cv_links.size > 0 %}
<h2 class="cv-section-heading">Additional Links</h2>

<div class="cv-section">
  <ul class="cv-item-highlights">
    {% for link in cv_links %}
    <li><a href="{{ link.url }}">{{ link.description }}</a></li>
    {% endfor %}
  </ul>
</div>
{% endif %} -->
