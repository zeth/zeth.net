---
title: Holder Privacy Policy
permalink: /legal/holder/privacy/
eyebrow: Legal · Draft
heading: Holder privacy policy
lede: Privacy information for the Holder applications.
description: Privacy policy for the Holder applications. Draft awaiting review.
sitemap: false
---
{%- assign c = site.data.company -%}

<div class="notice" role="note" markdown="1">
**Holder already publishes a privacy policy at [holder.team/privacy/](https://holder.team/privacy/)**, which is the policy to rely on. Decide whether this page should link to it, mirror it, or be removed.

**Draft: not yet in force.** This page is a placeholder for Holder's application-specific privacy policy. It must be written from the confirmed behaviour of each released version of the apps and reviewed before it is relied on, for example in an app store listing. Nothing here describes how Holder currently behaves.
</div>

## About Holder

[Holder]({{ c.holder.url }}) is an open-source, local-first knowledge workspace. Its development is supported by {{ c.legal_name }}. {% include placeholder.html text="Confirm the legal entity that publishes each app and acts as data controller." %}

## Sections to complete

- {% include placeholder.html text="Which apps and platforms this policy covers." %}
- {% include placeholder.html text="What data the apps store, and where: on the device, and anything that leaves it." %}
- {% include placeholder.html text="Any sync, backup or network features, and which servers or services they use." %}
- {% include placeholder.html text="Any third-party SDKs, crash reporting or analytics, or a confirmed statement that there are none." %}
- {% include placeholder.html text="Device permissions requested, and why." %}
- {% include placeholder.html text="How to delete data and how to get in touch." %}
- {% include placeholder.html text="Children's privacy, if relevant to the app store listings." %}
- {% include placeholder.html text="Date of last update and how changes are announced." %}

For privacy questions about Holder: {% include email-link.html email=c.holder.privacy_email %}.

The Holder source code is public at [{{ c.holder.github | remove: 'https://' }}]({{ c.holder.github }}).
