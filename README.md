# HTML_CSS
Trying to add my learnings of HTML and CSS.

## **HTML (HyperText Markup Language)** 
HTML defines the basic structure of a website, similar to the skeleton of a webpage.

### Basic HTML Tags
- `<html></html>`, `<head></head>`, `<body></body>`: These are the fundamental tags required in any `index.html` file.
- `<title></title>`: Defines the text that will be visible in the browser tab or window title.
- `<!-- -->`: Used to insert comments in the code that won’t be displayed on the webpage.
- `<h1>` to `<h6>`: Heading tags. `<h1>` is the largest and `<h6>` the smallest.
- `<p></p>`: Defines a paragraph of text.
- `<pre></pre>`: Preserves the format of the text, including spaces, line breaks, and indentation.

### Anchor Tags (Hyperlinks)
- `<a></a>`: Anchor tags create hyperlinks. Attributes include:
  - **`href`**: Specifies the URL or path to the linked document. There are two types of URLs:
    - **Absolute URL**: Full web address starting with the protocol (e.g., `http://` or `https://`), pointing to a specific location on the internet.
    - **Relative URL**: A path relative to the current page or website (e.g., linking to another HTML or CSS file within the project).
  - **`target="_blank"`**: Opens the linked document in a new tab.
  - **`title`**: Displays additional information when you hover over the link.

### Audio and Video Tags
- Both `<audio>` and `<video>` tags are used to embed media on a webpage. The common attributes for both tags are:
  - `controls`: Displays playback controls (e.g., play, pause, volume).
  - `autoplay`: Automatically plays the media once the page loads.
  - `muted`: Mutes the media on load; the user can manually unmute it.
  - `loop`: Repeats the media continuously.

### Self-Closing Tags
- `<br>`: Inserts a line break.
- `<hr>`: Inserts a horizontal line.
- `<img>`: Adds images to the webpage, with attributes such as:
  - `src`: Specifies the image source.
  - `alt`: Alternative text for the image, used for accessibility or when the image fails to load.
  - `height`, `width`: Set the dimensions of the image.
 
## Text Formatting in HTML

### 1. **Bold Text**
- **Tag**: `<b></b>` 
- **Use**: To make text bold.
- **Example**: 
    ```html
    <b>This is bold text</b>
    ```
- **Output**: This is bold text

### 2. **Italic Text**
- **Tag**: `<i></i>`
- **Use**: To make text italicized.
- **Example**:
    ```html
    <i>This is italic text</i>
    ```
- **Output**: *This is italic text*

### 3. **Underlined Text**
- **Tag**: `<u></u>`
- **Use**: To underline text.
- **Example**:
    ```html
    <u>This is underlined text</u>
    ```
- **Output**: <u>This is underlined text</u>

### 4. **Strikethrough (Deleted) Text**
- **Tag**: `<del></del>`
- **Use**: To show text that is "deleted" or struck through.
- **Example**:
    ```html
    <del>This is deleted text</del>
    ```
- **Output**: ~~This is deleted text~~

### 5. **Bigger Text**
- **Tag**: `<big></big>`
- **Use**: To display larger text than the surrounding content.
- **Example**:
    ```html
    <big>This text is bigger</big>
    ```
- **Output**: <big>This text is bigger</big>

### 6. **Smaller Text**
- **Tag**: `<small></small>`
- **Use**: To display smaller text than the surrounding content.
- **Example**:
    ```html
    <small>This text is smaller</small>
    ```
- **Output**: <small>This text is smaller</small>

### 7. **Subscript Text**
- **Tag**: `<sub></sub>`
- **Use**: To place text slightly below the normal line, like in chemical formulas.
- **Example**:
    ```html
    H<sub>2</sub>O
    ```
- **Output**: H<sub>2</sub>O

### 8. **Superscript Text**
- **Tag**: `<sup></sup>`
- **Use**: To place text slightly above the normal line, like in exponents.
- **Example**:
    ```html
    E = mc<sup>2</sup>
    ```
- **Output**: E = mc<sup>2</sup>

