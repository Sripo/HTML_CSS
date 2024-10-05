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

### Header & Footer Tags
- `<header></header>` : a container for holding introductory content at the top of our page. This is where you may see a title like an H1
```html
<body>
   <header>
      <h1> Welcome to HTML Documentation </h1>
      <a href = "" >Home </a>
      <a href = "" >About US </a>
      <a href = "" >Contact </a>
  </header>
  <main> </main>
  <footer></footer>
</body>
```
- `<footer></footer>` : a container that holds the concluding content at the bottom of your page.
```html
<body>
   <header>Add some headers </header>
   <main> Add some content that should be visible in the main page </main>
  <footer>
      <hr>
      author : Sri Ponakala <br>
      &copy; copyright reserved <br>
      <small><a href = "mailto:sripo@fake.com> Sripo@fake.com </a></small>
  </footer>
</body>
```

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
- `<input>` : has a variety of attributes that define its behavior and functionality
  - type : Specifies the type of input (e.g., text, email, password, radio, submit, checkbox, tel, button, checkbox, etc.).
  - name : The name of the input, used for form submission. (`<input type="text" name="username" />`) 
  - id: Unique identifier for the input field, useful for associating with a <label>. (`<input type="text" id="username" />`)
  - placeholder: Placeholder text shown inside the input when it's empty. (`<input type="text" placeholder="Enter your name" />`)
  - required: Makes the field mandatory for form submission. (`<input type="text" required />`)
  - pattern : Shows the pattern, how you want your input (`<input type= "tel" id ="phone" placeholder = "123-456-7890" pattern = "[0-9]{3}-[0-9]{3}-[0-9]{4}]">`)
  - disabled: Disables the input field, making it uneditable. (`<input type="text" disabled />`)
  - maxlength: Limits the number of characters allowed in the input. (`<input type="text" maxlength="10" />`)
  - minlength: Specifies the minimum number of characters required. (`<input type="text" minlength="5" />`)
  - value: Specifies the initial value of the input field or the value to submit. (`<input type="submit" value="Submit" />`)
 
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
To create a list of terms and descriptions, similar to a dictionary or glossary. you can add the styles to this list by adding the background-color in DL tag with inline styling.
- Tag: `<dl><dt><dd></dd></dt></dl>`
- **Example**:
    ```html
    <dl>
      <dt>HTML</dt>
      <dd>HyperText Markup Language</dd>
      <dt>CSS</dt>
      <dd>Cascading Style Sheets</dd>
      <dt>JS</dt>
      <dd> JavaScript</dd>
    </dl>
    ```
- **Output**:
    - **HTML**: HyperText Markup Language
    - **CSS**: Cascading Style Sheets

- What to Remember: The `<dt>` tag is for the term, and the `<dd>` tag is for its description. This is useful when you need to define terms or present data in a key-value format.

## Table Tags
- ** Tags & Purpose: ** `<table><tr><th></th></tr>  <tr><td></td></tr> </table>`. <ins> tr </ins> refers to row whereas <ins> th </ins> shows the items inside this tag would be the headings of the table. actual data of the rows will be wrapped inside the <ins> td </ins> tags.
    - atttributes of `<table>` tags are border (ie., `<table border ="1">` value = 0 refers to no border whereas as increase in the number will bolds the border)
    - you can set the alignment of text for row data by `<tr align = "center'>`
 
## Button Tag
- The `<button>` tag is used to create clickable buttons on a webpage. It is versatile and can contain not only text but also images or other HTML content. The `<button>` element can be customized using various attributes.

**Types of Buttons** : The most common type attributes for the <button> tag are:
    | **Button Type**  | **Description**                                                | **Code Example**                                         |
|------------------|----------------------------------------------------------------|----------------------------------------------------------|
| **`<button type="button">`**  | A general-purpose button that can be used to trigger JavaScript actions, but doesn't submit a form. | ```html <button type="button">Click Me</button>```      |
| **`<button type="submit">`**  | A button that submits form data when clicked, used inside a `<form>`. | ```html <button type="submit">Submit Form</button>```   |
| **`<button type="reset">`**  | A button that resets form fields to their default values. | ```html <button type="reset">Reset Form</button>```     |

