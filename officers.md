---
layout: page
title: Officers
---
If you're interested in reaching the CSGSA board or someone on one of the committees - please send us an email at csgsa@colorado.edu or message us on the #csgsa slack channel!
## CSGSA Executive Board

### CSGSA Chair

{::options parse_block_html="true" /}
<div class="container">
<div class="row">
{%assign person = site.data.officers.chair%}
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

1. Manage all open projects
2. Run meetings of the CSGSA
3. Arrange meetings and develop agenda
4. Represent graduate students to Department and University where appropriate
5. Assign responsibilities to members as appropriate

</div>
</div>
</div>

### CSGSA Vice Chair

{::options parse_block_html="true" /}
<div class="container">
<div class="row">
<div class="col-sm-4">
<div class="card">
{::options parse_block_html="true" /}
{%assign person = site.data.officers.vice_chair%}
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

1. Run CSGSA meetings in the chair’s absence
2. Manage and maintain organizational documents
3. Manage regular email communication with members and student body
4. Be responsible for minutes of meetings
5. Assist the Chair where necessary

</div>
</div>
</div>

### CSGSA Treasurer

{::options parse_block_html="true" /}
<div class="container">
<div class="row">
<div class="col-sm-4">
<div class="card">
{::options parse_block_html="true" /}
{%assign person = site.data.officers.treasurer%}
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

<h3>Chair</h3>
<ul>
  {% assign chair = site.data.officers.alumni | where: "title", "Chair" | first %}
  {% for person in chair.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>

<h3>Vice Chair</h3>
<ul>
  {% assign vice_chair = site.data.officers.alumni | where: "title", "Vice Chair" | first %}
  {% for person in vice_chair.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>

<h3>Treasurer</h3>
<ul>
  {% assign treasurer = site.data.officers.alumni | where: "title", "Treasurer" | first %}
  {% for person in treasurer.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>
