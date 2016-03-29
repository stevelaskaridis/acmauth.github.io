---
layout: page
navigation_title: Teams
title: ACM AUTh Teams
cover: 'https://www.acm.org/binaries/content/gallery/acm/banners/2_generic_acm_banner.jpg/2_generic_acm_banner.jpg/acm%3Adesktopbanner'
permalink: /teams/
---

{% assign active_teams = (site.teams | where: "state", "active") %}
{% assign proposed_teams = (site.teams | where: "state", "proposed") %}
{% assign past_teams = (site.teams | where: "state", "past") %}


<!--
The syntax with the newline inside each category is to prevent code liquid being parsed as <code>.
 -->

## Active

{% for page in active_teams %}
•
    [{{ page.title }}]({{ page.url }})
{% endfor %}


## Proposed

{% for page in proposed_teams %}
•
    [{{ page.title }}]({{ page.url }})
{% endfor %}


## Past

{% for page in past_teams %}
•
    [{{ page.title }}]({{ page.url }})
{% endfor %}
