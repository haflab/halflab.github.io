---
layout: default
title: People
---

## Principal Investigator

{% for person in site.people %}
  {% if person.group == "PI" %}
    <div class="person-block">
      <img src="{{ person.photo }}" alt="Photo of {{ person.name }}">
      <h3>{{ person.name }}</h3>
      <p><strong>{{ person.role }}</strong><br>{{ person.affiliation }}</p>
      <p>{{ person.content | markdownify }}</p>
    </div>
  {% endif %}
{% endfor %}

## Lab Members

<div class="people-grid">
{% for person in site.people %}
  {% if person.group == "member" %}
    <div class="person-card">
      <img src="{{ person.photo }}" alt="Photo of {{ person.name }}">
      <h4>{{ person.name }}</h4>
      <p><strong>{{ person.role }}</strong></p>

      {% if person.interests.size > 0 %}
      <ul>
        {% for interest in person.interests %}
          <li>{{ interest }}</li>
        {% endfor %}
      </ul>
      {% endif %}
    </div>
  {% endif %}
{% endfor %}
</div>

