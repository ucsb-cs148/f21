---
title: CS148 F21
permalink: "/"
---

# {{site.course}}, {{site.quarter}}

{% include collapse-button.html label="Information" id="info-list" %}
<div class="collapse" id="info-list">
 <div class="card card-body">
  {% include info_list.html %}
 </div>
</div>

{% include collapse-button.html label="Course Staff Bios" id="staff-list" %}
<div class="collapse" id="staff-list">
 <div class="card card-body">
  {% include staff_list.html %}
 </div>
</div>

{% include collapse-button.html label="Projects" id="projects" %}
<div class="collapse" id="projects">
 <div class="card card-body">
 {% include project_pages.html %}
 {% include project_table.html %}
 </div>
</div>

{% include collapse-button.html label="Labs" id="labs" %}
<div class="collapse" id="labs">
 <div class="card card-body">
 {% include lab_table.html %}
 </div>
</div>

{% include collapse-button.html label="Homework" id="hwk" %}
<div class="collapse" id="hwk">
 <div class="card card-body">
  {% include hwk_table.html %}
 </div>
</div>

{% include collapse-button.html label="Exams" id="exams" %}
<div class="collapse" id="exams">
 <div class="card card-body">
  {%include exam_table.html %}
 </div>
</div>

{% include collapse-button.html label="Lectures" id="lectures" %}
<div class="collapse" id="lectures">
 <div class="card card-body" markdown="1">

  See also: [LECTURE* repos]({{site.github_org_url}}?utf8=%E2%9C%93&q=LECTURE&type=&language=) from <{{site.github_org_url}}>
  
{%include lectures_table.html %}
 </div>
</div>
