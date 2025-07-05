
# Tables

## Tables `(<table>)`
<div align="center"><h2></h2></div>

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


# Tables and Columns Markdown Cheat Sheet

## Basic 2-column layout with image + content


```markdown
<table>
  <tr>
	<!-- LEFT COLUMN -->
	<td style="vertical-align: top; padding-right: 1rem;">
	  <!-- Example image -->
	  <img src="./assets/your-image.png" alt="Alt text" width="120"/>
	</td>
	<!-- RIGHT COLUMN -->
	<td style="vertical-align: top;">
	  <!-- Nested table for aligned key-value pairs -->
	  <table>
		<tr>
		  <td style="padding-right: 0.5rem;"><strong>Label 1</strong>:</td>
		  <td>Value 1</td>
		</tr>
		<tr>
		  <td style="padding-right: 0.5rem;"><strong>Label 2</strong>:</td>
		  <td>Value 2</td>
		</tr>
		<tr>
		  <td style="padding-right: 0.5rem;"><strong>Label 3</strong>:</td>
		  <td>Multiline<br>With breaks<br>Still aligned</td>
		</tr>
	  </table>
	</td>
  </tr>
</table>
<!-- Optional: continue below with full-width content -->
<p><strong>Section Title</strong>:</p>
<ul>
  <li>List item 1</li>
  <li>List item 2</li>
</ul>
```

### Result:

<table>
  <tr>
	<!-- LEFT COLUMN -->
	<td style="vertical-align: top; padding-right: 1rem;">
	  <!-- Example image -->
	  <img src="./assets/your-image.png" alt="Alt text" width="120"/>
	</td>
	<!-- RIGHT COLUMN -->
	<td style="vertical-align: top;">
	  <!-- Nested table for aligned key-value pairs -->
	  <table>
		<tr>
		  <td style="padding-right: 0.5rem;"><strong>Label 1</strong>:</td>
		  <td>Value 1</td>
		</tr>
		<tr>
		  <td style="padding-right: 0.5rem;"><strong>Label 2</strong>:</td>
		  <td>Value 2</td>
		</tr>
		<tr>
		  <td style="padding-right: 0.5rem;"><strong>Label 3</strong>:</td>
		  <td>Multiline<br>With breaks<br>Still aligned</td>
		</tr>
	  </table>
	</td>
  </tr>
</table>
<!-- Optional: continue below with full-width content -->
<p><strong>Section Title</strong>:</p>
<ul>
  <li>List item 1</li>
  <li>List item 2</li>
</ul>

---

### Quick Reference for Attributes
| Attribute               | Purpose                                                  |
| ----------------------- | -------------------------------------------------------- |
| `vertical-align: top;`  | Aligns top of content in table cells (no center gaps)    |
| `padding-right: 1rem;`  | Adds spacing between image/labels and content            |
| `<table>...</table>`    | Defines a table structure (used in HTML inside Markdown) |
| `<td>`                  | Table data (i.e., a cell)                                |
| `<tr>`                  | Table row                                                |
| `<br>`                  | Line break (inside table cells or paragraphs)            |
| `<ul><li>...</li></ul>` | Standard Markdown bullet list                            |

---

### Example Output (visual):
```mathematica
+-------------------------+--------------------------------------------+
|    [   Image here   ]   | Label 1: Value 1                           |
|                         | Label 2: Value 2                           |
|                         | Label 3: Multiline                         |
|                         |          With breaks                       |
+-------------------------+--------------------------------------------+
```

---

> [!TIP]  
> - Always use inline styles like `style="..."` — GitHub ignores `<style>` blocks.  
> - Nested `<table>` inside the right column is the key to aligned key-value data.  
> - Lists (`<ul>`) introduce indents. Use `<br>` inside `<td>` if you want tighter alignment.  

---

## 3-Column Layout with Centered Alignment

```markdown
<p align="center">
  <table>
	<tr>
	  <!-- COLUMN 1 -->
	  <td style="text-align: center; vertical-align: top; padding: 1rem;">
		<img src="./assets/icon-1.png" alt="Icon 1" width="80"/><br>
		<strong>Column 1</strong><br>
		Description A<br>
		Description B
	  </td>
	  <!-- COLUMN 2 -->
	  <td style="text-align: center; vertical-align: top; padding: 1rem;">
		<img src="./assets/icon-2.png" alt="Icon 2" width="80"/><br>
		<strong>Column 2</strong><br>
		Description A<br>
		Description B
	  </td>
	  <!-- COLUMN 3 -->
	  <td style="text-align: center; vertical-align: top; padding: 1rem;">
		<img src="./assets/icon-3.png" alt="Icon 3" width="80"/><br>
		<strong>Column 3</strong><br>
		Description A<br>
		Description B
	  </td>
	</tr>
  </table>
</p>
```

### Result:

<p align="center">
  <table>
	<tr>
	  <!-- COLUMN 1 -->
	  <td style="text-align: center; vertical-align: top; padding: 1rem;">
		<img src="./assets/icon-1.png" alt="Icon 1" width="80"/><br>
		<strong>Column 1</strong><br>
		Description A<br>
		Description B
	  </td>
	  <!-- COLUMN 2 -->
	  <td style="text-align: center; vertical-align: top; padding: 1rem;">
		<img src="./assets/icon-2.png" alt="Icon 2" width="80"/><br>
		<strong>Column 2</strong><br>
		Description A<br>
		Description B
	  </td>
	  <!-- COLUMN 3 -->
	  <td style="text-align: center; vertical-align: top; padding: 1rem;">
		<img src="./assets/icon-3.png" alt="Icon 3" width="80"/><br>
		<strong>Column 3</strong><br>
		Description A<br>
		Description B
	  </td>
	</tr>
  </table>
</p>

---

### Example Use Cases

| Layout Purpose     | Column Content Example                        |
| ------------------ | --------------------------------------------- |
| Skill cards        | Icon • Skill name • Tooltip-style description |
| Tech stack tiers   | Languages • Tools • DevOps                    |
| RPG stats          | Strength • Intelligence • Dexterity           |
| Achievement badges | Bronze • Silver • Gold                        |

--- 
> [!TIP]  
> - Wrap in `<p align="center">...</p>` for horizontal centering in GitHub Markdown.
> - Use `text-align: center` in `<td>` to center contents vertically *within each cell*.
> - Change `width="80"` to control image size.
> - Add or remove `<td>` blocks to make 2 or 4 column layouts with the same pattern.
