---
title: "Staff List"
permalink: "/staff/"
---

# {{site.course}}, {{site.quarter}}

# Course Staff

<table class="bios">
<tr><th>Name</th><th>Role</th><th>Bio</th><th>Photo</th></tr>
{% for b in site.staff %}
  <tr>
    <td><a href="{{b.url | relative_url }}">{{b.name }}</a></td>
    <td>{{b.role}}</td>
    <td><p class="staff-bio">{{b.bio}}</p></td>
    <td>
      {% if b.img100w %}
            {%- capture image_url %}/staff/{{b.img100w}}{%- endcapture -%}
     <img src="{{ image_url | relative_url }}"
          alt="{{b.name}} image">
     {% else %}
     &nbsp;
     {% endif %}
    </td>
  </tr>
{% endfor %}
</table>

