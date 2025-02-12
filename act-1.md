---
layout: default
title: 1 - Getting Started
nav_order: 2
parent: Workshop Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---

# Getting Started With HTML

Our HTML page will look basic at first, but if you finish the workshop you will have something that looks like a complete web page, with images, links, and more. 

If you have any questions, or get stuck, please ask the instructor for assistance. The intention of this workshop is for you to create an "about me" page, but it doesn’t have to be about you. For the workshop as a whole, you can use the examples provided, or apply their techniques and principles and create your own work as you like. My example "about me" page will be about "Zuko," a character from a cartoon show. Have fun!

If you haven’t already, **please install [Sublime text editor. (↪)](https://www.sublimetext.com/download) on your computer**. You are welcome to use any text editor you like, but our workshop examples use Sublime. We use this editor because it has some smart features that help to prevent code errors.


## Create a directory and your first HTML file

- First we are going to create a new folder by clicking on **file explorer** for Windows users
- Select your **Desktop** and then right click to select **New** and then toggle to slect **New Folder** 
- If you are using a Mac, right click on your desktop, select **New Folder**
- Name your folder as follows: `html_workshop`.

    <button onclick="toggle('gif1')">Show/Hide Animation</button>
    <div id="gif1">
    <img src="images/act1-1.gif" alt="Demonstration of making a folder."> <br>
    </div> 

- Open Sublime.
- Select **File** in the menu bar and then select **Save as** (within the `html_workshop` folder you just created). Name your file exactly like this: `about.html`. 
- Sublime will know that this new file is an HTML file because you used the `.html` extension, or suffix.
- We now have our first HTML file! Sublime will now be able to provide some HTML features, such as autocompletes, suggestions, and colour themes to make your code easier to read.
- To test Sublime's autocomplete feature, type the letter “**<h**”. Sublime has a dropdown list of suggestions, and selecting one will autocomplete the line for you. Like autocomplete with texting, it is easy to make a mistake, so make sure you are selecting the right one. 

<img width=500px src="images/act-1/act1-1.png" alt="autocomplete example">

## Introducing HTML "tags"

- HTML uses tags to tell the browser how to interpret content (text, images, videos, and so on).
- HTML tags have three elements: 
    - (1) the opening tag, which has a descriptor symbol such as `h1` between two pointy, or angle, brackets: `<` and `>`; 
    - (2) the closing tag, which has the same symbols as the opening tag, with a forward slash _before_ the descriptor (there are some tags that don’t need a closing bracket and these are called "self-closing" tags); 
    - (3) finally, we have the content (everything between the opening bracket and the closing bracket).

## Essential HTML 

- The first thing we need to do is to add the doctype declaration at the top of our `about.html` page.
- To add the declaration, type `<html` and press **tab** to autocomplete or copy and paste the following code

```
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title></title>
</head>
<body>

</body>
</html>
```

<img width=500px src="images/act-1/act1-2.png" alt="about html">
- The HTML `<!DOCTYPE html>` declaration is not an HTML element or tag, exactly, but an instruction that tells your browser what type of document to expect, so that your browser knows how to display, or render, it properly. 
- Here is what your `about.html` page should look like so far: 
    
    <img width=500px src="images/act-1/act1-3.png" alt="tag examples">

- Have you saved your file yet? Now is the time: in Sublime's main menu, click on **File > Save As...** or hit **CTRL (or Command for Mac users) + S** on your keyboard.

<!-- <button onclick="toggle('gif2')">Show/Hide Animation</button> -->
<!-- <div id="gif2">
    <img src="images/act-1/save-tags.gif" alt="save present tags" style="width:720px;">
    </div> -->

### Title tags
    
- Our current _file_ name is `about.html`, but we want to add a different title to our page. On a website, this title will appear as the name of the page's tab. 
- The title tag goes within the `<head>` tag and is therefore part of our page's [metadata (↪)](https://en.wikipedia.org/wiki/Metadata). 
- Place your cursor underneath the _open_ `<head>` tag, then hit tab on your keyobard to create indent, then add the following: `<title></title>`. We will keep the title tag on one line, which makes it more legible than splitting it up.
- Between the (`<title></title>`) tags, type the following: `About Me`. 
- **Save your `about.html` file.**
- We will now look at our `about.html` in a browser. 
- Navigate to your **Desktop** and go into your `html_workshop` folder and click on the `about.html` file. Your `about.html` file will open in whatever browser is the default on your computer. In the following example, I have opened my `<about.html>` file in Chrome: 

    <img src="images/act-1/view-page-title.png" alt="page title test">

Looking good! Let's move on to adding content to our `about.html` page...

### Headings tags
    
<!-- <button onclick="toggle('gif3')">Show/Hide Animation</button>-->
<!-- <div id="gif3">
    <img src="images/act-1/h-and-p.gif" alt="h and p tags" style="width:720px;">
    </div> -->
- Let’s move on to writing code and content between the `<body></body>` tags.
- We are going to start with heading or `<h>` tags.
- There are 6 types of heading tags: `h1`, `h2`, `h3`, `h4`, `h5`, and `h6`. Heading tags range from biggest text size, with `h1`, to the smallest text size, with `h6`.
- Heading tags are written as follows:<br>
`<h1></h1>`
- We are going to add the following heading tags (between the `<body></body>` tags) and content to our page:
`<h2>Hello, Zuko here.</h2>`<br>
`<h3>About Me</h3>`
- Here is an example of what we have, so far: 

<img width=500px src="images/act-1/act1-4.png" alt="adding first content">

- As you did before, **Save** your file and open it in your browser. Be sure to [hard refresh (↪)](https://www.howtogeek.com/672607/how-to-hard-refresh-your-web-browser-to-bypass-your-cache/) your browser if you do not see the changes you expect. 
- Feel free to take some time to try different heading tags to see the differences between them.

### Paragraph tag

- The `p` tag is used for paragraphs. 
- The content you want in a paragraph would go between the open and closed paragraph tags, as in the following example:<br>
    `<p>Your paragraph content would go here.</p>`
- We are going to add a couple of `p` tags and some content within them:<br>
        `<h2>Hello, Zuko here.</h2>`<br>
        `<p>Prince of the Fire Nation</p>`<br>
        `<h3>About Me</h3>`<br>
        `<p>Zuko is the son of the current Fire Lord of the Fire Nation, making him a prince of the fire nation. However, at 13 Zuko was scarred and subsequently banished by his father for disrespecting his authority. Zuko now roams the world searching for the Avatar as his father has deemed it the only way for Zuko to redeem himself.</p>`<br>
- <mark>Note</mark>: the paragraph content about Zuko is longer than anything we have added so far, and it could be that our paragraph text exceeds the width of the Sublime window, depending on how wide you have made it on your computer. If your text is disappearing off to the right of the Sublime window, and you have to scroll right to see it, we can enable "Word Wrap" so that you can always see your text no matter what size you make your Sublime window. 
  - To enable word wrap in Sublime, click on **View > Word Wrap**. 
- Let's add another paragraph beneath the first paragraph:<br>
`<p>Zuko is joined on his journey for redemption by his paternal uncle, Iroh. Iroh is a retired army general, who mentors Zuko by helping him improve his fire bending and keeping him on the right path. His love of tea often gets on Zuko’s nerves.</p>`
- As you did before, **Save** your file and open it in your browser. 
<!-- <button onclick="toggle('gif4')">Show/Hide Animation</button>-->
<!-- <div id="gif4">
    <img src="images/act-1/end-of-6.gif" alt="body paragraph" style="width:720px;">
    </div> -->
- Our page is coming along nicely! Let's add another bit of common website content: a list. 
    
### List tags
    
- You can use HTML markup to create two kinds of lists: ordered lists and unordered lists. 
- Use an ordered list if you want to display content in a particular order. 
- Use an unordered list if the order of the list items does not matter. 
- Ordered lists use an `<ol>` tag and display, in browsers, as numbered lists, meaning that a number will appear beside your list item. Here’s an example of an ordered list:  
> Frodo’s top three traveling essentials, in order of importance: 
> 1. The One Ring
> 2. Sting (the sword, not the musician)
> 3. Samwise Gamgee
- Unordered lists use a `<ul>` tag and display, in browsers, as a bulleted lists. Here’s an example of an unordered list: 
> Frodo’s shopping list for Bree Market: 
> - Pipe weed
> - Craft beer
> - Even more lembas bread?
- Both ordered (`<ol>`) and unordered (`<ul>`) lists contain list items, which are indicated with an `<li>`, or list item, tag. 
- It is considered best markup practice to indent your `<li>` tags within the `<ol>` or `<ul>` tags. 
- In the following examples, I use unordered lists, since the list (`<li>`) items do not need to be in any particular order. Note that the lists in both examples are nested inside paragraph (`<p>`) tags. 
- I have added a list of some of Zuko's attributes on my `about.html` page. I used an unordered list, since these details are not in any particular order.
- Here is an example of what we have, so far:

<img width=500px src="images/act-1/act1-5.png" alt="example page with list">

<!-- <button onclick="toggle('gif5')">Show/Hide Animation</button> -->
    
<!-- <div id="gif5">
    <img src="images/act-1/list-tag.gif" alt="list tags animated" style="width:720px;">
    </div> -->

<!-- <img src="images/act-1/list-tag.jpg" alt="list tags" style="width:720px;"> -->

### Text tags
    
- Applying style (such as font colours and sizes) to your HTML code should be done in CSS files (which we look at soon), but making changes in the HTML file is sometimes appropriate. For example, the `<del></del>` and `<ins></ins>` tags are used to indicate certain types of text. The `<del>` tag puts a line through the text and the `<ins>` tag underlines text.
- HTML tags can be put around any text. These tags don't have to encompass a whole block of text, or even a whole word, as in the following example:
    - This is <strong>important</strong>. This is <strong><ins>very</ins> important.</strong> Thank <ins>you!</ins>
    - We have two words in bold, one word underlined, and one word underlined _and_ in bold. Let’s look at what that would look like in HTML, with tags:<br/>`<p>This is <strong>important</strong>. This is <strong><ins>very</ins>important.</strong> Thank <ins>you!</ins></p>`
- Notice where the spaces and full stops are. With so many tags, it can be easy to forget to add important content in the right places.
- On your `about.html` page, play around with some of the following tags, saving your file as you go(!) and then looking at it in your browser:
  - `<strong>` = important
  - `<i>` = italic
  - `<em>` = emphasized
  - `<mark>` = marked, or <mark>highlighted</mark>
  - `<small>` = smaller
  - `<sub>` = subscript
  - `<sup>` = superscript
- Remember that there is no right or wrong with our growing `about.html` page. 
- We are taking this time to play around. Often, the best learning happens when we break things! 
- Let's move on the next section in our workshop....

<script>  

    function toggle(input) {
        var x = document.getElementById(input);
        if (x.style.display === "none") {
            x.style.display = "block";
        } else {
            x.style.display = "none";
        }
    }
</script>

[NEXT STEP: Adding Images and Links in HTML](https://uviclibraries.github.io/html-css/act-2.html){: .btn .btn-blue }
