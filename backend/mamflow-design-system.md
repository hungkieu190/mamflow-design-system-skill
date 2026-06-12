# MamFlow Design System

## Design Personality

The interface should feel:

* Professional
* Reliable
* Efficient
* Technical
* Focused

Not:

* Trendy
* Playful
* Over-designed
* Decorative

---

# Layout Structure

Preferred Page Structure:

Header

Context / Insight

Filters

Primary Content

Actions

Pagination

---

# Spacing Scale

4px
8px
12px
16px
24px
32px
48px

Use these values only.

---

# Typography

Page Title:
24px

Section Title:
18px

Card Title:
16px

Body:
14px

Helper Text:
13px

Meta Text:
12px

---

# Buttons

Only one primary action per screen.

Examples:

Create Plan
Add Course
Generate Site

Everything else should be secondary.

---

# Cards

Cards should:

* Group information
* Not replace tables
* Have clear hierarchy

Avoid dashboard card overload.

---

# Tables

Tables are first-class components.

Table density:

* Tables in operational admin screens should be compact enough for scanning.
* Header cells should use 12px vertical padding and 16px horizontal padding.
* Body cells should use 8px vertical padding and 12px horizontal padding by default.
* First and last table columns should keep clear edge padding; content must not sit flush against the table border.
* In WordPress `wp-list-table`, use selectors specific enough to override core admin table padding when needed.
* Use 12px vertical padding only when the row contains multi-line content or nested controls.
* Avoid large empty vertical space inside table rows.
* Do not use card-like blocks inside table cells unless the content needs clear grouping.
* Long text previews should have a controlled max width and line length.

Every table should support:

* Search
* Pagination
* Sorting

Optional:

* Bulk actions
* Filters

---

# Status Colors

Success:
Green

Warning:
Amber

Error:
Red

Info:
Blue

No additional status colors.

---

# Empty States

Structure:

Title

Explanation

Primary Action

Optional Documentation Link

Never use generic empty states.

---

# Loading States

Prefer:

Skeletons

Avoid:

Large spinners

---

# Error Messages

Bad:

Something went wrong.

Good:

Unable to connect to Stripe.
Verify API credentials and try again.

Errors should help users recover.
