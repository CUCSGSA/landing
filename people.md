---
layout: page
title: People
---


CSGSA will not be as successful as it is without the help of all of our amazing representatives, co-ordinators and volunteers. 


Here are some of the people in these roles currently.


## Department Graduate Committee Student Representatives

The Graduate Committee is charged with a broad range of graduate student affairs, both for Masters and PhD students. This committee reviews all applications for admission to the Masters and Doctoral programs in Computer Science. All problems regarding any proposed changes to both the Master’s program and the Ph.D. program are handled by this Graduate Committee. It is also responsible for defining course content, considering new course offerings, and other issues for the graduate degree programs. There are three student representatives on the Graduate Committee, two PhD students and one Masters student.



{::options parse_block_html="true" /}
<div class="container">
{%for person in site.data.officers.grad_comm%}
<div class="col-sm-6">
<div class="card">
{%if person.photo%}
![{{person.name}}]({{person.photo}}){:height="300px"}
{%endif%}
{{person.name}}

Pronouns: {{person.pronouns}}

Bio: {{person.bio}}
</div>
</div>
{%endfor%}
</div>


## Department Executive Committee Student Representative
{::options parse_block_html="true" /}
<div class="container">
<div class="row">
<div class="col-sm-4">
<div class="card">
{::options parse_block_html="true" /}
{%assign person = site.data.officers.exec_comm%}
{%if person.photo%}
![{{person.name}}]({{person.photo}}){:height="300px"}
{%endif%}
{{person.name}}

Pronouns: {{person.pronouns}}

Bio: {{person.bio}}
</div>
</div>

<div class="col-sm-8">
The student member of this committee is considered to be the senior student representative. This committee usually meets once a week and is concerned with all Department issues: budget, space, promotions, etc. The Executive Committee also reviews applications from prospective new faculty members. The student representative sits on both the Executive Committee and the Search Committee with one full vote. This position provides an excellent opportunity to see how an academic Department is really run. Sometimes the representative is required to poll graduate student opinion and is usually in charge of taking prospective new faculty members out to lunch with a group of graduate students.
</div>
</div>
</div>


## Student Representative for the DEIA (Diversity, Equity, Inclusion, and Accessibility) Committee
{::options parse_block_html="true" /}
<div class="container">
{%for person in site.data.officers.deia%}
<div class="col-sm-6">
<div class="card">
{%if person.photo%}
![{{person.name}}]({{person.photo}}){:height="300px"}
{%endif%}
{{person.name}}

Pronouns: {{person.pronouns}}

Bio: {{person.bio}}
</div>
</div>
{%endfor%}
</div>

## GPSG Student Representatives
[The Graduate and Professional Student Government](https://www.colorado.edu/gpsg/) is the primary advocacy group for graduate and professional students on the CU Boulder campus. They are committed to enhancing the graduate student experience by interacting with CU administration and the University of Colorado Student Government (CUSG) concerning issues such as financial aid, graduate stipends, healthcare, tuition and fees and graduate student well-being. Graduate students from each department and program are solicited to serve on the GPSG Assembly, ensuring diverse representation of the graduate student body. We have an official voting GPSG representative, but any student can attend GPSG meetings. Meetings are held weekly on Wednesdays, from 4 - 5 PM.

{::options parse_block_html="true" /}
<div class="container">
{%for person in site.data.officers.gpsg%}
<div class="col-sm-6">
<div class="card">
{%if person.photo%}
![{{person.name}}]({{person.photo}}){:height="300px"}
{%endif%}
{{person.name}}

Pronouns: {{person.pronouns}}

Bio: {{person.bio}}
</div>
</div>
{%endfor%}
</div>

## Web Guru

{::options parse_block_html="true" /}
<div class="container">
<div class="row">
<div class="col-sm-4">
<div class="card">
{::options parse_block_html="true" /}
{%assign person = site.data.officers.webguru%}
{%if person.photo%}
![{{person.name}}]({{person.photo}}){:height="300px"}
{%endif%}
{{person.name}}
{%if person.pronouns%}
Pronouns: {{person.pronouns}}
{%endif%}
{%if person.bio%}
Bio: {{person.bio}}
{%endif%}
</div>
</div>

<div class="col-sm-8">
Web Guru is responsible for maintaining CSGSA website (this website :P). This involves creating new pages, existing content updation and working of the website. Additionally, Web Guru has to collaborate with members of CSGSA to ensure all the work done is updated on the website.
</div>
</div>
</div>




# Alumni

We're sad to see you go! Thanks for all your help.

<h3>Grad comm reps</h3>
<ul>
  {% assign Graduate_Committee = site.data.officers.alumni | where: "title", "Graduate Committee" | first %}
  {% for person in Graduate_Committee.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>

<h3>Executive Committee</h3>
<ul>
  {% assign ecomm = site.data.officers.alumni | where: "title", "Executive Committee" | first %}
  {% for person in ecomm.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>

<h3>GPSG Rep</h3>
<ul>
  {% assign gpsg = site.data.officers.alumni | where: "title", "GPSG Student Representative" | first %}
  {% for person in gpsg.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>

<h3>Web guru</h3>
<ul>
  {% assign web_guru = site.data.officers.alumni | where: "title", "Web Guru" | first %}
  {% for person in web_guru.people %}
    <li>{{ person.years }} &raquo; {{ person.name }}</li>
  {% endfor %}
</ul>