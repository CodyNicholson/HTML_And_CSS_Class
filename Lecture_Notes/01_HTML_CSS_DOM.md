# HTML CSS DOM

HTML is a structural language for creating webpages, and CSS is a language for styling HTML webpages

Both of these languages have their own unique rules and syntax

### Hyper Text Markup Language (HTML)

An HTML Tag is the basic "word" in the HTML language

*Think of a tag as the main building block of the language*

The browser turns the tags into elements that form a tree

The browser knows how to do this because of the Document Object Model, otherwise known as the *DOM*

### Document Object Modal (DOM)

Document Object Modal is the standard convention for interacting with elements in HTML

The tree you can see for a webpage in dev tools is the DOM tree the browser built from the HTML document it was provided

Each HTML tag creates an element in the DOM that the browser uses to display the page

An element stretches from start tag to end tag and everything between them is content

Content can be empty, text, or another element

Each tag has a name/type: *img, p, div,* etc.

Each tag can have attributes with values like this div tag has a class attribute with the value "main":

```html
<div class="main">place holder content</div>
```

HTML tags and attributes define the structure and content of the page and form a tree what looks like this:

- html tag
    - divider tag
        - paragraph tag
        - image tag
    - button tag
        - link tag

If we use the above model and change it into code it would look like this:

```html
<!DOCTYPE html>
<html>
    <div>
        <p></p>
        <img>
    </div>
    <button>
        <link>
    </button>
</html>
```

See how it forms a tree with the HTML tag as the root, then the div and button tags as branches from the HTML tag, and then the p and img tag branching from the div and the link tag branching from the button tag?

### Cascading Style Sheet (CSS)

CSS stands for Cascading Style Sheet and defines the style of the page, like fonts, colors, positions of elements, etc.

CSS is a language with its own syntax and rules that change how elements look on a page

A CSS file must be included in the HTML files that you want to style

In CSS, when you want to refer to a class - say a class called "main" - you write:

```CSS
.main
{
    cssAttribute: newValue;
}
```

If "main" was an Id and not a class then you would write:

```
#main
{
    cssAttribute: newValue;
}
```

Including a CSS file in your html document in your head tag put:

```HTML
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" text="text/css" href="nameOfCssFile.css">
    </head>
    <body>
        <p> Placeholder content </p>
    </body>
</html>
```

For organizations sake, every web element is box shaped on a web page

Start every HTML file with: 

```html
<!DOCTYPE html>
```

And put all the code for that page between an 'html' tag like this:

```HTML
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" text="text/css" href="style.css">
    </head>
    <body>
        <div class="main">
            <p> Placeholder content </p>
        </div>
    </body>
</html>
```
