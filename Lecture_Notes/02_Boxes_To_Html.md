# Boxes to HTML

When creating a web page, start with big boxes and populate those big boxes with your smaller elements that are smaller boxes

All boxes should be defined using 'div' tags which are easy to remember because div is short for divider

Give your 'div' tags classes so you can style them in CSS using: .className { Attribute: Value;}

Like this:

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" text="text/css" href="style.css">
    </head>
    <body>
        <div id="main">
            <p> Placeholder content </p>
            <img src="">
        </div>
        <div class="undermain">
            <p> More placeholder content </p>
        </div>
    </body>
</html>
```

Then your style.css file could read:

```css
#main
{
    color: blue
}

.undermain
{
    color: gold
}
```

Notice we used a class selector and an id selector in our HTML and CSS. Typically ids are for elements that you only plan on having one of - like the main div you will only need one of. Classes are typically applied over and over to many different elements. Like on twitter, each tweet probably has the same class.
