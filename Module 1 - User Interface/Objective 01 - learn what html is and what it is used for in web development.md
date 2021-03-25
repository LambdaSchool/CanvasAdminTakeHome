<div class="wistia_responsive_padding" style="padding:56.25% 0 0 0;position:relative;"><div class="wistia_responsive_wrapper" style="height:100%;left:0;position:absolute;top:0;width:100%;"><iframe src="https://lambdaschool-1.wistia.com/medias/mvwtyzgiqk" allow="autoplay; fullscreen" allowtransparency="true" frameborder="0" scrolling="no" class="wistia_embed" name="wistia_embed" allowfullscreen msallowfullscreen width="100%" height="100%"></iframe></div></div><script src="https://fast.wistia.net/assets/external/E-v1.js" async></script>

## Overview

### What is HTML?

HTML is one of the languages we use for web development. HTML is what we call a "markup language" (as opposed to a "programming" language like JavaScript or Python). This means that it is specifically designed to *display data* in a graphical form (rather than *execute tasks*).

HTML was created as a language when the first visual web browsers came into existence in the early 90s. It is read by the browser and then used as a blueprint for displaying information on your screen.

#### What is a markup language?

Every webpage is essentially just plain text. If you type the sentence "Lambda school is awesome" in an HTML file, you can open it in your web browser and even deploy it to the web. Of course, we know that web pages are much more nuanced than that, and that is thanks to HTML elements.

We can think of elements as being boxes of content on our web page. Different types of content will be contained in different boxes depending on their importance. For example, "Lambda school is awesome" might be a `header` element, with a list of reasons why as a `p` (paragraph) element. When you box the text above in a `header` (or `h1`) element, it looks something like this.

```html
<h1> Lambda School is Awesome </h1>
```

We use certain elements for headers, other elements for images, and still other elements for text. We will be focusing on four different display elements today: division elements (divs), headers, paragraphs, and spans.

#### How do we create HTML code?

We will be writing our HTML code in a sandbox environment called CodePen. CodePen is a great learning tool (as well as a great place to tinker with small chunks of code on the job). We write HTML directly in the HTML section of CodePen and the elements that we create will render in real-time on screen. This is much faster than having to save our file and reload it in the browser every time we make a change.

Go ahead and edit the code below to make your webpage display any sentence you'd like.

