**Hi :-)**

---


# Lean UX NYC, 2014

Jonathan Berger, Pivotal Labs

---

# Towards a Theory of Test-Driven Design

---

**or**

---

***A Proposed program for Automated Testing in Design***


---

# Designers have Problems

---

- Who's had to refactor a mess of CSS?
- Who's had unintended design changes (especially in responsive designs) lead to regressions?

---

## Developers had similar problems

---

**and so devised**
***automated testing techniques***
**to protect their work.**


---

## What would automated testing look like for design?


---

## What would it look like to have a more defined definition of "done" for design?


---

## What if designers could refactor with impunity?


---

In this talk we'll explore testing possibilities for

- Visual design,
- User Experience design, and
- front-end engineering,

---

and
**try to build a testing pyramid for design.**

---

---

**20 yrs ago**

---

## Software development had problems

- Sclerosis around processes and tools,
- Compulsive (CYA) documentation,
- Endless negotiation about targets and deliverables,
- A fixation on following an old plan in a new situation.

---

## What is design?

(people ask "did you design that shirt?")

---

## What is Test-Driven Development?
- benefits
- technique

---

## What is Test-Driven Design?
- benefits
- technique

---

# Dev Testing Pyramid
- 1 ("Functional") Acceptance test
- 10 Integration tests
- 100 Unit tests

or

UI
Service
Unit

---

# Design Testing Pyramid

## Assert Design Decisions (cactus)
## Control Regressions (green_onion)
## Safely refactor bloated CSS (CSS Racionator)
## Enforce Code Conventions (CSS Lint)
## Enforce personas (persona_dot_yml)
## Enforce Styleguide-Driven Development (style_cop)


---

# Notes


## Ideal Workflow

### VxD
- designer designs new user_profile/show page
- creates a "test": screenshot
- developer implements feature
- run tests
  - screenshoot each page
  - image diff each screenshot against last version or design_tests

- (if PASS then NOTHING HAPPENS)
- if FAIL then
  - stop the line (e.g. break the CI build)
  -

### FE
- refactor some CSS
- run tests: screenshots are image-diff'd
- FAIL! user_profile/show looks different
- Was this a desired difference?
  - if YES: bless this new screenshot. Does this imply a Design Changelog?
  - if NO: fix it

- stop the line (e.g. break the CI build)
- look at what broke, fix the CSS



### UX
- design something new
- run tests
- if PASS then NOTHING HAPPENS
- if FAIL then
  - stop the line (e.g. break the CI build)
  -





---

# Thanks!

- <http://jonathanpberger.com/talks>
- Say hi on twitter at `@jonathanpberger`
- or `jonathanpberger` on github, gmail, forrst, etc...

---
<script src="js/jquery.js"></script>

<script src="js/impressConsole.js"></script>
<script>
    impressConsole().init();
    // impressConsole().open(); // for console to open automatically
</script>

