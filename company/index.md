---
title: Company Information
permalink: /company/
eyebrow: Company
heading: Company information
lede: >-
  Formal details of Zeth Ltd, for customers, partners and anyone verifying
  the company's identity.
description: >-
  Legal and company information for Zeth Ltd, a UK software engineering
  company.
---
{%- assign c = site.data.company -%}

<dl class="facts">
  <dt>Legal name</dt>
  <dd>{{ c.legal_name }}</dd>
  <dt>Company type</dt>
  <dd>{% include fact.html value=c.company_type label="company type, e.g. private company limited by shares" %}</dd>
  <dt>Company number</dt>
  <dd>{% include fact.html value=c.company_number label="Companies House registration number" %}</dd>
  <dt>Registered in</dt>
  <dd>{% include fact.html value=c.jurisdiction label="jurisdiction, e.g. England and Wales" %}</dd>
  <dt>Officers</dt>
  <dd>{% for o in c.officers %}{{ o.name }}, {{ o.role | downcase }}{% unless forloop.last %}<br>{% endunless %}{% endfor %}</dd>
  <dt>Registered office</dt>
  <dd>{% include fact.html value=c.registered_office label="registered office address" %}</dd>
  {%- if c.show_vat %}
  <dt>VAT number</dt>
  <dd>{% include fact.html value=c.vat_number label="VAT registration number" %}</dd>
  {%- endif %}
  <dt>Email</dt>
  <dd>{% include email-link.html %}</dd>
  <dt>Website</dt>
  <dd><a href="{{ site.url }}">{{ site.url | remove: 'https://' }}</a></dd>
</dl>

{% if c.company_number %}
You can check these details on the public register at [Companies House](https://find-and-update.company-information.service.gov.uk/company/{{ c.company_number }}).
{% else %}
These details can be checked on the public register at [Companies House](https://find-and-update.company-information.service.gov.uk/).
{% endif %}

## Software published by Zeth Ltd

Zeth Ltd supports the development of [Holder]({{ c.holder.url }}), an open-source knowledge workspace. Application-specific information is in the [Holder privacy policy]({{ '/legal/holder/privacy/' | relative_url }}).

{% include placeholder.html text="Confirm which apps, if any, are distributed under Zeth Ltd's name (for example as the publisher on an app store), and list them here." %}

## Legal

- [Privacy notice]({{ '/legal/privacy/' | relative_url }})
- [Holder privacy policy]({{ '/legal/holder/privacy/' | relative_url }})
