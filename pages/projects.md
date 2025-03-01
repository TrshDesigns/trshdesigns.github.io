---
layout: page
title: Projects
permalink: /projects/
---

<div class="projects-grid">
  {% for project in site.projects %}
    <div class="project-item">
      <a href="{{ project.url }}">
        <img src="{{ project.cover }}" alt="{{ project.title }} Cover" class="project-cover" />
        <span class="project-title">{{ project.title }}</span>
      </a>
      <p class="project-description">{{ project.description }}</p>
    </div>
  {% endfor %}
</div>

<style>
.projects-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr); /* Two columns */
    gap: 10px; /* Space between items */
    margin: 20px; /* Margin around the grid */
}

.project-item {
    text-align: center; /* Center the text */
}

.project-item:hover {
    background-color:rgba(240, 240, 240, 0.31); /* Light gray background on hover */
    transform: scale(1.05); /* Slightly enlarge the item */
    transition: background-color 0.3s ease, transform 0.3s ease; /* Smooth transition for effects */
    cursor: pointer; /* Change cursor to pointer */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Add shadow effect */
    border-radius:3px;
    color: black;
}

.project-cover {
    max-width: 100%; /* Responsive image */
    height: 120px;
    border: 2px solid #888; /* Optional: Add a border */
    border-radius: 2px; /* Optional: Add rounded corners */
    margin-bottom: 5px; /* Space between image and title */
}
</style>