<iframe height="265" style="width: 100%;" scrolling="no" title="PreCourse" src="https://codepen.io/lambdaschool/embed/f3c5f02c778ef23285f134f2f31369cb?height=265&theme-id=light&default-tab=html,result&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lambdaschool/pen/f3c5f02c778ef23285f134f2f31369cb'>PreCourse</a> by Lambda School
  (<a href='https://codepen.io/lambdaschool'>@lambdaschool</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

*Note:* CodePen allows us to leave out a couple of critical elements: the `html`, `head`, and `body` elements. These are important to understand when we start writing HTML code in our text editors, but for now, we can ignore them, because CodePen handles them automatically.

#### What are tags?

To create an HTML element, we need to use tags. Each element contains the text (like we saw above), the tag (`h1`) and any number of other details that we'll learn about later on.  The tag names are built into the language and must be written exactly as expected in order for our HTML to render correctly. For example, `paragraph` is not a valid tag name in HTML, but `p` is. You can use online documentation to verify which tag names exist and what elements they are used for.

If we wanted to tag the sentence above as an important header (the biggest text by default), we'd use the `<h1>` and `</h1>` beginning and end tags, as shown below. Before you move on, edit the codepen above to include the `<h1>` tags and note how the result changes!  

```html
<h1>Lamba School is Awesome!</h1>
```

Once we decide which tag we want to use, we can create an opening tag using brackets: `<p>`. These tags must be syntactically precise: an opening bracket + a tag name + a closing bracket. A closing tag looks almost exactly the same, except with a backslash before the tag name. So a closing paragraph tag would look like this: `</p>`. Thus, to create a paragraph with text, we need only write an opening tag and a closing tag:

```html
<p>text goes here</p>
```

#### So what are divs, headers, paragraphs, and spans exactly?

We will be focusing today on four types of display elements. Now that we understand how to create these elements, let's explore their use cases. 

* `<p>`
  * The p ("paragraph") element. This element is meant for holding text. By default, it will render text to the screen on a new line.

```html
  <p>Here is a paragraph!</p>
```

* `<div>`
  * The div element is a generic container. It is used primarily for grouping other HTML elements together. It is invisible by default but can be used to position or style a group of elements. Div isn't super useful in plain html, but will become powerful when we start to "stack" HTML with JavaScript and CSS.
  * `<div>` is a block-level element, meaning it will take up its own, full line.

```html
<div>
  <p>This paragraph is about grapefruits.</p>
  <p>This paragraph is also about grapefruits! I guess it's related to the paragraph above.</p>
</div>
```

* `<span>`
  * The span element is a generic text container. It does not create a new line like the p element does. This element is invisible by default but can be used for styling words or phrases within a larger body of text.
  * Unlike `<div>`, `<span>` operates inline and therefore doesn't take up its own line.

```html
<p>This paragraph contains a <span>very important phrase</span> that should be styled in some way.</p>
```

* `<h1>-<h6>`
  * These are heading tags there are intended to be used as a way to present the subject matter of the page. 1 is the most important and 6 is the least important. By default, 1 will be the largest, 2 will be the next largest, and etc.
  * Avoid using heading tags to resize text. Headings use size to indicate their relative importance, but CSS is preferred for general-purpose resizing.
  * You should only use one `<h1>` per page. Using more than one will not result in an error, but using only one is seen as a best practice. It makes logical sense — `<h1>` is the most important heading, and tells you what the purpose of the overall page is. You wouldn't have a book with more than one title, or a movie with more than one name! Having a single top-level title is also arguably better for screen reader users, and SEO.

<iframe height="265" style="width: 100%;" scrolling="no" title="PreCourse tag levels" src="https://codepen.io/lambdaschool/embed/19c92b335519fea1c509f759c4d14696?height=265&theme-id=light&default-tab=html,result&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lambdaschool/pen/19c92b335519fea1c509f759c4d14696'>PreCourse tag levels</a> by Lambda School
  (<a href='https://codepen.io/lambdaschool'>@lambdaschool</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### Semantic HTML5

The W3C uses the word `recommended` to describe the most up to date web standards. The current recommended standard for HTML markup is HTML5. HTML5 comes with more meaningful tags to better describe our code. We use the word `semantic` to describe tags with meaning.

Some examples of semantic tags include:
```html
<h1>
<p>
<section>
<nav>
<header>
<footer>
```

Notice that you can quickly figure out what each tag listed should be described in HTML. The fact that you can read the tag and know more about its meaning instantly is a direct example of why we say it’s semantic HTML.

Compare the semantic tags above with this list of non-semantic tags below:
```html
<div>
<span>
```

At this point, we can see the advantage of semantic markup for web developers. The clarity and meaning should be found right in the tags. There is another large advantage in writing semantically correct code: computer algorithms consuming your code.

Search engines are algorithms looking for meaning. If your code has a lot of divs without meaning, you could lose out on valuable search engine optimization ranking. Knowing that both humans and machines prefer semantic code, we should get some practice writing it and knowing when to use it.

### `<div>` Tags Aren’t Bad

In the example above, we shed a bit of bad light on using divs with classes, but the reality is that often, you need a div to get the job done. When do we use div tags? Whenever we don’t need to describe meaning. Using a div to create space, add structure, or style elements is just fine. The concept of using markup like this is called presentational HTML.

Presentational HTML does not convey meaning. It is used to achieve something the designer or client wanted but perhaps doesn’t contain meaning. An example of this would be:
```html
<section>
  <div>
    <p>Half the content here should go here.</p>
  </div>
  <div>
    <p>The other half here should go here.</p>
  </div>
</section>
```

Notice how we can use the `<section>` tag to wrap the content, but we could split the content into two halves using divs. Semantically we are still using `<section>`, and at the same time, we are using presentational `<div>` tags to split the content in half. We could then use CSS on our divs to split the content without hurting the semantic structure.

#### How can I inspect an existing web page?

When learning HTML, it can be useful to investigate existing web pages. There is a tool built into Chrome and Firefox called the inspector that allows us to do this. Just right-click any element on a webpage and select "inspect" or "inspect element", depending on the browser. Note that we don't recommend using Safari or Edge for web development. This will pop up a sidebar that allows you to explore all the HTML on the web page. It can be overwhelming for a new developer, but it is a good way to get a taste of what goes into building a complex, production web page.

## Follow Along

Let's practice marking up text in the pen below. For the next few lessons, we're going to focus on building a replica of an old version of Lambdaschool.com's home page. Please note that changes you make to inline pens will not 'save', to fork and save your own copy of this pen, click the logo in the right corner to open it in a new tab.

First, let's take a look at Lambda's old homepage: 

![lambda real website](https://i.imgur.com/ZWSo5vE.gif)

<iframe height="265" style="width: 100%;" scrolling="no" title="M2O1 - HTML tags" src="https://codepen.io/lambdaschool/embed/961cd3dbdd87725892b6d6415f547925?height=265&theme-id=light&default-tab=html,result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lambdaschool/pen/961cd3dbdd87725892b6d6415f547925'>M2O1 - HTML tags</a> by Lambda School
  (<a href='https://codepen.io/lambdaschool'>@lambdaschool</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

The first thing we want to do with our plain text is incorporate HTML elements to identify exactly what different components do. Looking at the real lambdaschool.com we can see that some text is large, some is small, and some is encased in a button. Together, lets add the proper tags in the codepen above. To start, we'll add a `<h1>` heading around "Lambda School" in `<h1>` header and `</h1>` closing tags.

```html
<h1> Your new tech career starts here </h1>
```

Next, let's grab the subtitle "Higher learning. Higher earning" and place it in `<h2>` heading and `</h2>` closing tags.

```html
<h2>Your new tech career starts here. </h2>
```

Next up, add "apply to Lambda". We want this to be a button - to create a button, all we have to do is use the semantic `<button>` tags. Right now, this button won't do anything, but we'll add that feature soon. For now, we can be excited that it *looks* like a button.

```html
<button> Apply to Lambda</button>
```

Finally, let's wrap the two "big" chunks of text in `<p>` tags.

```html
<button>Apply to Lambda</button>
```

Our final product should look something like this. Not quite the same as [lambdaschool.com](lambdaschool.com) yet, but we're on our way!

![Screen Shot 2020-01-16 at 4.28.21 PM](https://i.imgur.com/FJ21qOt.png)

## Challenge

Create your own CodePen. Add a `h1` title with  your name, and start to fill out the page with some details about you and why you're interested in web development. Be sure to include at least 3 tags.

[MDM Reference Guide](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference)
