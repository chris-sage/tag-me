---
layout: page
title: Release
subtitle: View all of our release on Github
---

Now showing all releases of {{ site.title }}

{% for release in site.github.releases %}
Name: [{{ release.name }}]({{ release.html_url }})  
Tag: {{ release.tag_name }}  
Is this pre-release: {{ release.prerelease }}  

Description: {{ release.body }}  

{% endfor %}
