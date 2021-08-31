---

title: Supporters
layout: event_noheader-2.0
permalink: /supporters/

---
<section class="member-list">
{% assign supporters = site.data.supporters | sort: "logo" | reverse %}
{% for supporter in supporters  %}
{%- if supporter.logo -%}
<div style="float:left;"><a href="{{supporter.url}}" class="supporter-logo" style="filter:none;"><img src="{{supporter.logo}}"/></a></div>
{% else %}
<div style="float:left;"><a href="{{supporter.url}}" class="supporter-logo" style="filter:none;">{{supporter.name}}</a></div>
{%- endif -%}
{% endfor %}
</section>