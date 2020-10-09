---
layout: page
title: Release
subtitle: View all of our release on Github
---

Now showing all releases of {{ site.title }}

<ul>
{% for release in site.github.releases %}
  <li>
    Release: {{ release.name }} {{ release.tag_name }} {{ release.prerelease }}

    {{ release.body }}

    <!-- <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a> -->
  </li>
{% endfor %}
</ul>

Now showing all repositories for {{ site.owner_name }}

{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}
