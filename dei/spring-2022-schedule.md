---
layout: page
---
## This was the BAIC schedule for Spring 2022 semester.
{% assign semester = site.data.baic.schedule.spring22 %}
{% for entry in semester %}

### {{ entry.abstract }}

**Date** : {{ entry.date }}

**Summary** : {{ entry.summary }}

{% if entry.resources.size > 0 %}
**Resources**:
{% for resource in entry.resources %}
* [{{ resource.text }}]({{ resource.url }})
{% endfor %}
{% endif %}
{% endfor %}
