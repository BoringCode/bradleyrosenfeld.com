---
layout: default
title: Portfolio
permalink: /portfolio/
nav_order: 2
---

Sometimes I build things. Check out [my resume](/assets/pdfs/bradleyrosenfeld-resume.pdf) for a full list of my experience and education.

## Projects

Most of my personal projects are open-source and are hosted on [GitHub](https://github.com/BoringCode/).

{% for project in site.data.projects %}
- [{{project.name}}]({{project.github}}){:class='primary-url'} {% if project.url %}&mdash; [Live Site]({{project.url}}){:class='secondary-url'}{% endif %}  
  {{project.description}}
{% endfor %}

## Awards & Recognition

{% for award in site.data.awards %}
- **{{award.name}}**, {{award.year}}  
  {% if award.issuer_url %}[{{award.issuer}}]({{award.issuer_url}}){% else %}{{award.issuer}}{% endif %}  
  {{award.description}}
{% endfor %}
