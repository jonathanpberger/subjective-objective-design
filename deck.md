

# TODO:

- have a drink
- record me talking about this
- transcribe
- figure out what the timing looks like, what makes the cut

---

# Subjective Design & Objective Design

---

## "Design" is a Messy Word

---


## I'm a designer

---


- web design,
- interaction design,
- product design,
- visual design,
- UX design,
- UI design,
- etc

---

## Modern "design" in the context of building products is a mix of many different design disciplines

---

# Is design objective or subjective?

---

## Can design can be objectively called "good"?

---

***what are we judging?***

---

*We tend not to distinguish between*

**the types of design that are highly objective** *and* **the types of design that are highly subjective.**

---

# E.g.

---

## marketing and branding design has a high degree of subjectivity to it.

---

## the design cannot be successful if the client doesn't feel good about it.

---

# Conversely

---

## designing a usable user interface is much more objective

---

## patterns exist,

**solutions can be tested**

---

## we can state with a high degree of confidence that one solution is (objectively) better

---

# Problem:

---

## we tend not to distinguish between different types of design when discussing work.

---

## when scoping design work, we confuse the meaning of "done" across various types of design.

---

*Designing a new logo and brand?*

**plan for several iterations of client approval**

---

*Designing a signup form?*

**"Done" can simply mean "a user can complete their goal"**

---

*To subject objectively-judge-able species of design to the approval of a non-designer client is akin to demanding client approval from your dentist or surgeon.*

---

# Articulating Objective and Subjective Design

---

### how can we address this problem?

- by crafting better stories for non-designers, explaining which parts of design benefit greatly from subjective feedback and which don't,
- by starting a conversation about a taxonomy of design types and the level of subjectivity for each.

---

## A provisional taxonomy of types of design and how subjective they tend to be

---

### ::MOST SUBJECTIVE::

- Mar/Com Design
- Product Design
- Graphic Design
- User Experience Design
- User Interface Design
- Information Architecture

### ::MOST OBJECTIVE::

---

## Marketing / Communication Design
- "How should we design our brand?"
- "Does this have the right feel?"
- "Do we like the logo?"

---

## Product Design
- "What problem should we try to solve?"
- "How can we solve it?"
- "Is this a problem worth solving?"

---

## Graphic Design
- "Does this color scheme effectively direct the user's attention?"
- "Is there a clear representation of the different nouns in the system?"
- "Is this a pleasing, balanced composition?"

---

## User Experience Design
- "Is this product a compelling way for users to accomplish their goal?"
- "Do I enjoy using the product?"
- "Is experience emotional? Persuasive?"

---

## User Interface Design
- "Does this interface help the user do what they need to?"
- "Do affordances telegraph interface? Is it understandable?"
- "Is it concise? Does it fit?"

---

## Information Architecture

- "Does this IA help the user model the world we're building?"
- "Is navigation clear and intuitive?"
- "Can new features be added in a way that makes sense for the rest of the system?"


---

## TL;DR

The utility of objective and subjective judgement varies by type of design. Designers don't do a good job of speaking clearly about this. If we, as a design community can educate clients the spectrum of subjectivity vs. type-of-design, we can save ourselves tons of pain—and save clients mega-tons of money.

---

# Thanks!

---

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

