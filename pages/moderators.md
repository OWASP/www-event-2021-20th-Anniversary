---

title: Moderators
layout: event_noheader
permalink: /moderators/

---

# {{ page.title }}

<br>
<div class="keynote-full">
{% for moderator in site.data.moderators %}
<hr>
		{% if moderator.name %}
		<div>
		    <a name="{{moderator.name}}"><img style="background-image: url(/assets/images/keynotes/{{moderator.image | default: 'owasp_logo.png'}});{{moderator.style}};"></a>
		</div>
		<div class='keynote-info'>
			<a><strong>{{moderator.name}}</strong></a>
			<br>
			{{moderator.company}}
			<br>
            {{moderator.title}}
		</div>
		{% endif %}
{% endfor %}
</div>