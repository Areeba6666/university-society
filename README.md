# LGU Society — Lahore Garrison University

A three-page front-end website built for **Web Technologies (BSCS, Semester 5) — Assignment #2**.
Topic: **University Society** (Home & activities · Events & membership plans · Membership registration).

- **Name:** _your name_
- **Roll number:** _your roll number_
- **Section:** _your section_
- **GitHub repository:** _paste URL_
- **Live website:** _paste GitHub Pages URL_

## Project structure

| File | Purpose | CSS method |
| --- | --- | --- |
| `index.html` | Home: introduction, image, activities list | Inline CSS |
| `information.html` | Events and membership plans: article, aside, tables, audio, video | Embedded CSS |
| `registration.html` | Membership registration form | External CSS (`style.css`) |
| `style.css` | Stylesheet for `registration.html` | — |
| `images/`, `audio/`, `video/` | Media files used by the pages | — |
| `validation/` | W3C validation screenshots (add yours here) | — |

## Short explanation

CSS (Cascading Style Sheets) controls how HTML content looks: colours, fonts, spacing and layout. Its main benefits are a clean separation of content from presentation, consistent styling across many pages, and easier maintenance, because one rule can restyle an entire site.

A CSS rule has a selector, properties and values. In `style.css`, the rule `button[type="submit"] { background-color: #17463f; }` uses `button[type="submit"]` as the selector, `background-color` as the property and `#17463f` as the value.

Inline CSS is written in a `style` attribute on a single element, as on `index.html`. It is quick but cannot be reused. Embedded CSS sits inside a `<style>` element in the `<head>`, as on `information.html`, and styles only that page. External CSS lives in a separate file linked with `<link>`, as `registration.html` does with `style.css`. It can be shared by many pages and is the easiest to maintain.

CSS1 (1996) introduced basic fonts, colours and margins. CSS2 (1998) and CSS2.1 added positioning, media types and table styling, and CSS2.1 corrected earlier errors. Modern CSS is split into independent modules such as Flexbox, Grid, Selectors and Media Queries, which are developed and released separately.

Browser support matters because browsers can render the same CSS slightly differently, and some newer features are not available everywhere. I tested the site in Google Chrome and Mozilla Firefox to check that layout, form controls and media behave consistently.

Semantic HTML describes meaning. For example, `<nav>` in each page marks the navigation links. Non-semantic HTML has no meaning of its own, such as `<div class="field">` in `registration.html`, which only groups a label and its input for styling.

## Validation

All three pages were checked with the W3C Markup Validation Service (https://validator.w3.org/). Add the screenshots to the `validation/` folder:

- [ ] `validation/index.png`
- [ ] `validation/information.png`
- [ ] `validation/registration.png`

## Form testing (dummy data only)

| Test | Expected result |
| --- | --- |
| Submit with all fields empty | Browser blocks submission and flags Full Name, Email, Password and Faculty |
| Email `not-an-email` | Browser asks for a valid email address |
| Password `short` (5 characters) | Browser asks for at least 8 characters |
| Age `12` or `70` | Browser rejects values outside 16–60 |
| Type more than 300 characters in comments | Text stops at 300 characters |
| Valid details, then Submit | Confirmation message appears (nothing is stored or sent) |

## Browser testing

Record what you saw in each browser:

| Check | Browser 1: Google Chrome | Browser 2: Mozilla Firefox |
| --- | --- | --- |
| Navigation links and layout | | |
| Table styling | | |
| Audio and video playback | | |
| Form controls, focus and hover | | |
| Differences noticed | | |

## Media note

The banner image and audio clip were created for this project as placeholders. `video/lgu-society.mp4` is currently a placeholder too: replace it with the society's own reel (same file name, MP4/H.264) before submitting. The logo in `images/lgu-logo.png` comes from the university emblem.
