
> *TODO!* -> Show html AND markdown versions ..   

# Markdown & HTML Cheatsheet
For GitHub's profile `README.md` and other `.md` files.

---

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

## Headings

<h1>Heading 1</h1>   <!-- Largest -->
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>   <!-- Smallest -->

<details><summary>See the code</summary>

```markdown
<h1>Heading 1</h1>   <!-- Largest -->
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>   <!-- Smallest -->
```

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

## Links `(<a>)`
<a href="https://example.com">Visit Example</a>

<a href="https://example.com" target="_blank" rel="noreferrer">Open in New Tab</a>

<details><summary>See the code</summary>

```markdown
<a href="https://example.com">Visit Example</a>

<a href="https://example.com" target="_blank" rel="noreferrer">Open in New Tab</a>
```
</details>

---

## Images `(<img>)`
<img src="https://via.placeholder.com/150" alt="Example Image" width="100">

<details><summary>See the code</summary>

```markdown
<img src="https://via.placeholder.com/150" alt="Example Image" width="100">
```
</details>

### Adding Clickable Images (Icon with Link)
<a href="https://github.com">
  <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="40">
</a>

<details><summary>See the code</summary>

```markdown
<a href="https://github.com">
  <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="40">
</a>
```
</details>

---

## Lists

### Unordered List `(<ul>)` (Bullets)
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<details><summary>See the code</summary>

```markdown
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```
</details>

### Ordered List `(<ol>)` (Numbers)
<ol>
  <li>First</li>
  <li>Second</li>
  <li>Third</li>
</ol>

<details><summary>See the code</summary>

```markdown
<ol>
  <li>First</li>
  <li>Second</li>
  <li>Third</li>
</ol>
```
</details>

### Description List `(<dl>)`
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>

<details><summary>See the code</summary>

```markdown
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```
</details>

---

## Tables `(<table>)`
> [Check tables with columns](./tables-and-column-info.md)  

<table>
  <tr>
    <th>Column 1</th>
    <th>Column 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>

<details><summary>See the code</summary>

```markdown
<table>
  <tr>
    <th>Column 1</th>
    <th>Column 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>
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
  <img src="https://via.placeholder.com/100" width="50">
</p>

<details><summary>See the code</summary>

```markdown
<p align="center">
  <img src="https://via.placeholder.com/100" width="50">
</p>
```
</details>

---

## Horizontal Line `(<hr>)`
<hr>

<details><summary>See the code</summary>

```markdown
<hr>
```

`---` also works.

</details>

---

## Inserting Whitespace
`&nbsp;` to add a single space. ->&nbsp;<-  
`&ensp;` to add 2 spaces. ->&ensp;<-  
`&emsp;` to add 4 spaces. ->&emsp;<-  

## Commenting Code `(<!-- -->)`
<!-- This is a comment. It won't be displayed. -->

<details><summary>See the code</summary>

```markdown
<!-- This is a comment. It won't be displayed. -->
```
</details>

---

## ASCII Art Centering

### `<pre>`

Why Use `<pre>`?
  - Maintains exact formatting (spaces, new lines, indentation).
  - Keeps ASCII art properly aligned inside a `<div>`.
  - Ensures GitHub README renders ASCII art exactly as written.

### Example Without `<pre>` (Incorrect Formatting)
<div align="center">
██╗███╗   ██╗████████╗ █████╗  ██████╗████████╗
██║████╗  ██║╚══██╔══╝██╔══██╗██╔════╝╚══██╔══╝
██║██╔██╗ ██║   ██║   ███████║██║        ██║   
██║██║╚██╗██║   ██║   ██╔══██║██║        ██║   
██║██║ ╚████║   ██║   ██║  ██║╚██████╗   ██║   
╚═╝╚═╝  ╚═══╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝   ╚═╝   
</div>

<details><summary>See the code</summary>

```markdown
<div align="center">
██╗███╗   ██╗████████╗ █████╗  ██████╗████████╗
██║████╗  ██║╚══██╔══╝██╔══██╗██╔════╝╚══██╔══╝
██║██╔██╗ ██║   ██║   ███████║██║        ██║   
██║██║╚██╗██║   ██║   ██╔══██║██║        ██║   
██║██║ ╚████║   ██║   ██║  ██║╚██████╗   ██║   
╚═╝╚═╝  ╚═══╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝   ╚═╝   
</div>
```
</details>

### Correct Example With `<pre>` (Recommended)
<div align="center">
<pre>
██╗███╗   ██╗████████╗ █████╗  ██████╗████████╗
██║████╗  ██║╚══██╔══╝██╔══██╗██╔════╝╚══██╔══╝
██║██╔██╗ ██║   ██║   ███████║██║        ██║   
██║██║╚██╗██║   ██║   ██╔══██║██║        ██║   
██║██║ ╚████║   ██║   ██║  ██║╚██████╗   ██║   
╚═╝╚═╝  ╚═══╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝   ╚═╝   
</pre>
</div>

<details><summary>See the code</summary>

```markdown
<div align="center">
<pre>
██╗███╗   ██╗████████╗ █████╗  ██████╗████████╗
██║████╗  ██║╚══██╔══╝██╔══██╗██╔════╝╚══██╔══╝
██║██╔██╗ ██║   ██║   ███████║██║        ██║   
██║██║╚██╗██║   ██║   ██╔══██║██║        ██║   
██║██║ ╚████║   ██║   ██║  ██║╚██████╗   ██║   
╚═╝╚═╝  ╚═══╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝   ╚═╝   
</pre>
</div>
```
</details>

---

## Basic Formatting Tags
| Tag     | Description                                          | Example Usage                   |
| ------- | ---------------------------------------------------- | ------------------------------- |
| `<div>` | Defines a block container (**useful for alignment**) | `<div align="center">...</div>` |
| `<p>`   | Creates a paragraph                                  | `<p>This is a paragraph.</p>`   |
| `<br>`  | Adds a line break (new line)                         | `Line 1 <br> Line 2`            |
| `<b>`   | **Bold text**                                        | `<b>Bold Text</b>`              |
| `<i>`   | *Italic text*                                        | `<i>Italic Text</i>`            |
| `<u>`   | _Underlined text_                                    | `<u>Underlined</u>`             |
| `<s>`   | ~~Strikthrough text~~                                | `<s>No longer relevant</s>`     |
| `<hr>`  | Creates a horizontal divider                         | `<hr>`                          |

---

## Text Alignment & Structure
| Tag                    | Description                            | Example Usage                                   |
| ---------------------- | -------------------------------------- | ----------------------------------------------- |
| `<h1>` - `<h6>`        | Headings (h1 = biggest, h6 = smallest) | `<h1>Title</h1>`                                |
| `<div align="center">` | Centers content inside                 | `<div align="center"><h1>Title</h1></div>`      |
| `<div align="right">`  | Aligns content to the right            | `<div align="right"><p>Right-aligned</p></div>` |
| `<blockquote>`         | Indents a quote block                  | `<blockquote>Quoted Text</blockquote>`          |

---

## Links & Images
| Tag             | Description              | Example Usage                                                      |
| --------------- | ------------------------ | ------------------------------------------------------------------ |
| `<a href="">`   | Creates a clickable link | `<a href="https://github.com">GitHub</a>`                          |
| `<img>`         | Displays an image        | `<img src="logo.png" width="100">`                                 |
| `<a>` + `<img>` | Clickable image link     | `<a href="https://github.com"><img src="logo.png" width="40"></a>` |

---
