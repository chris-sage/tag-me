---
layout: page
title: Release
subtitle: View all of our release on Github
---

Now showing all releases of {{ site.title }}

<ul>
{% for release in site.github.releases %}
  <li>
    Name: {{ release.name }} 
    Tag: {{ release.tag_name }}
    Is this pre-release: {{ release.prerelease }}

    Description: {{ release.body }}
    Link: {{ release.url }}

    <!-- <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a> -->
  </li>
{% endfor %}
</ul>

Now showing all repositories for {{ site.github.owner_name }}

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}
