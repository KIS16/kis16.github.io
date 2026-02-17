---
layout:    page
title:     Projects
description: >
  참여·주도한 프로젝트와 연구·개발 결과물입니다.
---

참여·주도한 프로젝트와 연구·개발 결과물입니다. 항목을 클릭하면 상세 페이지로 이동합니다.

## 프로젝트 목록

{% assign sorted_projects = site.projects | sort: 'date' | reverse %}
{% for project in sorted_projects %}
- **[{{ project.title }}]({{ project.url }})**  
  {{ project.description | strip_html | strip_newlines | truncate: 120 }}
{% endfor %}
