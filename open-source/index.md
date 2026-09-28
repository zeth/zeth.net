---
title: Open Source
permalink: /open-source/
eyebrow: Open Source
heading: Engineering you can inspect
lede: >-
  Much commercial work cannot be shown in public. Open-source work can.
  Zeth Ltd contributes engineering time and infrastructure to open-source
  projects, which keep their own names, communities and direction.
description: >-
  Open-source projects supported by Zeth Ltd, including Holder, a
  local-first knowledge workspace.
---
{%- assign h = site.data.company.holder -%}

## Why we do it

Open source lets anyone inspect, use and improve software, and it keeps our own engineering honest because the work is visible. Supporting it is part of how Zeth Ltd works, not a marketing exercise.

<section class="feature" id="holder" aria-labelledby="holder-heading">
<div markdown="1">
<p class="eyebrow">Featured project</p>

## Holder {#holder-heading}

<p class="feature__quote">{{ h.tagline }}</p>

Holder is a local-first workspace for cards, projects, resources and AI threads. Your knowledge is kept on your own machine, not only on someone else's server.

Holder is a volunteer-run project maintained by the Holder Team. Zeth Ltd supports it with development, infrastructure, and administrative and organisational help, but Holder is its own project, with its own website and community. Anyone is welcome to use it and contribute.

<div class="button-row">
  <a class="button" href="{{ h.url }}">Visit holder.team</a>
  <a class="button button--ghost" href="{{ h.github }}">Source code on GitHub</a>
</div>
</div>
{% include holder-slot.html %}
</section>

### What Holder demonstrates

<div class="split split--pairs" markdown="1">
<div markdown="1">
#### Cross-platform architecture

Mobile and desktop applications share one C/C++ core, so the essential logic is written and tested once and every platform behaves consistently.
</div>
<div markdown="1">
#### Local-first design

Designing for data that lives on the user's device raises practical questions about storage, reliability and keeping multiple devices in step.
</div>
<div markdown="1">
#### Testing

A shared core only works if it is trustworthy. Automated tests are part of the project and can be read alongside the code.
</div>
<div markdown="1">
#### Packaging and release

Desktop releases are published for each platform: an Ubuntu PPA, a signed AppImage for Linux, a signed and notarised macOS disk image, and a Windows installer. Each is built, packaged and distributed repeatably.
</div>
</div>

### Where it stands

- **Desktop:** version 0.2.0, available for Ubuntu, Linux, macOS and Windows from [holder.team]({{ h.url }}).
- **Android:** in active development and built from source; not yet on the Play Store.
- **Beyond the GUI:** a local backend service with an HTTP API and a command-line tool, so Holder can fit into other workflows.

Holder is young and says so plainly: some platforms and features are further along than others.

## Other contributions

- **Python:** contributions to Python itself, and **inputs**, a cross-platform Python library for USB devices, created by Zeth.
- **Django:** closed a Django bug during the DjangoCon Europe 2025 sprints in Dublin.
- **Interedition and CollateX:** collaborated in these EU projects to create open-source software for scholarly editing, including [CollateX](https://collatex.net/about/) for comparing versions of texts.
- **Community:** Zeth founded Python West Midlands, co-founded PyCon UK and is a Fellow of the Python Software Foundation. [More on the About page]({{ '/about/#open-source-and-community' | relative_url }}).

## Get involved

If you are interested in one of these projects, the best place to start is the project's own website and repository. For anything to do with Zeth Ltd itself, [contact us]({{ '/contact/' | relative_url }}).
