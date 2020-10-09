---
layout: page
title: Release
subtitle: View all of our release on Github
---

Now showing all releases of {{ site.title }}

<ul>
{% for release in site.github.releases %}
    Name: {{ release.name }} 
    Tag: {{ release.tag_name }}
    Is this pre-release: {{ release.prerelease }}

    Description: {{ release.body }}
    Link: <a href="{{ release.html_url }}">{{ release.html_url }}</a>

{% endfor %}
</ul>
