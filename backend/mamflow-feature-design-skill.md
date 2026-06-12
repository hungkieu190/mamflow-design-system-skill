# MamFlow Feature Design Skill

When designing a feature, always provide:

## Goal

Why does this feature exist?

What business problem does it solve?

---

## User

Who uses this feature?

* Admin
* Instructor
* Customer
* Developer
* Support Agent

---

## Primary Workflow

Describe the ideal path.

Keep it under 5 steps whenever possible.

---

## Information Hierarchy

What should users see first?

What can be hidden?

What should require interaction?

---

## States

Always define:

### Empty State

What if no data exists?

### Loading State

What appears while data loads?

### Error State

What happens if something fails?

### Success State

How does the user know the action succeeded?

---

## Permissions

Never rely on UI restrictions.

Permissions must be enforced by backend.

UI should only reflect permissions.

---

## Edge Cases

Always consider:

* Large datasets
* Missing permissions
* Failed integrations
* Partial success
* Slow responses

---

## Review Checklist

Before finalizing:

* Is the feature understandable?
* Is the workflow efficient?
* Does it follow existing patterns?
* Can users recover from errors?
* Is backend enforcement defined?

If any answer is No, revise the design.
