[![License](https://img.shields.io/badge/License-MIT-blue.svg)](license.md)
[![Release](https://img.shields.io/github/release/badlydrawnrob/anki)](https://github.com/badlydrawnrob/anki/releases)
[![GitHub Repo stars](https://img.shields.io/github/stars/badlydrawnrob/anki?style=social)](https://github.com/badlydrawnrob/anki/stargazers)

# Anki programming themes
## Learning to code with Anki — themes, cards, templates, syntax highlighting

******Create a new image. Simplify where possible. Add examples where possible.******

<img align="right" width="250" height="auto" src="./source/media/preview.png" style="padding-left: 20px;">


💻 Want to learn how to code?

Anki helps you learn and remember quickly. The default cards aren't great for programming, so these flashcards and themes make it fun to learn.

- Suitable for all learning levels
- Perfect for frontend and backend programmers
- Popular languages supported
- Add color to your code
- Fully customisable (create your own themes and cards!)

Are you looking to master **html**, **css**, **javascript**, **php**, **python**, **lisp**, **elm**, **R** — or just getting started? If you're new to Anki, [read these guides first](https://github.com/badlydrawnrob/anki/discussions/123); otherwise ... let's begin!

## Quick start

1. Download the [latest Anki deck (`.apkg`)](https://github.com/badlydrawnrob/anki/releases)
2. Open [Anki](https://apps.ankiweb.net). Select `File > Import ...`
3. Import the Anki deck
4. Add a new card
5. Select the `Anki themes` type
6. Get creative with your cards!


## Cards

There's two types of cards to choose from:

1. 💡 **[Simple](./source/docs/simple/index.md)**
    - What's the answer?
    - What does this syntax do?
2. 🔎 **[Missing!](./source/docs/missing/index.md)**
    - A question with a `[…]` word
    - A question with a `[missing]` word

Next, you'll probably want to [add some pretty colors](#add-color-to-your-code) to your code. But first, a quick tip on how to keep your Anki deck nice and organised ...


## Keep it simple, stupid!

> ☝️ [One idea](https://github.com/badlydrawnrob/anki/issues/41) per card. Just one.

**Simple is better.** If you only had 280 characters, what would you say? It's good practice to write your flashcards like you'd write code — as clear as possible. Those 10 cards you wrote with 100 related ideas? Sifting through those will become a chore; 100 cards with one idea is much better!

Imagine you're stupid, writing for your stupid future self; you'll look back on your flashcards and they'll make perfect sense.

- One idea per card
- Less is more (trim the fat)
- Keep it concise and relevant (reduce cognitive load)

A card stuffed with facts will overload the brain. I imagine you're trying to learn:

- A theme, or idea
- A function, or code snippet
- Syntax, or high-level documentation

That's great! But. Keep your questions clear — perhaps split a hard question into three easy cards — if you're spending more than a minute reviewing each card; reduce, reduce, reduce. Simplify it!


## Add color to your code

### Syntax highlighting

> 🎨 Life is better in full colour!

They say code is an art form. Anki themes comes with both a light and dark colour palette; highlight any [`code string`](./source/docs/simple/index.md#-syntax-inline-code) with [basic highlighting](./source/docs/highlight/index.md#basic-syntax-highlighting), or go [full colour](./source/docs/highlight/index.md#full-syntax-highlighting) with Markdown and Pandoc.

- 🖌️ **Starter themes**
    - 🌅 Monochrome
    - 🌃 Breeze Dark
- 🧑‍🎨 **[Create your own colour theme](./source/docs/highlight/index.md#customising-themes-the-easy-way)**




## Custom colors and a child theme

Once you've got the basics down, you can get _really_ fancy with offline `markdown->html`, custom cards, and using **NPM**, **Pandoc**, and **CSS** to create your theme **[🧑‍🎓 the professional way](./source/docs/advanced/index.md)**.


## Why Anki Themes instead of a plugin?

I've spent a lot of time so you can:

- Use Anki themes as they are ...
- Use the excellent `markdown->html` workflow
- Customise the css to your hearts content.

Works on all platforms: [AnkiMobile](http://ankisrs.net/docs/AnkiMobile.html), [MacOS](https://apps.ankiweb.net) (Intel, Qt6) and [Android](https://github.com/ankidroid/Anki-Android). It depends on very little from the Anki; stable software, no add-ons required, with a simple setup.

### Dependency hell

> 🕰️ A tool or a piece of software that's still around in 5 years, without any serious changes, [is a good thing](https://github.com/badlydrawnrob/anki/issues/53)

There _are_ other plugins out there that are fun to use, but [beware of dependency hell](./source/docs/error/index.md)!



## Be careful when ...

### Upgrading your deck

> ⚠️ **Always backup your deck** before installing a new version!

I try to stick to **major.minor.patch** [semantic versioning](http://semver.org), so updates don't break existing cards. Anki makes this tricky, so view commits for any major changes to the theme.

### Creating your flashcards

> ⚠️ **Stick to [Common Markdown](https://commonmark.org/) or [safe HTML](https://en.wikipedia.org/wiki/HTML_sanitization)** to [avoid unintended consequences in Anki](https://github.com/badlydrawnrob/anki/issues/27). Here's some [helpful guides](https://github.com/badlydrawnrob/anki/discussions/123) on how to use the Anki software.

### Can't swipe left to view code on Anki Mobile

The Anki Mobile app defaults to launching the menu with the _swipe left_ gesture.
This is not desirable, as often our code will have an `overflow` which we want to
scroll horizontally. You can change the settings, [see issue #118](https://github.com/badlydrawnrob/anki/issues/118) for a fix.

### Formatting problems

> ⚠️ If you're having formatting problems, make sure you're **[following the guide](#cards)** and clicking `Toggle HTML Editor ⌘⇧X` (`‹›`) in the editor to copy/paste your HTML or raw text. For more information, see [this issue](https://github.com/badlydrawnrob/anki/issues/62). Many [editors](https://en.wikipedia.org/wiki/WYSIWYG) break formatting when you `copy->paste` text, or add junk to the html.


## Licensed under MIT

Anki themes are licensed under the [MIT Open Source License](./license.md)


## Thanks to ...

### Inspiration

I've had a lot of inspiration from [Enduring CSS](https://tinyurl.com/yc4pnxyr) for component naming conventions, [@mdo code guide](http://codeguide.co/) for HTML/CSS and [@cbracco](https://github.com/cbracco) for sane frameworks ... so, thanks! iPhone photo by `@svstudioart` on Freepik.
