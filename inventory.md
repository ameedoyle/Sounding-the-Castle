---
layout: default
title: Inventory
nav_order: 3
---

# Inventory

## Collections

- [Antiphoners]({{ "/objects/" | relative_url }})
- Chant fragments/Lampshades
- Instruments
- Piano rolls
- Performers and performances

## Antiphoners

<table>
  <thead>
    <tr>
      <th>Object ID</th>
      <th>Title</th>
      <th>Date</th>
      <th>Place</th>
      <th>Type</th>
    </tr>
  </thead>
  <tbody>
    {% for item in site.data.antiphoner %}
      <tr>
        <td><a href="{{ item.url | relative_url }}">{{ item.id }}</a></td>
        <td>{{ item.title }}</td>
        <td>{{ item.date }}</td>
        <td>{{ item.place }}</td>
        <td>{{ item.type }}</td>
      </tr>
    {% endfor %}
  </tbody>
</table>