**Summary of Attribute**
- `type` : Specifies the button type(`button`, `submit`, `reset`)
- `disabled` : Disables the button , making it unclickable.
- `form` : Associates the button with a specific form via the form's `id`.
- `formmethod` : Defines the HTTP method (get, post) to use when submitting (overrides the form’s method).
- `formtarget` : Specifies where to display the response after submitting (e.g., `_blank`, `_self`, etc.).
- `name` : Assigns a name to the button, useful when passing button-specific data during form submission.
- `value` : Specifies the value to be submitted with the button (useful when the button's value matters in form data).

## form Tag
The form tag is used to create an HTML form for user input and submission. It contins form elements like `<input>`, `<text area>`, `<select>` and few other buttons. Below are the  attributes of `<form>` tag. Sometimes you need to change the encryption type of form. 

**Example: ** `<form action = "index.php" method = "POST" enctype = "multipart/form-data">` . Let's say you're sending image &image is a large file, so we will set the encryption type to multipart in simple terms when we send the large amount of data we'll break it into multiple parts then when all of that data is received those will be reassembled `<input type = "file" id = "file" accept = "image/png , image/jpeg">`. This accept attribute takes the values of what type will be accpeted in comma seprated (,) .

- action : Specifies the URL to send the form data to when the form is submitted.
- method : Specifies the HTTP method to be used when sending form data (GET or POST). `<form action="/submit-form" method="post">`
- target : Specifies where to display the response after submitting the form. Can be _blank, _self, _parent, or _top.  `<form target="_blank">`
- autocomplete : Enables or disables autocomplete for the entire form.  `<form autocomplete="off">`
- label : Defines a label for an `<input>` element, improving accessibility by making the form more understandable to screen readers and clickable for users.
    - this label tag is used to hold the text that is visible on the form (`<label for ="username">Username : </label>`) for attribute is for visual inpaired person this for will read the text
- ** `<input>` ** : this input tag is used to take the data into form. It has type, placeholder, min, max but for user to understand what this `<input>` tag will take you need to add the `<label>` tag. This `<label>``<input>` tags goes hand-in-hand. label indicates what this input can hold.
- `<select></select>` : This select tag is used for drop-down menu. Let's say you have to do payment or select the highest Education, then this comes into handy
  ```html
     <select id = "Education">
          <option value = "Secondary"> Secondary</option>
          <option value = "Bachelor's"> Bachelor's</option>
          <option value = "Master's"> Master's</option>
      </select>
   ```
- `<textarea></textarea>` : used to add the comments type of textbox in form. you can set the no.of rows & Columns as well. (`<textarea id = "comment" rows = "3" cols = "25"> </textarea>`)
- 

## **Tricky Questions ** 

- Can you display a web page inside a web page or Is nesting of webpages possible  : Yes, html provide a tag `<iframe>` using which we can achieve this functionality. (` <iframe src = "url of the webpage to embed"/> `)
---

## **CSS (Cascading Style Sheets)** 
CSS adds style to a web page, acting as the decoration, design, and color of the webpage's "interior." There are 3 different ways of applying the CSS.

-Inline : Within the opening tag of one of your elements, you can change the style attribute then list one of many CSS properties.
```html 
       <body style = "background-color : black"> <h1 style= "color : white"> This is my HTML Repo </h1></body>
 ```
-Internal : Adding the style sheet within the head of our HTML document through pair of style tags.
```html
    <head>
      <style>
         body{
            background-color : black;
         }
         h1{
         color: white;
         }
         p{
         color: white;
         }
      </style>
    </head>
  ```
-External : This are probably the most popular method because we can make a stylesheet that's reusable. To create an external stylesheet within our website folder we're going to create a new document (i.e.,s style.css) . We need to link this stylesheet to our HTML file by
```html
<head>
   <link rel = "stylesheet" href = "style.css">
</head>
```
```CSS
Style.css
body{
 background-color : black;
}
h1{
  color: white;
}
p{
  color: white;
}

```
- Identifiers : n identifier (also called an ID selector) allows you to target and style specific HTML elements using the id attribute. The syntax for selecting an ID in CSS is to prefix it with a #, like
```html
<div id="myElement">Hello World</div>
<p id = p1> lorem+ Click tab </p>
```
```CSS 
#myElement {
  color: blue;
  font-size: 18px;
}
#p1{
  color : yellow;
}
```

### Terminology 
The terms `px`,`pt`, and `rem` are units of measurement used in CSS for defining sizes, particularly for fonts, apdding, margins, and other layout dimensions. They don't belong to HTML directly but are used within CSS to style HTML elements.

- **px(Pixels)** : refers to smallest unit of measurement on the screen. It represents an absolute size, meaning 10px will always be 10 pixels regardless of screen size or resolution.

      - <ins> When to use(pro's) </ins> Use `px` when you want precise, fixed control over an element's size. It's good for small details like borders, icons, or when you want an exactly layout.
      - <ins> Con's </ins> since pixels are fixed, they don't scale well across different screen sizes or accessibility needs.

- **pt(Points)**: which comes from print design (not user-friendly). There are 72 points per inch. Like `px`, it's an absolute measurement, but it's more commonly used in printed materials (like PDF's).
   - Rarely used in web design. It's more suitable for print, not responsive design.

- **rem(Root Em)**: rem is a relative unit, which is based on the root element's ( `<html>` ) font size. It is scalable, meaning it adapts based on the user’s settings or the browser’s default size (typically 16px by default).

      - <ins> When to use </ins> Use rem for responsive design, as it scales better across different devices and respects user accessibility settings. It's great for layouts and text, making your     design flexible and user-friendly.

| Unit | When to Use | Description |
|------|-------------|-------------|
| **px** | When you need absolute control over the size of elements | Good for small or decorative elements that don’t need to scale. Doesn’t respond to user settings or device screen size. |
| **rem** | When you want your design to be flexible, scalable, and responsive | Ideal for modern web design, respects user accessibility settings, and scales well across devices. |
| **pt** | Only in rare cases, primarily for print | Used mostly for print-related designs. Not recommended for web design as it doesn’t adapt well to screen environments. |
