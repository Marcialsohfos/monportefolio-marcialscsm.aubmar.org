---
layout: page
title: Tous mes projets
---

<div class="projects-page">

  <p class="page-description">Découvrez l'ensemble de mes réalisations en gestion de données, de la santé publique aux données urbaines.</p>

  <div class="projects-list">
    {% assign sorted_projects = site.projects | sort: 'date' | reverse %}
    {% for project in sorted_projects %}
    <div class="project-item">
      <div class="project-date">{{ project.date | date: "%B %Y" }}</div>
      <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
      <div class="project-meta">
        <span class="project-client">{{ project.client }}</span>
        <div class="project-tags">
          {% for tag in project.tags %}
          <span class="tag">{{ tag }}</span>
          {% endfor %}
        </div>
      </div>
      <p class="project-excerpt">{{ project.excerpt | strip_html | truncatewords: 50 }}</p>
      <a href="{{ project.url | relative_url }}" class="read-more">Lire la suite →</a>
    </div>
    {% endfor %}
  </div>

</div>

<style>
.projects-page {
  max-width: 900px;
  margin: 0 auto;
}
.page-description {
  font-size: 1.2rem;
  color: #586069;
  margin-bottom: 3rem;
}
.project-item {
  margin-bottom: 3rem;
  padding-bottom: 2rem;
  border-bottom: 1px solid #eaecef;
}
.project-item:last-child {
  border-bottom: none;
}
.project-date {
  color: #6a737d;
  font-size: 0.9rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  margin-bottom: 0.5rem;
}
.project-item h2 {
  margin-top: 0;
  margin-bottom: 0.5rem;
}
.project-item h2 a {
  color: #24292e;
  text-decoration: none;
}
.project-item h2 a:hover {
  color: #0366d6;
}
.project-meta {
  margin-bottom: 1rem;
}
.project-client {
  display: inline-block;
  background: #f1f8ff;
  color: #0366d6;
  padding: 0.2rem 0.8rem;
  border-radius: 3px;
  font-size: 0.9rem;
  font-weight: 500;
  margin-right: 1rem;
}
.project-tags {
  display: inline-block;
}
.tag {
  display: inline-block;
  background: #f6f8fa;
  color: #24292e;
  padding: 0.2rem 0.5rem;
  border-radius: 3px;
  font-size: 0.8rem;
  margin-right: 0.3rem;
}
.project-excerpt {
  color: #586069;
  line-height: 1.6;
}
.read-more {
  color: #0366d6;
  text-decoration: none;
  font-weight: 500;
}
.read-more:hover {
  text-decoration: underline;
}
</style>