---
title: Contact
permalink: /contact/
eyebrow: Contact
heading: Get in touch
lede: >-
  The simplest way to reach Zeth Ltd is by email. A few sentences is plenty
  to start with; you will get a reply from Zeth directly.
description: >-
  Contact Zeth Ltd about contract engineering or a new application
  development project.
---
{%- assign c = site.data.company -%}

<p class="lede">Email: <strong>{% include email-link.html %}</strong></p>

<div class="split">
<div class="panel" id="contract" markdown="1">
### Contract engineering

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
### A new app idea

For businesses, charities and communities. No technical detail needed; just tell us:

- what you would like the app to do;
- who it is for;
- any timescale or budget you have in mind.

We will reply to arrange an informal conversation.

<div class="button-row">
  {% include email-link.html class="button" subject="New app idea" label="Email about an idea" %}
</div>
</div>
</div>

<p class="small">See the <a href="{{ '/privacy/' | relative_url }}">privacy notice</a>. Formal company details are on the <a href="{{ '/company/' | relative_url }}">company information</a> page.</p>
