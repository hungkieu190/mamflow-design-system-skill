# MamFlow AI Framework

This file is the entry point for all MamFlow AI workflows.

When this file is referenced, the AI must automatically load and follow the related MamFlow skills.

Never skip a required skill.

Always determine the task type first.

---

# Skill Registry

## Core Skills

Always load:

* mamflow-product-principles.md
* mamflow-visual-language.md

These files define the product DNA and visual identity.

Every output must follow them.

---

# Task Routing

Determine the user's intent and load additional skills.

---

## UI / UX Design

Examples:

* Create a screen
* Design a dashboard
* Create a settings page
* Generate wireframes
* Review UI

Load:

* mamflow-product-principles.md
* mamflow-visual-language.md
* mamflow-design-system.md
* mamflow-feature-design-skill.md

---

## Feature Planning

Examples:

* Create feature specification
* Build PRD
* Feature proposal
* Product requirements

Load:

* mamflow-product-principles.md
* mamflow-feature-design-skill.md

Focus on:

* Business goals
* User workflows
* Edge cases
* Permissions
* Scalability

Do not focus on visual implementation.

---

## UI Review

Examples:

* Review design
* Evaluate mockup
* Review wireframe

Load:

* mamflow-product-principles.md
* mamflow-visual-language.md
* mamflow-design-system.md

Evaluate:

* Consistency
* Hierarchy
* Clarity
* Visual language
* UX quality

Provide:

Strengths
Weaknesses
Recommendations

---

## HTML Generation

Examples:

* Generate Tailwind UI
* Create admin screen
* Build component

Load:

* mamflow-product-principles.md
* mamflow-visual-language.md
* mamflow-design-system.md

Requirements:

* Use TailwindCSS
* Follow MamFlow spacing scale
* Follow MamFlow color tokens
* Follow MamFlow component patterns

Never invent styles.

---

## WordPress Plugin UI

Examples:

* Settings page
* Admin screen
* Plugin dashboard

Load:

* mamflow-product-principles.md
* mamflow-visual-language.md
* mamflow-design-system.md

Additional Rules:

* Respect WordPress conventions.
* Feel native inside wp-admin.
* Avoid SaaS-style navigation.
* Prioritize tables and forms.

---

## Copywriting

Examples:

* Product description
* Documentation
* Empty states
* Error messages
* Tooltips

Load:

* mamflow-product-principles.md
* mamflow-copywriting.md

Focus on:

* Clarity
* Conciseness
* Actionability

Avoid marketing fluff.

---

## Documentation

Examples:

* User guides
* Technical docs
* API docs

Load:

* mamflow-product-principles.md
* mamflow-copywriting.md

Requirements:

* Beginner-friendly
* Step-by-step
* Action-oriented

---

# Conflict Resolution

If multiple skills provide conflicting instructions:

Priority Order:

1. mamflow-product-principles.md
2. mamflow-visual-language.md
3. mamflow-design-system.md
4. Task-specific skill

Higher priority always wins.

---

# Design Guardrails

Never:

* Use gradients
* Use glassmorphism
* Use excessive shadows
* Use rainbow dashboards
* Add decorative elements without purpose
* Introduce new color tokens

---

# Product Identity

MamFlow builds tools for professionals.

The interface should feel:

* Reliable
* Efficient
* Technical
* Focused

Not:

* Trendy
* Playful
* Over-designed

Every decision should support productivity.

---

# Final Validation

Before generating output:

Ask:

1. Does this follow MamFlow principles?
2. Does this follow MamFlow visual language?
3. Does this respect existing patterns?
4. Is this useful for professionals?
5. Is there unnecessary complexity?

If any answer is No:

Revise before responding.
