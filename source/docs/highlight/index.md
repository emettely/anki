# Themes

- [Home](../../../README.md)
    + 💡 [Simple](../simple/index.md) card
    + 🔎 [Missing!](../missing/index.md) card
    + 🖍️ [Draw!](../draw/index.md) card
    + 🧑‍🎨 **[Add color to your code](../highlight/index.md)**
    + 🧑‍🎓 [The professional way](../professional/index.md)


## Basic syntax highlighting

> **Default colors**: Monochrome and [Breeze Dark](../../source/style/modules/variables/breezedark.less)

You can mark any inline **[`code string`](../simple/index.md#-syntax-inline-code)** field with **bold** or _**italic**_ buttons in the Anki editor for basic highlighting. It uses simple [HTML5 tags](https://developer.mozilla.org/en/docs/Web/HTML/Element) to add colour to your code.

1. **Bold**:
    + `<b>` or `<strong>`
2. **Italic**:
    + `<i>` or `<em>`

For regular `string` fields, such as `★ Title` you can highlight a code section by wrapping your text in a `code` tag. Something like this:

```html
<!-- ★ Title card field is wrapped in a `h1` -->
<code>{ string = <b>"bold"</b>, italic = <i>42</i> }</code>
```


## Full syntax highlighting

> We use our `code block`s with generated HTML for our pretty colours.
> For beginners, use the [online tool](https://tinyurl.com/mr43ydea).
> If you know how to use `npm` go here.

Currently using Monochrome and [Breeze Dark](../../source/style/modules/variables/breezedark.less) themes. To generate highlighted `code block`s you can follow the steps below. If you know how to use a terminal, there's a [🧑‍🎓 better way](../professional/index.md)!

Basic colours are fine for small lines of code, but you'll probably want to go [full colour](#full-syntax-highlighting) next. Wherever you see a **[`code block`](../simple/index.md#-sample-code-block)**, Anki Theme provides pretty colours (CSS) to use with Markdown and [Pandoc](https://pandoc.org/demo/example18f.html) to generate your code.

1. Write your code as [Markdown fenced code blocks](https://help.github.com/articles/github-flavored-markdown/#fenced-code-blocks),
2. Convert [Markdown to HTML5 online](https://tinyurl.com/mr43ydea),
3. Add a card in Anki,
4. Choose a [`code block`](#!) field,
5. Add your rendered HTML,
6. Press the `A𝐴` button ([`Toggle Visual Editor ⌘⇧X`](https://github.com/badlydrawnrob/anki/issues/62)) to preview your code,
7. Repeat the process — save your card!

That's it. You're done. Simple, right?!


### Customising themes (the easy way)

For quick customisations, view this file:

```text
source
│
└───style
    │
    └───base
        │
        └───variables
              breezedark.less
```

The easiest way to change the colors for the `code string` and `code block` fields is to edit the `--color-code-bold`, `--color-code-italic`, and `--color-code-dark-*` variables in your Anki cards. This will overwrite the defaults.

### How to change your theme colours

> Pandoc has some ready made themes you can use. See [this issue](https://github.com/badlydrawnrob/anki/issues/142) for more info.

1. You'll have the latest [Anki flashcards release](https://github.com/badlydrawnrob/anki/releases).
2. In the Anki app menu, go to `Manage Note Types`.
3. Select the `Anki flashcards: ...` Note Type.
4. Select the `Cards` button.
5. Select the `Styling` option.
6. Copy our `--color-code` variables from `breeze.dark.less`.
7. Add them to the bottom of the `Styling` box, and [edit them](https://github.com/badlydrawnrob/anki/issues/78).
8. Repeat for all Anki flashcard card types

#### Updates to Anki flashcards

If you edit your colors this way, **changes will be lost every time** you download a new release of Anki Flashcards and import them to Anki. See below for a better way.


## Compiling offline and custom themes
### A better way to manage our flashcards

> If you don't want to lose your theme changes everytime a new release of Anki Flashcards is imported to Anki, **you'll need to clone or fork this repo.**

Once you've levelled up your programming skills and the thought of using [terminal](https://en.wikipedia.org/wiki/Command-line_interface) doesn't scare you, you're ready to try your hand at doing things **[🧑‍🎓 the professional way](../professional/index.md)**.

