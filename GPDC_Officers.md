---
layout: page
title: GPDC Officers
---



If you're interested in reaching the CSGPDC execs - please send us an email at csgpdc@colorado.edu

### CSGPDC Chair

{::options parse_block_html="true" /}
<div class="container">
<div class="row">
{%assign person = site.data.officers.gpdc_chair%}
<div class="col-sm-4">
<div class="card">
{::options parse_block_html="true" /}
{%if person.photo%}
![{{person.name}}]({{person.photo}}){:height="300px"}
{%endif%}
{{person.name}}

Pronouns: {{person.pronouns}}

Bio: {{person.bio}}
</div>
</div>

<div class="col-sm-8">
The chair's responsibilities are to:

1. Manage all open activities and events
2. Work closely with identified resources (both on and off campus) to organize events.
3. Work on identifying questions from various companies to run the practice coding events
4. Host meetings of CS-GPDC
5. Arrange meetings and develop agenda
6. Assign responsibilities to members as appropriately

</div>
</div>
</div>

### CSGPDC Vice Chair

{::options parse_block_html="true" /}
<div class="container">
<div class="row">
<div class="col-sm-4">
<div class="card">
{::options parse_block_html="true" /}
{%assign person = site.data.officers.gpdc_vice_chair%}
{%if person.photo%}
![{{person.name}}]({{person.photo}}){:height="300px"}
{%endif%}
{{person.name}}

Pronouns: {{person.pronouns}}

Bio: {{person.bio}}
</div>
</div>

<div class="col-sm-8">
The vice chair's responsibilities are to:

1. Run CS-GPDC meetings in the chair’s absence
2. Manage and maintain organizational documents
3. Manage regular email communication with members and student body
4. Be responsible for minutes of meetings
5. Assist the Chair where necessary

</div>
</div>
</div>

### CSGPDC Treasurer

{::options parse_block_html="true" /}
<div class="container">
<div class="row">
<div class="col-sm-4">
<div class="card">
{::options parse_block_html="true" /}
{%assign person = site.data.officers.gpdc_treasurer%}
{%if person.photo%}
![{{person.name}}]({{person.photo}}){:height="300px"}
{%endif%}
{{person.name}}

Pronouns: {{person.pronouns}}

Bio: {{person.bio}}
</div>
</div>

<div class="col-sm-8">
The treasurer's responsibilities are to:

1. Handle any and all financial matters
2. Apply for funding each year from multiple sources
3. Submit reimbursement forms when needed
4. Assist the Chair where necessary
5. Report regularly on financial status of the organization

</div>
</div>
</div>


# Alumni

We're sad to see you go! Thanks for all your help.

<h3>CSGPDC Chair</h3>
<ul>
  {% assign chair = site.data.officers.alumni | where: "title", "GPDC Chair" | first %}
  {% for person in chair.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>

<h3>CSGPDC Vice Chair</h3>
<ul>
  {% assign vice_chair = site.data.officers.alumni | where: "title", "GPDC Vice Chair" | first %}
  {% for person in vice_chair.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>

<h3>CSGPDC Treasurer</h3>
<ul>
  {% assign treasurer = site.data.officers.alumni | where: "title", "GPDC Treasurer" | first %}
  {% for person in treasurer.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>





 
