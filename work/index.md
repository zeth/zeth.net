---
title: Work
permalink: /work/
eyebrow: Work
heading: Engineering you can inspect
lede: >-
  Much commercial work cannot be shown in public. Open-source work can, so
  it is the clearest evidence of how Zeth Ltd approaches engineering.
description: >-
  Selected engineering work by Zeth Ltd, including Holder, an open-source,
  local-first knowledge workspace for mobile and desktop.
wide: true
---
{%- assign h = site.data.company.holder -%}

<section class="feature" id="holder" aria-labelledby="holder-heading">
<div markdown="1">
<p class="eyebrow">Featured · Internally developed open-source project</p>

## Holder {#holder-heading}

<p class="feature__quote">{{ h.tagline }}</p>

Holder is a local-first workspace for cards, projects, resources and AI threads. Your knowledge is kept on your own machine, not only on someone else's server. It is developed in the open, with support from Zeth Ltd, and has its own project identity and community.

<div class="button-row">
  <a class="button" href="{{ h.url }}">Visit holder.team</a>
  <a class="button button--ghost" href="{{ h.github }}">Source code on GitHub</a>
</div>
</div>
{% include holder-slot.html %}
</section>

## What Holder demonstrates

<div class="split split--pairs" markdown="1">
<div markdown="1">
### Cross-platform architecture

Mobile and desktop applications share one C/C++ core, so the essential logic is written and tested once and every platform behaves consistently.
</div>
<div markdown="1">
### Local-first design

Designing for data that lives on the user's device raises practical questions about storage, reliability and keeping multiple devices in step.
</div>
<div markdown="1">
### Testing

A shared core only works if it is trustworthy. Automated tests are part of the project and can be read alongside the code.
</div>
<div markdown="1">
### Packaging and release

Desktop releases are published for each platform: an Ubuntu PPA, a signed AppImage for Linux, a signed and notarised macOS disk image, and a Windows installer. Each is built, packaged and distributed repeatably.
</div>
</div>

### Where it stands

- **Desktop:** version 0.2.0, available for Ubuntu, Linux, macOS and Windows from [holder.team]({{ h.url }}).
- **Android:** in active development and built from source; not yet on the Play Store.
- **Beyond the GUI:** a local backend service with an HTTP API and a command-line tool, so Holder can fit into other workflows.

Holder is young and says so plainly: some platforms and features are further along than others.

<p class="small">Holder is an internally developed open-source project, not a commissioned client project. Details of client work are shared privately where confidentiality allows.</p>

## Client and contract work

Client work is usually confidential, so it is summarised without names: machine-learning pricing tools, insurance payments, fleet management, electric-vehicle app backends, research software and more. See the [experience summary]({{ '/services/contract-engineering/#experience' | relative_url }}) on the contract engineering page.

<div class="panel" markdown="1">
### Want something similar built?

The same engineering goes into client projects. [Read about application development]({{ '/services/app-development/' | relative_url }}) or [get in touch]({{ '/contact/' | relative_url }}).
</div>
