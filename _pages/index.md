---
layout: page
title: Home
id: home
permalink: /
---

# Wassup! 😎

Пишу музыку, иногда делаю видео и фото приколы.

<strong>Ссылки:</strong>
- [Telegram](https://t.me/dierehart)
- [SoundCloud](https://soundcloud.com/joyeuxrouge)
- [YouTube](https://www.youtube.com/@joyeuxrougem)

<strong>Содержание:</strong>
- [[Музыка]]
- [[Видео]]
- [[Фото]]

<strong>Недавно обновленные заметки:</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
