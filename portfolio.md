---
layout: default
title: Portfolio
permalink: /portfolio/
nav_order: 2
---

I've made some pretty cool things. I've worked as a full-stack web developer and I've competed in a variety of capture the flag hacking competitions. I like to think laterally and my experience allows me to do that. Check out [my resume](/assets/pdfs/bradleyrosenfeld-resume.pdf) for a full list of my experience and education.

## Projects

Most of my personal projects are open-source and are hosted on [GitHub](https://github.com/BoringCode/). My philosophy is to work on projects that I would want to use. I've also worked on quite a few closed source projects for my employers. Many of which involved front-end and back-end web development.

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