### 9. **Monospaced (Teletype) Text**
- **Tag**: `<tt></tt>`
- **Use**: To display text in a monospaced (equal-width) font, commonly used for code snippets.
- **Example**:
    ```html
    <tt>This is monospaced text</tt>
    ```
- **Output**: <tt>This is monospaced text</tt>

### 10. **Highlighted Text**
- **Tag**: `<mark></mark>`
- **Use**: To highlight text with a background color.
- **Example**:
    ```html
    <mark>This text is highlighted</mark>
    ```
- **Output**: <mark>This text is highlighted</mark>
- You can also change the highlight color using inline CSS:
    ```html
    <mark style="background-color: lightgreen;">This is highlighted in light green</mark>
    ```
- **Output**: <mark style="background-color: lightgreen;">This is highlighted in light green</mark>
---
## Grouping Content in HTML

### 1. **Using `<span>` for Inline Grouping** 
The `<span>` tag is used to group inline elements, typically for styling. It's like a small highlighter that only applies to the text or elements inside it.
- Tag: `<span></span>`
- **Example**:
    ```html
    <span style="color: red;">This text is grouped inline and colored red</span>
    ```
- What to Remember: The `<span>` tag does not create a new line. It’s perfect when you want to apply styles to a specific part of the content without breaking the flow of text.

### 2. **Using `<div>` for Block Grouping**
 The `<div>` tag is used to group block-level elements. Unlike `<span>`, it creates a new line and takes up the full width of its container.
- Tag: `<div></div>`
- **Example**:
    ```html
    <div style="background-color: lightblue;">
      This is grouped as a block element.
    </div>
    ```
- What to Remember: Think of `<div>` like a container for larger sections of your webpage. It separates content and makes it easy to apply styles to whole sections.

---

## Creating Lists in HTML

Lists are a great way to organize content. Whether it’s a simple bullet-point list or a structured description, here’s how you can use lists in HTML:

### 1. **Unordered List (Bullets)**
To create a list where each item is preceded by a bullet.
- Tag: `<ul></ul>` for the list, `<li></li>` for each item.
- **Example**:
    ```html
    <ul>
      <li>Apples</li>
      <li>Bananas</li>
      <li>Oranges</li>
      <ul>
        <li>Valencia</li>
        <li>Navel</li>
      </ul>
    </ul>
    ```
- **Output**:
    - Apples
    - Bananas
    - Oranges
      - Valencia
      - Navel

- What to Remember: You can easily nest lists by adding another `<ul>` or `<ol>` inside an `<li>`. In the example above, "Oranges" contains a nested list of different types of oranges.

### 2. **Ordered List (Numbered)**
 To create a list where each item is numbered.
- Tag: `<ol></ol>` for the list, `<li></li>` for each item.
- **Example**:
    ```html
    <ol>
      <li>First step</li>
      <li>Second step</li>
      <li>Third step</li>
      <ol>
        <li>Sub-step 3.1</li>
        <li>Sub-step 3.2</li>
      </ol>
    </ol>
    ```
- **Output**:
    1. First step
    2. Second step
    3. Third step
        1. Sub-step 3.1
        2. Sub-step 3.2

- What to Remember: Ordered lists automatically generate numbers for you, and you can nest them too. The sub-steps (3.1, 3.2) are created by adding another `<ol>` inside the third `<li>`.

### 3. **Description List (Key-Value Pairs)**
To create a list of terms and descriptions, similar to a dictionary or glossary.
- Tag: `<dl><dt><dd></dd></dt></dl>`
- **Example**:
    ```html
    <dl>
      <dt>HTML</dt>
      <dd>HyperText Markup Language</dd>
      <dt>CSS</dt>
      <dd>Cascading Style Sheets</dd>
    </dl>
    ```
- **Output**:
    - **HTML**: HyperText Markup Language
    - **CSS**: Cascading Style Sheets

- What to Remember: The `<dt>` tag is for the term, and the `<dd>` tag is for its description. This is useful when you need to define terms or present data in a key-value format.

---

## **CSS (Cascading Style Sheets)** 
CSS adds style to a web page, acting as the decoration, design, and color of the webpage's "interior."
