Markdown Style Guide
====================

> Markdown is not a replacement for HTML, or even close to it. Its syntax is
> very small, corresponding only to a very small subset of HTML tags.&hellip;The idea for Markdown is to
> make it easy to read, write, and edit prose. HTML is a _publishing_ format;
> Markdown is a _writing_ format.

— [Markdown Syntax Documentation][markdown-syntax]

Document Structure
------------------

Markdown documents should follow the following structure:

1. YAML front matter
2. Content
3. Link label definitions
4. Image label definitions

Headings
--------

- Underline `h1` elements using equals signs `=`
- Underline `h2` elements using hyphens `-`
- Use multiple hashes `#` for `h3` through `h6`
- Use a single blank new line after all headings

```
This is an h1
=============

This is an h2
-------------

### h3

#### h4

##### h5

###### h6
```

Lists
-----

- Use hyphens `-` for unordered list items
- Use numbers followed by periods `1.` for ordered list items
- Insert a single space following list item markers
- Don't wrap text inside list items

```
- This is an unordered list item
  - This is a nested unordered list item
- This is an unordered list item
  1. This is an ordered list item
```

Code Blocks
-----------

- Identify a code block by using triple backticks <code>&#96;&#96;&#96;</code>
- Label the code block language (if using a compatible code highlighter)

<!-- The following code block is indented to prevent backticks from being parsed literally. Use the backtick syntax for all other code blocks. -->

    ```sass
      .card
        background: $c-background-invert
        border-radius: $b-borderRadius
        box-shadow: $b-boxShadow
        padding: $b-space
        position: relative
    ```

Blockquotes
-----------

- Wrap lines at 80 characters
- Use a "greater than" character `>` to begin each line
  - Insert a single space following each "greater than" character
- Place attribution following the blockquote after one blank new line.

```
> If you copy an entire article from this site and republish it on your own
> site like you wrote it, that's a little uncool. I won't be mad at you for
> stealing, I just think you're better than that and want to see you do better.

— [CSS-Tricks License][csstricks-license]
```

Emphasis
--------

- Use underscores `_` to emphasize inline text

```markdown
One of these words has _stress_ emphasis.
```

Strong
------

- Use double asterisks `**` to strengthen inline text

```markdown
One of these words has **strong** importance.
```

Links
-----

- Label all links at the bottom of the Markdown file.
- Use only lowercase letters when labeling links.
- Use hyphens to separate words in a link label.

<!-- The following code block is indented to prevent link label definitions from being parsed literally. Use the backtick syntax for all other code blocks. -->

    This paragraph contains a link to a CSS-Tricks [blog post][csstricks-prefill-forms].

    [csstricks-prefill-forms]: http://css-tricks.com/prefill-forms-dev/

Images
------

- Label all images beneath the document's content.
- Use only lowercase letters when labeling images.
- Use hyphens to separate words in an image label.

<!-- The following code block is indented to prevent iamge label definitions from being parsed literally. Use the backtick syntax for all other code blocks. -->

    Check out this sweet GIF:
    ![Coding in a nutshell][gif-coding]

    [gif-coding]: http://gificiency.com/m/codinginanutshell.gif

HTML
----

> For any markup that is not covered by Markdown's syntax, you simply use HTML
> itself. There's no need to preface it or delimit it to indicate that you're
> switching from Markdown to HTML; you just use the tags.

— [Markdown Syntax Documentation][markdown-syntax]

[markdown-syntax]: http://daringfireball.net/projects/markdown/syntax
