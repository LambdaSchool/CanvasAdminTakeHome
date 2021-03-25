<div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><iframe src="https://lambdaschool-1.wistia.com/medias/sit5qu3vxn" allow="autoplay; fullscreen" allowtransparency="true" frameborder="0" scrolling="no" class="wistia_embed" name="wistia_embed" allowfullscreen msallowfullscreen width="100%" height="100%"></iframe></div></div><script src="https://fast.wistia.net/assets/external/E-v1.js" async></script>

## Overview

### Introduction to Cascading Stylesheets

Before we begin, let's think about the analogy of a web page as a house. In order to build a house, we need a few things. First, we need raw materials - like wood and bricks. Then, we need paint and decorations, and a plan to put them together. In this analogy, HTML is the raw materials. It has so much potential, but it's just laying in a pile on the ground. We need the plan, the paint, and the decorations to make a home. That is where CSS comes in.

Eventually, we'd want electricity and plumbing to make our home functional. That's JavaScript, which we'll learn about next.

#### What is CSS?

CSS stands for Cascading Style Sheets. It is a different language than HTML but it works with HTML. It allows us to add style and layout to our web pages. Usually, when we think about web pages, we think about nicely put-together, pretty-looking sites, and so far what we have built has been pretty bland, if not ugly. HTML and CSS work together to create the webpages we are used to seeing. Once the browser reads the HTML, it will then read the CSS and give different styling rules to different elements in our HTML based on how we select them.

#### The `style` and `link` Elements

Before we can add CSS to our web page, we need to inform the browser that what it is reading is in fact CSS. We can tell the browser that through HTML elements known as the `style` and `link` elements. These elements will go in between the `head` tags, as it is not necessarily data we need to appear on the screen.

There are two ways of including CSS in our HTML.

- We can write our CSS directly between two `style` tags, this isn't very common, but it would look something like this.

```html
<style>
  <!-- CSS goes here -->
</style>
```

- More often, we will link to an external CSS file using the `link` element. This element will include two attributes: `rel` and `href`. `rel` will refer to the type of file we are linking: in this case, `"stylesheet"`, and the `href` will point to the location of the file on your computer, or more simply, the file name.

```html
<head>
  <link rel="stylesheet" href="./styles.css" />
</head>
```

Note that, in codepen, linking is done "under the hood", so we can code our CSS straight in the CSS pannel like so.

