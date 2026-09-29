---
title: Contact
permalink: /contact/
eyebrow: Contact
heading: Get in touch
lede: >-
  The simplest way to reach Zeth Ltd is by email. A few sentences is plenty
  to start with; you will get a reply from Zeth or Jutta directly.
description: >-
  Contact Zeth Ltd about contract engineering or a new application
  development project.
---
{%- assign c = site.data.company -%}

<p class="lede">Email: <strong>{% include email-link.html %}</strong></p>

<div class="split">
<div class="panel" id="contract" markdown="1">
### For Zeth to join your team

For recruiters and engineering managers. It helps to include:

- the role or project, and the main technologies;
- expected start date and duration;
- location and working arrangements.

A current CV is available on request.

<div class="button-row">
  {% include email-link.html class="button" subject="Contract enquiry" label="Email about a contract" %}
</div>
</div>
<div class="panel" id="app" markdown="1">
### For us to deliver your project

For businesses, charities and communities, with or without an in-house team. Tell us:

- what you would like the software to do;
- who it is for;
- any timescale or budget you have in mind.

We will reply to arrange an informal conversation.

<div class="button-row">
  {% include email-link.html class="button" subject="Project enquiry" label="Email about a project" %}
</div>
</div>
</div>

<p class="small">See the <a href="{{ '/privacy/' | relative_url }}">privacy notice</a>. Formal company details are on the <a href="{{ '/company/' | relative_url }}">company information</a> page.</p>
