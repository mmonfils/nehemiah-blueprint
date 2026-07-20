# The Nehemiah Blueprint
> An open-source, modular framework for faith-rooted systemic analysis.

The Nehemiah Blueprint is a low-tech, high-utility monorepo designed to bridge timeless scriptural truths with modern macroeconomic realities. Inspired by Nehemiah’s historic audit of broken city systems and his direct confrontation of economic exploitation, this repository hosts a universal structural framework for generating 45-minute "Scripture Sandwich" study modules.

Through a blend of Systems Theory and the STEEPLE framework (Social, Technological, Economic, Environmental, Political, Legal, and Ethical systems), this project views community challenges through the theological lenses of Holistic Shalom and Economic Solidarity. It helps private citizens look at local infrastructures not just as blocks of concrete, but as interconnected systems that affect human flourishing.

---

## Core Architecture

This monorepo uses a single-scroll, mobile-friendly Markdown setup powered by Jekyll. The structure keeps files organized so that any advocate can easily download, adapt, and run these modules locally or host them as a static site.

```text
nehemiah-blueprint/
├── _layouts/
│   └── default.html
├── _config.yml
├── index.md
├── template.md
└── _modules/
    ├── 2026-07-20-faith-and-social-work.md
    └── 2026-07-27-housing-justice.md
```

*   **_layouts/**: Contains the core Jekyll HTML layout configuration files.
*   **_config.yml**: The master configuration file for the site theme and settings.
*   **index.md**: The main landing page outlining the framework architecture.
*   **template.md**: The universal master template file used to build new topic modules.
*   **_modules/**: Individual flat Markdown study files named using chronological date prefixes to ensure unique namespaces and easy sorting.

---

## Available Study Modules

Browse our 5 most recent faith-rooted systemic analysis modules. For our complete historical library, visit the [Full Module Archive]({{ site.baseurl }}/archive).

{% assign sorted_modules = site.modules | reverse %}
{% for module in sorted_modules limit: 5 %}
*   **[{{ module.title }}]({{ site.url }}{{ site.baseurl }}{{ module.url }})** - Published: {{ module.date | date: "%Y-%m-%d" }}
    {% if module.tags %}Tags: *{{ module.tags | join: ", " }}*{% endif %}
{% endfor %}

---

## The Scripture Sandwich Framework

The heart of this blueprint is a 45-minute learning session that honors your time and deepens your impact. We map the traditional Pastoral Cycle (See, Judge, Act) directly onto the Inductive Bible Study Method (Observation, Interpretation, Application) to move groups from historical context to immediate public advocacy.

### Opening Liturgy (Minute 0)
*   **Time:** 1 minute.
*   **Focus:** A brief spiritual grounding prayer to center the hearts of participants on community shalom.

### Part 1: The Anchor (Minutes 1 to 15)
*   **Method Mapping:** See & Judge / Observation & Interpretation.
*   **Focus:** Grounding the session in a heavy scriptural foundation using the ESV text.
*   **Action:** Read the passage out loud and unpack the historical-cultural context. We establish what the text said to its original audience before drawing modern parallels.

### Part 2: The Friction (Minutes 16 to 30)
*   **Method Mapping:** See & Judge / Systemic Friction.
*   **Title:** The News & The Neighborhood.
*   **Focus:** Analyzing structural tension through the STEEPLE categories.
*   **Action:** Place biblical mandates directly alongside local public interest events, secular documentation, city budgets, or newspaper archives to see where the system is breaking down.

### Part 3: The Synthesis (Minutes 31 to 45)
*   **Method Mapping:** Act / Application.
*   **Focus:** Moving from awareness to tangible economic solidarity.
*   **Action:** Drive toward immediate community responses. This includes committing to personal micro-habits, participating in localized mutual aid networks, or taking public advocacy steps.

### Closing Liturgy (Minute 45)
*   **Time:** 1 minute.
*   **Focus:** A brief transition prayer sending participants back out into the neighborhood to do the work.

---

## Open Source and Civic Contribution

This repository is built entirely for private-citizen advocates who want to take independent civic action. To ensure maximum access, adaptability, and local utility, all original contents of this framework are dedicated to the public domain.

### CC0 1.0 Universal License
This work is published under the Creative Commons CC0 1.0 Universal License. The author has permanently waived all copyright and related rights to this work worldwide to the extent allowed by law. You can copy, modify, distribute, and perform the work, even for commercial purposes, all without asking permission.

---

## Module Generator Engine

<details>
<summary>Click to view the AI System Prompt for Module Generation</summary>

```text
You are an expert curriculum designer specialized in faith-rooted systemic analysis, the STEEPLE framework, and Systems Theory. Your task is to generate a highly structured, single-scroll, mobile-optimized Bible study module in Markdown that adheres to the 45-Minute Scripture Sandwich framework. 

Use a warm, community-casual, faith-rooted tone written at a strict 8th-grade reading level. Do not use em dashes or emojis. Break up the content using clean vertical bullet points and standard Markdown headers (##, ###) to maintain layout compliance for mobile screens. Include Jekyll Front Matter at the top with layout, title, and tags variables.

Please use the following outline to build out the new topic module based on the user's provided Scripture passage and local public policy focus area:

---
---
layout: default
title: "[Insert Catchy, Faith-Rooted Title]"
tags: [insert, lowercase, tags, here]
---

# Module Title: [Insert Title]
> Theme: [Insert Short Focus Statement Connecting Scripture to the Policy Issue]

## Opening Liturgy (Minute 0)
- Provide a 1-minute written prayer focusing on peace, structural awareness, and community healing.

## Part 1: The Anchor (Minutes 1–15)
### Scripture Reading
- Insert the relevant Scripture text in the ESV translation.
### Historical-Cultural Context
- Provide 3-5 vertical bullet points outlining who wrote the text, who the original audience was, and what systemic issues (social, economic, or political) were present at the time.

## Part 2: The Friction (Minutes 16–30)
### The News & The Neighborhood
- Analyze the modern issue using relevant STEEPLE filters.
- Connect the biblical text directly to secular public interest events or institutional documentation.
- Provide 3-5 vertical bullet points showing the structural tension or systemic friction present in local communities today.

## Part 3: The Synthesis (Minutes 31–45)
### Immediate Community Response
- Provide actionable next steps broken down into three distinct areas:
  1. Personal Micro-Habits: Small daily or weekly changes in lifestyle or spending.
  2. Localized Mutual Aid: Concrete steps to share resources and share burdens with neighbors.
  3. Public Advocacy Steps: Direct civic actions, such as writing letters to local officials, speaking at city council meetings, or supporting policy reform.

## Closing Liturgy (Minute 45)
- Provide a 1-minute sending prayer that commissions participants to act justly in their neighborhood throughout the week.
---
```

</details>