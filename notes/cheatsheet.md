
<div align=center>
  <h1>Markdown & HTML Cheatsheet (wip)</h1>
For GitHub's profile <code>README.md</code> and other <code>.md</code> files.
</div>

> [!WARNING] TODO:  
> - Add info on Section Links and Custom Anchors 
>   - (Does not expand collapsed/hidden content...)  
> 

<!-- Nested blockquotes -->
<!-- Show html AND markdown versions .. -->

---

## Other Cheetsheets

> - [Check tables with columns](./tables.md)

---

## Links

> [!TIP] 
> - [Basic Syntax Guide](https://www.markdownguide.org/basic-syntax/)
> - [Section Links](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#section-links)
> - [Custom Anchors](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#custom-anchors)
> - [Check Heading Syntax Documentation](https://www.markdownguide.org/basic-syntax/#headings)  
> - []()
> 
> To Check:
> - [Hacks](https://www.markdownguide.org/hacks/#indent-tab)

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

## Formatting, Alignment & Structure

# Text Alignment & Structure


## Headings/Section Titles

<h1>Heading 1</h1>   <!-- Largest -->
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>   <!-- Smallest -->

<details><summary>See the code</summary>

```html
<!-- HTML -->
<h1>Heading 1</h1>   <!-- Largest -->
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>   <!-- Smallest -->
```
```markdown
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
</details>

---

### HTML Tags

| Tag      | Description             | Example Usage                      |
| -------- | ----------------------- | ---------------------------------- |
| `<b>`    | <b>Bold text</b>        | ``<b>Bold Text</b>``               |
| `<i>`    | <i>Italic text</i>      | ``<i>Italic Text</i>``             |
| `<u>`    | <u>Underlined text</u>  | ``<u>Underlined</u>``              |
| `<s>`    | <s>Strikethrough</s>    | ``<s>No longer relevant</s>``      |
| `<mark>` | <mark>Highlighted</mark>| ``<mark>Important!!</mark>``       |
| `<br>`   | Line 1<br>(Line Break)</br>Line 2       | ``Line 1<br>(Line Break)</br>Line 2`` |
| `<hr>`   | — (horizontal rule)     | ``<hr>``                           |
| `<p>`    | <p>Paragraph block</p>  | ``<p>This is a paragraph.</p>``    |
| `<div>`  | Block container         | ``<div align="center">Text</div>`` |
| `<h1>`–`<h6>`          | <h3>Heading levels 1–6</h3> | ``<h3>Heading levels 1–6</h3>``            |
| `<p align="center">`   | Center a paragraph          | ``<p align="center">Centered text.</p>``   |
| `<div align="center">` | Center any block (wrapper)  | ``<div align="center">…</div>`` |
| `<h3 align="center">`  | Center a heading            | ``<h3 align="center">Centered Title</h3>`` |
| `<!-- ... -->`         | Comment (won’t render)             | ``<!-- This is a comment -->``                            |
| `<details>`            | Collapsible content (`<summary>…`) | ``<details><summary>More</summary>Hidden text</details>`` |
| `<code>`               | <code>Inline</code> code           | ``<code>Inline</code> code``                              |

### Markdown Syntax

| Syntax              | Description                  | Example Usage                   |
| ------------------- | ---------------------------- | ------------------------------- |
| `**Bold**`          | **Bold text**                | ``**Bold Text**``               |
| `*Italic*`          | *Italic text*                | ``*Italic Text*``               |
| `~~Strike~~`        | ~~Strikethrough~~            | ``~~Struck Text~~``             |
| `` `code` ``        | `Inline code`                | `` `code` ``                    |
| ` ``` `             | Code block                   | see "Code Block Example” below  |
| `#`–`######`        | Headings levels 1–6          | ``### Subsection Title``        |
| *(blank line)*      | Paragraph separation         | see “Paragraph Example” below   |
| Two trailing spaces | Line break                   | see “Line-Break Example” below  |
| `---`               | Horizontal rule              | ``---``                         |
| `<!-- ... -->`      | Hidden comment (HTML syntax) | ``<!-- Hidden comment -->``     |
| `>`                 | Blockquote                   | `> A quoted sentence`           |

---

#### Markdown Code Block, Paragraph & Line-Break Examples

<details><summary>Code Block example</summary>

```markdown
```js
function greet() {
  console.log("Hello!");
}
```

Will render like this:

```js
function greet() {
  console.log("Hello!");
}
```
</details>

<details> <summary>Paragraph & Line-Break Example</summary>

<p>This is a paragraph.</p>

<p>This is another paragraph.<br>With a line break.</p>

<details><summary>See the code</summary>

```markdown
<p>This is a paragraph.</p>

<p>This is another paragraph.<br>With a line break.</p>
```
</details>

</details>

---

## HTML Entities Reference
> [!NOTE]  
> HTML entities are used to represent special characters
> that would otherwise be interpreted as HTML.  
> [View Full HTML Entities List](https://www.freeformatter.com/html-entities.html)

### Symbols Entities

| Character      | Entity   | Description         | Usage Example (Rendered) |
| -------------- | -------- | ------------------- | ------------------------ |
| `<`            | `&lt;`   | Less than symbol    | &lt;                     |
| `>`            | `&gt;`   | Greater than symbol | &gt;                     |
| `&`            | `&amp;`  | Ampersand           | &amp;                    |
| `"`            | `&quot;` | Double quote        | &quot;                   |
| `'`            | `&apos;` | Single quote        | &apos;                   |

### Whitespace Entities

| Entity     | Name                   | Width Equivalent        | Usage Example (Rendered) |
| ---------- | ---------------------- | ----------------------- | -------------------------|
| `&nbsp;`   | Non-breaking space     | 1 regular space         | Word&nbsp;Word           |
| `&ensp;`   | En space               | \~½ em (about 2 spaces) | Word&ensp;Word           |
| `&emsp;`   | Em space               | \~1 em (about 4 spaces) | Word&emsp;Word           |
| `&thinsp;` | Thin space             | Narrower than en space  | Word&thinsp;Word         |
| `&zwnj;`   | Zero-width non-joiner  | No width, prevents join | Word&zwnj;Word           |
| `&zwj;`    | Zero-width joiner      | No width, enforces join | Word&zwj;Word            |

> [!NOTE]  
> | Unit   | Relative To | Description                                                                    |
> | ------ | ----------- | ------------------------------------------------------------------------------ |
> | **em** | Font size   | 1em = width of the capital letter "M" in the current font (usually full width) |
> | **en** | Half of 1em | 1en = half the width of an em, approximately the width of the letter "N"       |
> 
> So if the font size is 16px:
> - 1em = 16px
> - 1en = 8px

---

<!-- 
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
-->

## TOFIX


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
</details>
```
</details>

---

## Centering Content

### Center a heading:

<h3 align="center">Centered Title</h3>

<details><summary>See the code</summary>

```markdown
<h3 align="center">Centered Title</h3>
```

</details>

### Center a paragraph:
<p align="center">This text is centered.</p>

<details><summary>See the code</summary>

```markdown
<p align="center">This text is centered.</p>
```

</details>

### Center images or icons:

<p align="center">
  <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="Centered GitHub Logo" width="50">
</p>

<details><summary>See the code</summary>

```markdown
<p align="center">
  <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="Centered GitHub Logo" width="50">
</p>
```
</details>

> [!TIP]  You can always center content by placing it between `<div align=center>` and `</div>`
>  <details><summary>See the code</summary>
>  
>  ```markdown
>  <div align=center>
>  
>  Centered content
>  
>  </div>
>  ```
> </details>

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
