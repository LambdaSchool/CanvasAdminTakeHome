<div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><iframe src="https://lambdaschool-1.wistia.com/medias/8g7o0s0t6k" allow="autoplay; fullscreen" allowtransparency="true" frameborder="0" scrolling="no" class="wistia_embed" name="wistia_embed" allowfullscreen msallowfullscreen width="100%" height="100%"></iframe></div></div><script src="https://fast.wistia.net/assets/external/E-v1.js" async></script>


## Overview

### Expanded 'Basic' elements

There are dozens of elements available in HTML. However, just a handful are used regularly. We will only cover the most commonly used in this lesson. You can achieve virtually anything you want with these basic HTML elements and some CSS (which we will talk about later). It is important to note that your HTML elements should match the exact information you are attempting to display. This is known as being 'semantically correct'. This is done for a number of reasons including accessibility and SEO and is considered industry standard.

#### Attributes

Before we jump into learning about a couple more HTML elements, let's learn about another way to supply data to an element. When we need to include information that we don't want to render on the page (like the link to an image) we use special flags inside of our tags called attributes. We will see attributes in action in the next section for hyperlinks and images.

To this point we've learned the terms element, tag, and attribute. While those can get confusing quickly, the distinctions are visually clear.

![Screen-Shot-2014-08-12-at-2.08.43-AM](https://i.imgur.com/Ro4Ia1r.png)

#### More Elements

* `<a>`
  * The 'a' ("anchor") element, allows us to create links to other web pages (or even to other areas within our own web page). You will always see the 'a' element used with the `href` attribute to tell the browser what address you want the link to point to.

```html
  <a href="http://www.lambdaschool.com">Here is a link!</a>
```

* `<img>`
  * This element will display an image on the screen. It will always have an 'src' attribute which points to the address of the image to be displayed. NOTE: img tags can be self-closing, as in they do not need two tags. Simply put the `/` before the closing bracket in the first tag:

```html
  <img src="https://picsum.photos/500/300" />
```
* `<ul>` and `<ol>`
  * This element represents an "unordered list". This is the parent element and will contain list items. There is also an ordered, or numbered, list `<ol>`, each has their own purpose. Generally speaking, `<ul>` would be used for a grocery list and `<ol>` for a recipe where direction need to be followed in a specific order. In addition, some developers like to style their lists in CSS and opt not to use these tags.
* `<li>`
  * This stands for `list item` and is the companion to `<ul>` and `<ol>`. These elements represent the items to appear in the list. Any other elements can appear in an `li`.

<iframe height="265" style="width: 100%;" scrolling="no" title="PreCourse tags" src="https://codepen.io/lambdaschool/embed/39f0bcce5f5149bc0524a13bb1767bf3?height=265&theme-id=default&default-tab=html,result&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lambdaschool/pen/39f0bcce5f5149bc0524a13bb1767bf3'>PreCourse tags</a> by Lambda School
  (<a href='https://codepen.io/lambdaschool'>@lambdaschool</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

**Challenge:** Before moving on, add a fourth item to the list that links to Wikipedia's [List of List Article.](https://en.wikipedia.org/wiki/List_of_lists_of_lists) (hint: you'll need to use both a tag and an attribute!)

#### Nesting Elements and Indentation

We've seen in previous examples that we can nest, or level, elements inside of tags. In fact, this is a major part of writing HTML. Nested elements are referred to as `children` and the top-level elements as `parents`. You will see this type of structure throughout your time writing HTML (and all code for that matter). One thing to note is that while indentation is not a requirement of HTML (nor of CSS and JavaScript), it is still often practiced as a readability issue. We not only write code for ourselves, but also for our teammates and those that come after us. Indentation lets your code be much more easily read and understood. Feel free to test this out by editing the code above, you shouldn't see a change in the 'result' page.

## Follow Along

<iframe height="451" style="width: 100%;" scrolling="no" title="M2O2 - Attributes" src="https://codepen.io/lambdaschool/embed/5d24a9de4455e40d4a5dc5c628812326?height=451&theme-id=default&default-tab=html,result&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lambdaschool/pen/5d24a9de4455e40d4a5dc5c628812326'>M2O2 - Attributes</a> by Lambda School
  (<a href='https://codepen.io/lambdaschool'>@lambdaschool</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

With our newfound knowledge of attributes we can add in the image, and make our "Apply to Lambda" button functional.

First, let's add the image with an `<img>` tag. The Lambda School homepage image lives at the following URL: `https://assets-global.website-files.com/5cd091cfb5499f22bdf72905/5d1133da829994859a190d12_website-home4.jpg`. We'll use the `src` attribute to add this to our page. Note that `img` elements don't need a closing tag. Also, notice that this URL is **not** "lambdaschool.com," even though that's where we see the picture. Instead, the URL points to the location where the image is hosted on the cloud. Following this link will lead to *just* our background photo.

```html
<img src = "https://assets-global.website-files.com/5cd091cfb5499f22bdf72905/5d1133da829994859a190d12_website-home4.jpg">
```

We can also use attributes to make our "Apply to Lambda." button functional. To do so, we'll need to use the attribute `href`, and point it to Lambda School's application page: `https://apply.lambdaschool.com/apply/`. If we were building the whole website from scratch, we'd reference another html file the our folder.

```html
<button onclick = "location.href='https://apply.lambdaschool.com/apply/';"> Apply to Lambda.</button>
```

Right now, the image is huge and that's okay. In the next lesson, we'll learn about CSS and start to style things how we want them to look.

## Challenge

Go back to your CodePen and add some images of things you like, or links to your social media profiles, blog, or other websites you enjoy!

Note: to add an image, it will need to live somewhere on the web. You can store images on the cloud and right click, then navigate to `copy image URL` to obtain an image's location.
