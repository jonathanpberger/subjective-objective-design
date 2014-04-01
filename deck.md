# TODO:

- have a drink
- record me talking about this
- transcribe
- figure out what the timing looks like, what makes the cut

---

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
- Who's had trouble defining "done" for a design problem?

---

## Developers had similar problems

---

**and so devised**
***automated testing techniques***
**to protect their work.**


---

## What might automated testing look like for design?


---

**What would it look like to have a more defined definition of "done" for design?**


---

**What if designers could refactor with impunity?**


---

In this talk we'll explore testing possibilities for

- Visual design,
- User Experience design, and
- front-end engineering,

---

and
**try to build a testing pyramid for design.**

---

***20 yrs ago***

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

### Benefits

Paul Wilson [says](http://www.neo.com/2014/03/20/the-many-faces-of-test-driven-development):

> For me, TDD's benefits are:

> - It gives me **confidence** that my code does what I think it does

> - It confers the **ability to refactor** code without the fear that I have broken something

> - It encourages a testable, and hence modular, **design**

> - The **tests describe the behaviour** of the code

---

### Technique
- Red
- Green
- Refactor

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

<!-- not sure where this goes -->

Independent: maybe?
Negotiable: yes!
Valuable: yes!
Estimatable: in theory, yes
Small: maybe?
Testable: working on that now

---

# 99 (Hypo)theses
not sure if this is part of the talk, a new version of the talk, or what. But I shuold go with it for a little while.

---

> "We believe [TYPE OF USER] has a problem [DOING THING]. We can help them with [OUR SOLUTION]. We'll know we're right if [CHANGE IN METRIC]."

---

We believe designers have a problem 

*refactoring the messes of CSS that metastasize once a project gets past the early phases.*

We can help them with 

*a tool that provides for refactoring CSS with impunity.*

We'll know we're right 

*if Latter-Day Stylesheets become less of a problem (we can test this on our own codebases).*

---

We believe designers suffer from unintended design regressions (especially in responsive designs) when changes in one part of the codebase unexpectedly affect another. We can help them with a tool that craws the whole app and announces if anything's changed.

---


We believe designers suffer from the *fear* of unintended design regressions, never being 100% certain that new changes haven't broken old styling.

---


*We believe*

designers have trouble defining "done", which makes it hard to set expectations, to communicate with teams, and to manage their own work. 

*We can fix this *

with a practice of Test-Driven Design, where "done" can be INVESTED up-front. 

*We'll know we're right*

if there're fewer client disapprovals, because expectations were better set up-front. We'll know we're right if life gets better for designers.

---


We believe developers lacked confidence that their code would continue to work in the face of a changing codebase. They fixed it by testing their code and running Continuous Integration tests. We know they're right because this is a growing practice among businesses and developers.

---


We believe developers suffered from an inability to safely refactor code for fear of breaking something. They fixed this with tests, and we know they're right because techniques like Red-Green-Refactor can become cornerstones of their practice.

<!-- 2 more: testable and hence modular, and "tests describe behavior" -->

---


We believe designers have a problem with the imprecision of the word "design". We can fix this by spreading a vocabulary with more subtle distinctions. We'll know we're right if expectations are better set because client and designer share a ubiquitous language.


---

# Pyramid of types of design

what is it?, what do we usually call it?, how do we usually deliver it?, how could we test it?
concept / visual language / metaphor (IA?)
UX / wires

CSS
expression: final app

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

