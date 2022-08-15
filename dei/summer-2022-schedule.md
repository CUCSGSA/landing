---
layout: page
---
## This was the BAIC schedule for Summer 2022 semester.
{% assign semester = site.data.baic.schedule.summer22 %}
{% for entry in semester %}

### {{ entry.abstract }}

**Date** : {{ entry.date }}

**Summary** : {{ entry.summary }}

**Resources**:

{% for resource in entry.resources %}
  * [{{ resource.text }}]({{ resource.url }})
{% endfor %}
{% endfor %}