<iframe height="265" style="width: 100%;" scrolling="no" title="PreCourse Style" src="https://codepen.io/lambdaschool/embed/4918a680ea2327cb02fc888270483aa0?height=265&theme-id=default&default-tab=html,result&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lambdaschool/pen/4918a680ea2327cb02fc888270483aa0'>PreCourse Style</a> by Lambda School
  (<a href='https://codepen.io/lambdaschool'>@lambdaschool</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

**Check for Understanding:** Before you move on, edit the CodePen to make our text blue.

#### Introduction to CSS Selectors

You may notice in the pen above that the CSS references a specific tag, in this case, `<h1>`. In order for us to apply styling rules to HTML elements, we have to know which elements to apply the rules to. This is where selectors come in.

You can select all elements of a certain type - `p`, `div`, `h1`, or `body`; or you can select all elements with a certain `class` or `id`. By adding a `class` or `id` attribute to an element, we then make it possible for the CSS to select that element more easily and accurately. Compare the HTML tags to the CSS selectors below and see if you can figure out the rules governing CSS selectors.

<iframe height="352" style="width: 100%;" scrolling="no" title="PreCourse Style w divs" src="https://codepen.io/lambdaschool/embed/061349c6b346983da14bdba6939809a8?height=352&theme-id=default&default-tab=html,result&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lambdaschool/pen/061349c6b346983da14bdba6939809a8'>PreCourse Style w divs</a> by Lambda School
  (<a href='https://codepen.io/lambdaschool'>@lambdaschool</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

#### Anatomy of Styling Rules (Syntax)

In CSS, after the name of the selector, we will use braces (`{}`) to hold property and value styles for that selector.

Styling rules will need to adhere to a certain syntax in our CSS so that the browser knows how to read them properly. Within the braces, we will then have the name of the property, a colon(`:`), and the value of the rule. This will be followed by a semicolon(`;`).

```css
body {
  background: blue;
}
```

```css
div {
  styling_property: value of rule;
}
```

`Id`s: are titles that can only appear on a single element. Think of it as you would your driver's license number. ONLY you have that one number.

`Class`es: on the other hand can apply to multiple elements. Think of it like a classroom. Usually, you aren't the only person in a class, although you might be. The class is big enough for lots of people.

Class selectors will always begin with `.`, and Id selectors will always begin with `#`.

**Check for Understanding:** In the codepen above, change the text color of the **class** to _red_.

#### Styling Rules

Now that we have some HTML elements selected, we can begin to add styling. There are a LOT of different ways you can style an object. You can control how big or small it is, what color it is, where it is placed on the screen, or even if it is visible or not. We will go over some of the most common styling properties and how to use them.

- `background` or `background-color`
  - Background can be set to a variety of rules. Most common would be setting the background to a color or an image. Both are displayed below. If you want to be more explicit, you can use the property `background-color` to only set the color of the background.

```css
h1 {
  background: red;
}
body {
  background: url("http://imageurl.com/image.jpg");
}
```

- `color`

  - Color is used for text only. It will change the color of your text.

- `font-size`
  - We can't use width or height for text, but we can determine the size of the font used. You can use any size unit here that you would use with a font in a word processor (px, em, in, and etc). Px or pixel is the most popular.

**Challenge:** In the codepen above, change the background color of your webpage to _grey_

## Follow Along

When we added the image to lambdaschool.com it created a _massive_ problem (no pun intended). Together let's add some CSS style to get our image to the background, and to change text color and style.

<iframe height="402" style="width: 100%;" scrolling="no" title="M3O1 - CSS " src="https://codepen.io/lambdaschool/embed/52b9e575871e7ebb68d0e7a42dd20422?height=402&theme-id=default&default-tab=html,result&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lambdaschool/pen/52b9e575871e7ebb68d0e7a42dd20422'>M3O1 - CSS </a> by Lambda School
  (<a href='https://codepen.io/lambdaschool'>@lambdaschool</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

Let's start with the simple stuff. Before we do anything else, let's add some font color and style to our semantic elements. Here we are selecting multiple elements with commas and assigning all of the text to the color "black" and the font-family "sans-serif". We're also designating text color, background color, and font size for our button.

CSS is a great place to practice your google-fu. There are hundreds of CSS styling properties and infinitely more descriptors. You're not expected to know all of these properties. Instead, describe your issue to google, test things out, and use your design eye to find what you like the most.

```css
h1,
h2,
p {
  color: black;
  font-family: sans-serif;
}

button {
  color: white;
  background-color: #bb2026;
  font-size: 16px;
}
```

Next, let's add id attributes in HTML and style to them by selecting those ids in CSS. We'll start by creating an 'image-container' and 'text-container' id. We want the 'image-container' to wrap around everything _except_ "Higher learning. Higher earning." and "Lambda is designed for student success...etc," to do that, we'll need to place a `<div id ="image-container">` tag at the beginning of our HTML, and a `</div>` tag after the button. We'll add a second div called `<div id ="text-container">` around the rest.

Finally, we can move our image from the "body" to the div and start getting a more complete website. You'll notice that the image looks cut off - the box model will help us deal with that.

```CSS
#image-container {
  background: url("https://assets-global.website-files.com/5cd091cfb5499f22bdf72905/5d1133da829994859a190d12_website-home4.jpg");
  background-position: center;
}

#text-container {
  text-align: center;
}
```

Our final product should look like this. It is looking a lot closer to lambdaschool.com, but...squished? Next up, we'll learn about the box model which will help take care of the squishing and get us to a more believable lambdaschool replica.

![Screen Shot 2020-01-16 at 4.48.44 PM](https://i.imgur.com/hMywz6G.png)

## Challenge

Go back to your codepen and add style. Include a font, text-color, and background style.
