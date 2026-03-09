---
layout: default
title: Accueil
---

<div class="hero-section">
  <h1 class="hero-title">Data Management Specialist | Santé publique & Gouvernance des données</h1>
  
  <blockquote class="hero-quote">
    J'ai accompagné le Ministère de la Santé Publique du Cameroun dans la cartographie nationale des laboratoires et la mise en place d'outils de gestion des données de santé.
  </blockquote>
</div>

---

## Compétences clés

<div class="skills-tags">
  <span class="skill-tag">Python</span>
  <span class="skill-tag">R</span>
  <span class="skill-tag">Qgis</span>
  <span class="skill-tag">SQL</span>
  <span class="skill-tag">Power BI</span>
  <span class="skill-tag">Kobocollect</span>
  <span class="skill-tag">MapitGit</span>
  <span class="skill-tag">Gouvernance des données</span>
  <span class="skill-tag">RGPD</span>
  <span class="skill-tag">ETL</span>
  <span class="skill-tag">Données géospatiales</span>
  <span class="skill-tag">Santé publique</span>
  <span class="skill-tag">Gestion de projet</span>
</div>

---

## À propos

Basé à Yaoundé, je suis spécialisé dans la gestion des données de santé publique et des données urbaines. Mon parcours est marqué par une expérience terrain au **Service des Laboratoires du MINSANTE**, où j'ai piloté la cartographie nationale des laboratoires et mis en place des systèmes de surveillance.

Convaincu que la donnée de santé doit être fiable et accessible pour éclairer les décisions, j'ai développé des outils (LogicAppAnalytics, application de gestion des doublons) qui sont aujourd'hui utilisés par d'autres data analysts.

Je maîtrise l'ensemble de la chaîne de traitement :
- **Collecte** : Kobocollect, MapitGit
- **Appurement et nettoyage** : Python, R, application anti-doublons
- **Analyse statistique et géospatiale** : R, Python, Qgis
- **Restitution** : dashboards MAPE/biosécurité, cartes thématiques

---

## Projets récents

<div class="projects-grid">
  {% for project in site.projects limit:3 %}
  <div class="project-card">
    <a href="{{ project.url | relative_url }}">
      {% if project.image %}
      <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
      {% endif %}
      <h3>{{ project.title }}</h3>
      <p>{{ project.excerpt | truncatewords: 30 }}</p>
      <div class="project-tags">
        {% for tag in project.tags limit:3 %}
        <span class="tag">{{ tag }}</span>
        {% endfor %}
      </div>
    </a>
  </div>
  {% endfor %}
</div>

<a href="{{ '/projects' | relative_url }}" class="button">Voir tous les projets →</a>