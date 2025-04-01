---
title: Happamia sanoi kettu pihlajanmarjoista
---

<img width="759" alt="Screenshot 2025-04-01 at 21 50 23" src="https://github.com/user-attachments/assets/49b41630-a973-43b3-9521-cff73382859f" />

Tarinoita ja turinoita ja sen semmoista.

<h2>Viimeisimmät kirjoitukset</h2>

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <span class="post-date">{{ post.date | date: "%d.%m.%Y" }}</span>
      <h3>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      {% if post.excerpt %}
        <p>{{ post.excerpt }}</p>
        <a href="{{ post.url | relative_url }}" class="read-more">Lue lisää &raquo;</a>
      {% endif %}
    </li>
  {% endfor %}
</ul>
