# Neurohackademy 2019 course materials

This repository contains links and descriptions of all publicly shareable materials, code, data, etc. used by instructors at Neurohackademy 2019. The ordering of lectures and tutorials follows the chronology of the course.

{% for sec in sections %}* {{sec.name}} ({{sec.value}})
{% for bl in blocks %}{% if bl.date == sec.value %}	* [{{bl.time}}] {% if bl.slides %}[{% endif %}{{bl.title}}{% if bl.slides %}]({{bl.slides}}){% endif %} ({{bl.instructor}}){% if bl.repo %} [[repo]]({{bl.repo}}){% endif %}{% if bl.video %} [[video]]({{bl.video}}){% endif %}
{% endif %}{% endfor %}
{% endfor %}
