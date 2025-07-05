
<div align=center>
  <h1>Markdown & HTML Cheatsheet (wip)</h1>
For GitHub's profile <code>README.md</code> and other <code>.md</code> files.
</div>

> [!WARNING] TODO:  
> Add info on Section Links and Custom Anchors 
>   - (Does not expand collapsed/hidden content...)  
> 

<!-- Nested blockquotes -->
<!-- Show html AND markdown versions .. -->

---

## Other Cheetsheets

> - [Check tables with columns](./tables.md)

---

## Links

- [Basic Syntax Guide](https://www.markdownguide.org/basic-syntax/)
- [Section Links](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#section-links)
- [Custom Anchors](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#custom-anchors)
- []()

To Check:
- [Hacks](https://www.markdownguide.org/hacks/#indent-tab)

---

## Alerts

> [!NOTE]
> Useful information that users should know, even when skimming content.  

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

<details><summary>See the code</summary>

```markdown
> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.
```
</details>

---

## Headings/Section Titles

<h1>Heading 1</h1>   <!-- Largest -->
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>   <!-- Smallest -->

<details><summary>See the code</summary>

```markdown
<!-- HTML -->
<h1>Heading 1</h1>   <!-- Largest -->
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>   <!-- Smallest -->

<!-- Markdown -->
# Heading 1          <!-- Largest -->
## Heading 2
### Heading 3
####  Heading 4
#####  Heading 5
######  Heading 6    <!-- Smallest -->

<!-- Alternate Syntax -->
Heading 1 alt
=============

Heading 2 alt
-------------
```

> [!TIP] [Check Heading Syntax Documentation](https://www.markdownguide.org/basic-syntax/#headings)  

</details>

---

## Paragraphs & Line Breaks

<p>This is a paragraph.</p>

<p>This is another paragraph.<br>With a line break.</p>

<details><summary>See the code</summary>

```markdown
<p>This is a paragraph.</p>

<p>This is another paragraph.<br>With a line break.</p>
```
</details>

---

## Collapsible Content
<details>
  <summary>Click to expand!</summary>
  Hidden text here.
</details>

<details><summary>See the code</summary>

```markdown
<details>
  <summary>Click to expand!</summary>
  Hidden text here.
  (links to sections of text do not open hidden text..)
</details>
```
</details>


---

## Horizontal Line `(<hr>)`

<!-- HTML -->
<hr>

<!-- Markdown -->
---

<details><summary>See the code</summary>

```markdown
<!-- HTML -->
<hr>

<!-- Markdown -->
---
```

</details>

---

## Commenting Code `(<!-- -->)`
<div align="center"><h2></h2></div>

<!-- This is a comment. It won't be displayed. -->

<details><summary>See the code</summary>

```markdown
<!-- This is a comment. It won't be displayed. -->
```
</details>

---

## Basic Formatting Tags

| Tag         | Description                                          | Example Usage                   |
|-------------|------------------------------------------------------|---------------------------------|
| `<div>`     | Defines a block container (**useful for alignment**) | `<div align="center">...</div>` |
| `<p>`       | Creates a paragraph                                  | `<p>This is a paragraph.</p>`   |
| `<br>`      | Adds a line break (new line)                         | `Line 1 <br> Line 2`            |
| `<b>`       | **Bold text**                                        | `<b>Bold Text</b>`              |
| `<i>`       | *Italic text*                                        | `<i>Italic Text</i>`            |
| `<u>`       | _Underlined text_                                    | `<u>Underlined</u>`             |
| `<s>`       | ~~Strikthrough text~~                                | `<s>No longer relevant</s>`     |
| `<hr>`      | Creates a horizontal divider                         | `<hr>`                          |


### Advanced Formatting Tags

## Highlight Tag

| Tag       | Description                 | Example Usage                       |
|-----------|-----------------------------|-------------------------------------|
| `<mark>`  | <mark>Highlight</mark> text | `<mark>Important!!</mark>`          |


<table>
  <tr>
    <th>Tag</th>
    <th>Description</th>
    <th>Example Usage</th>
  </tr>
  <tr>
    <td>&lt;mark&gt;</td>
    <td><mark>Highlighted</mark> text</td>
    <td>&lt;mark&gt;Important!!&lt;/mark&gt;</td>
  </tr>
</table>

### Combined Table (WIP)

| Tag/Markdown | Description            | Example Usage                        | Rendered Output               |
|--------------|------------------------|--------------------------------------|-------------------------------|
| `<mark>`     | Highlight text (HTML)  | `<mark>Important!</mark>`            | <mark>Important!</mark>       |
| `**`         | Bold (Markdown)        | `**bold**`                           | **bold**                      |
| `*`          | Italic (Markdown)      | `*italic*`                           | *italic*                      |
| `<u>`        | Underline (HTML)       | `<u>underlined</u>`                  | <u>underlined</u>             |
| `~~`         | Strikethrough (MD)     | `~~not needed~~`                     | ~~not needed~~                |

| Tag / Syntax     | Type      | Description     | Example Usage                   | Rendered Output                    |
| ---------------- | --------- | --------------- | ------------------------------- | ---------------------------------- |
| `<b>` / `**`     | HTML / MD | Bold            | `<b>Bold</b>` / `**Bold**`      | <b>Bold</b> / **Bold**             |
| `<i>` / `*`      | HTML / MD | Italic          | `<i>Italic</i>` / `*Italic*`    | <i>Italic</i> / *Italic*           |
| `<u>`            | HTML      | Underline       | `<u>Underlined</u>`             | <u>Underlined</u>                  |
| `<s>` / `~~`     | HTML / MD | Strikethrough   | `<s>Struck</s>` / `~~Struck~~`  | <s>Struck</s> / \~\~Struck\~\~\~\~ |
| `<mark>`         | HTML      | Highlight       | `<mark>Important</mark>`        | <mark>Important</mark>             |
| `<br>`           | HTML      | Line Break      | `Line 1<br>Line 2`              | Line 1<br>Line 2                   |
| `<hr>`           | HTML      | Horizontal Line | `<hr>`                          | <hr>                               |
| `<p>`            | HTML      | Paragraph Block | `<p>This is a paragraph.</p>`   | <p>This is a paragraph.</p>        |
| `<div>`          | HTML      | Block Container | `<div align="center">...</div>` | (May not render visibly on GitHub) |
| `#`, `##`, `###` | Markdown  | Headings        | `## Subheading`                 | ## Subheading                      |
| `>`              | Markdown  | Blockquote      | `> A quoted sentence`           | > A quoted sentence                |
| `` `code` ``     | Markdown  | Inline code     | `` `console.log()` ``           | `console.log()`                    |
| ` ``` `          | Markdown  | Code block      | ` ```js\nalert("Hi")\n``` `     | (see below)                        |

> <details><summary>See example</summary>
> <pre> ```js function greet() { console.log("Hello!"); } ``` </pre>  
> Will render like this:
> ```js
> function greet() {
>   console.log("Hello!");
> }
> ```
> </details>


---

## HTML Entities

<!--

Escape '<' :
  &lt;
Escape '>' :
  &gt;

Inserting Whitespace:

`&nbsp;` to add a single space. ->&nbsp;<-  
`&ensp;` to add 2 spaces. ->&ensp;<-  
`&emsp;` to add 4 spaces. ->&emsp;<-  

-->

HTML entities are used to represent special characters that would otherwise be interpreted as HTML:

| Character | Entity | Meaning               |
|-----------|--------|-----------------------|
| `<`       | `&lt;` | "less than" symbol    |
| `>`       | `&gt;` | "greater than" symbol |

---
