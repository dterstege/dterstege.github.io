---
layout: splash
permalink: /repositories/
hidden: true
title: "GitHub"
excerpt: "GitHub Repositories"
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/main_hero.png
---

{% if site.data.repositories.github_users %}
## GitHub users
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>

  ---

{% endfor %}
{% endif %}
{% endif %}

{% if site.data.repositories.github_repos %}
<!-- ## GitHub Repositories -->
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
