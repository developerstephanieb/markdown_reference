# Markdown Reference

A comprehensive guide to the most commonly used Markdown syntax.

---

## Table of Contents

- [Markdown Reference](#markdown-reference)
  - [Table of Contents](#table-of-contents)
  - [Headers](#headers)
  - [Text Formatting](#text-formatting)
  - [Lists](#lists)
    - [Unordered Lists](#unordered-lists)
    - [Ordered Lists](#ordered-lists)
    - [Task Lists](#task-lists)
  - [Blockquotes](#blockquotes)
  - [Horizontal Rule](#horizontal-rule)
  - [Links](#links)
  - [Images](#images)
  - [Code](#code)
    - [Inline Code](#inline-code)
    - [Fenced Code Blocks](#fenced-code-blocks)
  - [Tables](#tables)
  - [Reference-Style Links and Images](#reference-style-links-and-images)
  - [Linking to Headers (Table of Contents)](#linking-to-headers-table-of-contents)
  - [Escaping Characters](#escaping-characters)
  - [Math (Using LaTeX)](#math-using-latex)
    - [Inline Math](#inline-math)
    - [Block Equations](#block-equations)
  - [Using HTML (Comments)](#using-html-comments)

---

## Headers

Headers are created using the `#` symbol. The number of `#` symbols corresponds to the header level.

```markdown
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
```

---

## Text Formatting

Text can be formatted to be bold, italic, or have a strikethrough.

| Style         | Syntax                       | Example                       |
| ------------- | ---------------------------- | ----------------------------- |
| Bold          | `**text**` or `__text__`     | **This is bold text**         |
| Italic        | `*text*` or `_text_`         | *This is italic text*         |
| Strikethrough | `~~text~~`                   | ~~This is strikethrough~~     |
| Bold & Italic | `***text***` or `___text___` | ***This is bold and italic*** |


---

## Lists

### Unordered Lists

Use `*`, `+`, or `-` to create unordered lists.

```markdown
* Item 1
+ Item 2
  - Nested Item 2a
  * Nested Item 2b
+ Item 3
```

**Output**:
* Item 1
+ Item 2
  - Nested Item 2a
  * Nested Item 2b
+ Item 3

### Ordered Lists

Use numbers followed by a period.

```markdown
1. First item
2. Second item
3. Third item
   1. Nested item 3a
   2. Nested item 3b
```

**Output**:
1. First item
2. Second item
3. Third item
   1. Nested item 3a
   2. Nested item 3b

### Task Lists

Create task lists (checkboxes) within a list.

```markdown
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task
```

**Output**:
- [x] Completed task
- [ ] Incomplete task
- [ ] Another task

---

## Blockquotes

Blockquotes are used to indicate quoted text.

```markdown
> This is a blockquote.
>
> > This is a nested blockquote.
```

**Output**:
> This is a blockquote.
>
> > This is a nested blockquote.

---

## Horizontal Rule

Create a horizontal rule with three or more asterisks `***`, dashes `---`, or underscores `___`.

---

## Links

Create links to navigate to other pages or websites.

```markdown
[Google](https://www.google.com "Link to Google")
```

**Output**:
[Google](https://www.google.com "Link to Google")

---

## Images

The syntax for images is similar to links, but with a `!` at the beginning.

```markdown
![A placeholder image](https://placehold.co/400x200/EEE/31343C?text=Placeholder+Image "Placeholder Image")
```

**Output**:   
![A placeholder image](https://placehold.co/400x200/EEE/31343C?text=Placeholder+Image "Placeholder Image")

---

## Code

### Inline Code

Wrap code with single backticks `` ` ``.

```markdown
This is an example of `inline code`.
```

**Output**:
This is an example of `inline code`.

### Fenced Code Blocks

Use triple backticks ` ``` ` to create a code block. You can also specify the language for syntax highlighting.

````markdown
```javascript
function greet() {
  console.log("Hello, world!");
}
```
````

**Output**:
```javascript
function greet() {
  console.log("Hello, world!");
}
```

---

## Tables

Tables are created using pipes `|` and hyphens `-`.

```markdown
| Header 1 | Header 2 | Header 3 |
| :------- | :------: | -------: |
| Align L  |  Center  |  Align R |
| Cell 4   |  Cell 5  |   Cell 6 |
```

**Output**:
| Header 1 | Header 2 | Header 3 |
| :------- | :------: | -------: |
| Align L  |  Center  |  Align R |
| Cell 4   |  Cell 5  |   Cell 6 |

---

## Reference-Style Links and Images

Use reference-style links when reusing the same URLs.

```markdown
Learn more about [GitHub][gh] and [Stack Overflow][so] for coding help.

[gh]: https://github.com "GitHub Homepage"
[so]: https://stackoverflow.com "Stack Overflow Q&A"
```

**Output**:

Learn more about [GitHub][gh] and [Stack Overflow][so] for coding help.

[gh]: https://github.com "GitHub Homepage"
[so]: https://stackoverflow.com "Stack Overflow Q&A"

---

## Linking to Headers (Table of Contents)

Use internal links to jump to specific headers within the same document.

```markdown
- [Jump to Escaping Characters](#escaping-characters)
- [Jump to Math (Using LaTeX)](#math-using-latex)
  - [Inline Math](#inline-math)
  - [Block Equations](#block-equations)
```

- [Jump to Escaping Characters](#escaping-characters)
- [Jump to Math (Using LaTeX)](#math-using-latex)
  - [Inline Math](#inline-math)
  - [Block Equations](#block-equations)

---

## Escaping Characters

To display a literal character that has special meaning in Markdown, use a backslash `\` before it.

```markdown
\*This is not italic.\*
```

**Output**:
\*This is not italic.\*

---

## Math (Using LaTeX)

For mathematical and scientific notation, many Markdown renderers support LaTeX.

### Inline Math

Wrap equations in single dollar signs `$` for inline math.

```markdown
The Pythagorean theorem is $a^2 + b^2 = c^2$.
```

**Output**:
The Pythagorean theorem is $a^2 + b^2 = c^2$.

### Block Equations

Wrap equations in double dollar signs `$$` to display it as a centered block on its own line.

```markdown
The quadratic formula is:
$$x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$$
```

**Output**:   
The quadratic formula is:
$$x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$$

---

## Using HTML (Comments)

Use raw HTML for features Markdown doesn't support, like comments and collapsible sections.

```html
<!-- This is a comment -->

<details>
  <summary>Click to expand!</summary>
  
  This content is hidden by default but is revealed when you click the summary text.
  You can even include **Markdown** `inside` HTML.
</details>
```

**Output**:
<details>
  <summary>Click to expand!</summary>
  
  This content is hidden by default but is revealed when you click the summary text.
  You can even include **Markdown** `inside` HTML.
</details>
