
<h3>Keynote Speakers</h3>
<ul>
{% for speaker in site.data.keynotespeakers %}
    {% if speaker.name %}
        <li><a href="/program/keynotes#{{speaker.name}}" class="keynote-img" style="background-image: url(assets/images/keynotes/{{speaker.image | default: 'owasp_logo.png'}});">
            <!--<h4>{{ speaker.name }}</h4>--></a>
        </li>
    {% endif %}
{% endfor %}
</ul>