# HTML_CSS
Trying to add my Learnings of HTML,CSS

# **HTML (Hyper Text Markup Language)** : is the basic structure of the website pages just like skeleton

* `<html></html>`, `<head></head>`, `<body></body>` are the most basic tag need to be present in index.html code.
* `<title></title>` is where you will write what ever need to be visble in URL.
* `<!-- -->` is used for comments.
* `<h>` tags are used for Headings and there are from h1 to h6
*  `<p></p>` tags are used for paragraph of text and `<pre></pre>` is used for pre-formatting the text(adding the line breaks or writing the text in required format)
*  `<a></a>` anchor tags are used for hyperlinks (ie.,if you give href='mailto:test@fakegmail.com' it will open the outlook) and it requires attributes
    - ins>**href**</ins> hold the URL links and this url's are of two kinds.
       - Absolute URL : which contains the full web address, starting with protocol (http:// or https://) and points to a specific location on the internet.
       - Relative URL : doesn't have the full web address, only the path re;ative to current pages or website(i.e., other html or css page in project code). It is used for linking within the same site.
    - `<a></a>` has another attribute <ins> target </ins> 'target= _blank' it opens the href URL in new page.
    - `title` attribute shows the additional information when you hover on the href.
* `<audio></audio>` used to add the audio files with `<source>` as self ending tag and contains few attributes
       - `controls` attribute to display the controllers on the page.
       -`autoplay` is used play the audio once page is loaded.
       -`muted` will mute the audio on loading and you have to unmute.
       -`loop` loops the audio.
*  Self- Ending tags are
       -`<br>` for line break.
       -`<hr>` for line a horizontal line across your page.
       -`<img>` to inculde the image and it has attributes like height, width and alt(i.e., to display the text if incase something went wrong with picture or for visual impaired people).

# **CSS (Cascading Style Sheets)** : that adds style to a web page just like Decorations and design and colors of the interior
