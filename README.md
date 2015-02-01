# Subjective Design and Objective Design, from the LeanUX NYC 2014 conference.

---

# Pivotal Presentation README

This is a presentation template for Pivots who prefer to write presentations using command-line-based tools rather than keynote.

## To use
1. `$ bundle install`
2. Start writing slides in `deck.md` using markdown. Use an `&lt;hr/&gt;` (or three hyphens, `---` in markdown) to demarcate slides.
3. `$ rake build` and in a new tab `$ rake open`
4. ???
5. Profit!

## Features
- Presentation Console with look-ahead and notes. (Hit 'p' to activate.)

## Why should I use this instead of Keynote?

The goal is to make it easy for Pivots to create on-brand presentations using more developer-friendly tools than Keynote. Pivotal branding is a requirement for our conference policy, and a useful convention—semantic markdown-y markup helps remove lots of trivial decisions about formatting and hierarchy that come with the Keynote territory. Because it's basically plaintext and terminal, keep all the goodness of your regular dev toolkit (version control, text editor of choice, etc.) instead of dealing with janky Keynote software and its janky UI.

## Workflow Recommendation
- overwrite `deck.md` and outline your thoughts in markdown
- run `rake` to rapidly turn it into a presentation
- iterate on timing, rhythm, etc. by adding, rm'ing, splitting slides. Etc.