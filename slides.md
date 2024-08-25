---
theme: light-icons
image: ./images/intro.jpg
title: Web development - Introduction | Part 1
transition: slide-left
mdc: true
layout: intro
download: true
favicon: "https://scratchmy.dev/favicon.ico"
---

<div class="mb-4 absolute top-20 left-12">
  <span class="text-6xl text-teal-400 font-500" >
    Web development<light-icon icon="code"/>
  </span>
  <div class="text-4xl text-white text-opacity-60 font-300 uppercase" >
    Introduction – Part 1
  </div>
</div>

<div class="mb-4 absolute bottom-4 right-12">
  <div class="flex gap-x-4 items-center">
    <div class="rounded-full p-0.5 shadow-lg shadow-zinc-800/5 ring-1 backdrop-blur bg-white ring-white/10">
      <img src="/images/profile.webp" sizes="4rem" class="rounded-full object-cover h-16 w-16" alt="Profile picture" width="400" height="400" loading="lazy" decoding="async">
    </div>
    <div class="flex flex-col">
      <p class="!my-1 text-xl">Sébastien VIALLEMONTEIL</p>
      <p class="!my-1">Full stack web developer</p>
      <a href="mailto:sebastien.viallemonteil@institut-agro.fr"><light-icon icon="mail" class="inline-block mb-0.5"/> sebastien.viallemonteil@institut-agro.fr</a>
    </div>
  </div>
</div>


---
layout: image-right
image: ./images/gifs/sad.webp
equal: true
---

# First, a bit of history

It’ll be quick, I promise.

---
layout: dynamic-image
image: ./images/pray.jpg
equal: false
left: false
---

<v-clicks>

- **Tim Berners-Lee** created the ~~_universe_~~ web in 1991
- **HTML** was born at the same time (what a coincidence!)
- Its sibling, the infamous **CSS** was born in 1996

</v-clicks>

<img v-click class="absolute top-[50%] -mt-32 right-30 border-2 border-gray-300 dark:border-white/80 rounded-md" src="/images/gifs/84years.webp" alt="It’s been 84 freacking years!" />

---
layout: center-image
image: ./images/html-everywhere.jpg
---

---
layout: center
---

# What is HTML?

<v-clicks>

- First, it stands for 🥁🥁🥁 **HyperText Markup Language**
- It allows the worthy to create **static** web pages
- Structuring language
- Made of **tags** interpreted by web browsers

</v-clicks>

---
layout: dynamic-image
image: ./images/html-versions.jpg
equal: false
left: false
---

# HTML versions

<v-clicks>

- HTML 1: created in 1991 (obviously), first HTML files but there is no standard to follow yet
- HTML 2: 1995, the W3C (more on that later) gives standards
- HTML 3: 1997, first tables, scripts and basic positioning
- HTML 4: end of 1997, better tables, forms, frames, style sheets inclusion, etc.
- HTML 5: officially released in 2014 but was available since 2008 a draft

</v-clicks>

<div v-click class="text-center mt-4">
  Latest version: 5.2 since 2017
</div>

---
layout: dynamic-image
image: ./images/rules.jpg
equal: false
left: true
---

# W3C

<v-clicks>

- Well it’s the **World Wide Web Consortium** created by *master* Tim Berners-Lee of course
- It gives standards that web browsers should follow
- Tool to test and validate web pages

</v-clicks>

---
layout: center-image
---

<h1 class="text-4xl mb-4 text-teal-400">Time to code…</h1>

![Excited gif](/images/gifs/excited.webp)


---
layout: center-image
---

<h1 class="text-4xl mb-4 text-teal-400">Well, almost…</h1>

![Pedro laugh and cry gif](/images/gifs/pedro.webp)

---
layout: center
---

# HTML tags

<v-clicks>

- Keywords
- Two categories of tags
- Composed of attributes

</v-clicks>

---
layout: center-image
---

<div class="text-left grid cols-2 divide-x divide-gray-200 dark:divide-white/70">
  <div class="pr-8 space-y-4">
  <h2 class="text-3xl text-teal-400">Container tags</h2>
  <div v-click>

```html {*}{lines:true}
<tag>...</tag>
```

  </div>
  <h2 v-click class="text-3xl text-teal-400">Nested tags</h2>
  <div v-click>

```html {*}{lines: true}
<tag1>
  <tag2>...</tag2>
</tag1>
```

  </div>
  </div>
  <div class="pl-8 space-y-4">
  <h2 v-click class="text-3xl text-teal-400">Self-closing tags</h2>
  <div v-click>

```html {*}{lines: true}
<tag>
```

  </div>
  <div v-after class="h-px bg-gray-200 dark:bg-white/70 mb-4"></div>
  <div v-after>

```html {*}{lines: true}
<tag />
```

  </div>
  <div v-after class="text-gray text-center">Both syntaxes are valid</div>
  </div>
</div>

---
layout: center-image
---

# Attributes

```html {*}{lines:true}
<tag attribute1="value" attribute2="value">...</tag>
```

Attributes are usually shaped this way: <strong v-mark.circle.red="1">key</strong>=<strong v-mark.circle.blue>value</strong>

<span v-mark.circle.red="1" class="absolute text-transparent mt-0.5 -ml-0.5 top-[44.5%] left-[38%] text-[12px] font-[var(--prism-font-family)]">attribute1</span>
<span v-mark.circle.red="1" class="absolute text-transparent mt-0.5 -ml-1 top-[44.5%] left-[51%] text-[12px] font-[var(--prism-font-family)]">attribute2</span>
<span v-mark.circle.blue="1" class="absolute text-transparent mt-0.5 top-[44.5%] left-[46%] text-[12px] font-[var(--prism-font-family)]">value</span>
<span v-mark.circle.blue="1" class="absolute text-transparent mt-0.5 -ml-0.5 top-[44.5%] left-[59%] text-[12px] font-[var(--prism-font-family)]">value</span>

<ComplementaryMessage>Sometimes attributes don’t have any value</ComplementaryMessage>


---
layout: center-image
---

<h1 class="text-4xl mb-4 text-teal-400">First web page</h1>

![At last gif](/images/gifs/at-last.webp)

---
layout: center-image
---

<h1 class="text-4xl mb-4 text-teal-400">The bare minimum</h1>

<div class="text-left">

```html {all|1|2,14|3-9|10-13}{lines:true}
<!DOCTYPE html> <!-- HTML5 Doctype -->
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <!-- Other meta tags (description, keywords, viewport,...) | optional -->
    <title>Document</title>
    <!-- Tags to load CSS and Javascript files | optional -->
    <!-- favicon | optional -->
  </head>
  <body>
    <!-- Page content (blocs, paragraphs, images, links) -->
    <!-- Tags to load Javascript files | optional -->
  </body>
</html>
```

</div>

---
layout: image-right
image: ./images/gifs/score.webp
equal: false
---

# Using real tags to add content

Brace yourselves kids

---
layout: dynamic-image
image: ./images/html-code.jpg
left: false
equal: false
---

# Text blocks (1/2)

### Paragraphs

````md magic-move {lines: true}
```html {*}
<p>
  First paragraph.
  Notice this sentence is on the same line despite the line break.
</p>
<p>
  Second paragraph
</p>
```

```html {*}
<p>
  First paragraph.<br>
  Notice this sentence is on a new line but in the same paragraph.
</p>
<p>
  Second paragraph
</p>
```
````

<arrow class="delay-1000" v-click="1" x1="360" y1="75" x2="230" y2="155" color="#7f1d1d" width="2" />

<div v-motion v-click.hide="1" :initial="{x:0}" :leave="{x:-999, transition: { delay: 1000 }}" class="mt-4 p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <p>
    First paragraph.
    Notice this sentence is on the same line despite the line break.
  </p>
  <p>
    Second paragraph
  </p>
</div>
<div v-motion v-click="1" :initial="{x:-999}" :enter="{x: 0, y: -168, transition: { delay: 1000 }}" class="mt-4 p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <p>
    First paragraph.<br>
    Notice this sentence is on a new line but in the same paragraph.
  </p>
  <p>
    Second paragraph
  </p>
</div>

---
layout: dynamic-image
image: ./images/html-code.jpg
left: false
equal: false
---

# Text blocks (2/2)

### Preformatted text

```html {*}{lines:true}
<pre>
  Some text that will be displayed as is.
  A second line
</pre>
```

<div class="mt-4 p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md relative">
  <pre>
    Some text that will be displayed as is.
    A second line.
  </pre>
  <div v-mark.box.blue="1" class="absolute top-2 bottom-2 left-2 w-10"></div>
  <div v-mark.box.blue="1" class="absolute bottom-2 left-14 right-2 h-8"></div>
</div>

<ComplementaryMessage>Notice spaces and tabulations in the codes also appear on screen</ComplementaryMessage>
<ComplementaryMessage type="alert">Use with caution</ComplementaryMessage>

---
layout: dynamic-image
image: ./images/html-code.jpg
left: false
equal: false
---

<div class="flex items-center gap-2">
  <h1>Hyperlinks</h1>
  <span class="text-teal-400 -mt-2"><light-icon icon="link" size="24px" /></span>
</div>

### Internal

```html {*}{lines:true}
<a href="page1.html" title="First page">
  Go to the first page of this website
</a>
```

<div v-click>

### External

```html {*}{lines:true}
<a href="https://youtube.com" title="Youtube">
  Go to Youtube’s home page
</a>
```

</div>

<div v-click>

### Anchor (specific part of a page)

```html {*}{lines:true}
<a href="#part-3" title="Third part">
  Go to the third part of this page
</a>
```

</div>

---
layout: dynamic-image
image: ./images/html-code.jpg
left: false
equal: false
---

<div class="flex items-center gap-2">
  <h1>Images</h1>
  <hugeicons-image-01 class="text-teal-400 text-xl -mt-1" />
</div>

### From the local website

```html {*}{lines:true}
<img src="wink.webp" title="Wink wink !" 
  alt="A gif of a person winking" />
```

<div v-click>

### Online image

```html {*}{lines:true}
<img src="https://exemple.fr/pics/668989b1q0p0.jpg" title="Surprise !"
alt="You found me !" />
```

</div>

<ComplementaryMessage type="alert" bordered v-click>Online images can be removed from the original website and therefore disappear on your website</ComplementaryMessage>

<img v-click src="/images/gifs/wink.webp" alt="A gif of a person winking" class="absolute border-2 border-gray-300 dark:border-white/80 rounded-md w-3/12 h-auto right-26 top-[50%] -mt-10" />

---
layout: dynamic-image
image: ./images/html-code.jpg
left: false
equal: false
---

# Headings

There are six levels of heading in HTML, **1** being the most important and obviously, **6** the least important.

<div v-click>

```html {*}{lines:true}
<h1>A very important heading</h1>
```

</div>
<div v-click>

```html {*}{lines:true}
<h2>An important heading</h2>
```

</div>

<div v-click>

```html {*}{lines:true}
<h3>A less important heading</h3>
```

</div>

<p v-click class="text-xs text-center">Well, you get the gist.</p>

<ComplementaryMessage type="alert" bordered>Try and respect the heading hierarchy in your web pages like you would in a text document</ComplementaryMessage>

<div v-click class="absolute scale-80 bg-white border-2 border-teal-600 rounded-md p-4 -right-6 top-[25%] space-y-4 text-gray-800">
  <p class="text-4xl">A very important heading</p>
  <p class="text-3xl">An important heading</p>
  <p class="text-2xl">A less important heading</p>
  <p class="text-xl">Well… an even less important heading</p>
  <p class="text-lg">An almost insignificant heading</p>
  <p>Last heading, I promise</p>
</div>

---
layout: intro
image: ./images/quiz.jpg
---

<h1 class="absolute left-12 bottom-12">Quiz time</h1>

<img v-click src="/images/gifs/mouahahah.webp" class="absolute right-12 top-[30%] border-2 border-white rounded-md" alt="Mouahaha Gif" />

---
layout: dynamic-image
image: ./images/question.jpg
equal: false
---

# Riddle me this
It’s really simple 😉

<v-clicks>

- Write a basic HTML page
- Add a very important heading
- Add a paragraph so the heading does not feel lonely
- Finally… add a hyperlink to Google (https://google.com in case you don’t know the URL…)

</v-clicks>

<ComplementaryMessage type="danger" bordered>
  <span>Give ChatGPT and its associates a rest, save it for later</span>
  <img src="/images/troll.png" alt="Troll face" class="h-6 inline-block ml-2"/>
</ComplementaryMessage>

---
layout: dynamic-image
image: ./images/time.jpg
equal: false
left: false
---

# Time’s up!
Who wants to write some code?

<div v-click="1">

```html {*|all|1-7,11,12|8|9|10}{lines:true}
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Document</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>Say hello to my friend</p>
    <a href="https://google.com">and go to Google</a>
  </body>
</html>
```

</div>

---
layout: dynamic-image
image: ./images/containers.jpg
equal: false
left: false
---

# Containers
Useful little tags to group and/or style content

<div v-click>

### Divisions
```html {*}{lines:true}
<div>
  <p>First paragraph in this block.</p>
  <a href="https://example.org">I want to leave</a>
</div>
```

</div>
<div v-click>

### Spans

```html {*}{lines:true}
<p>I have a very <span>particular</span> thing to say.</p>
```

</div>

<ComplementaryMessage bordered>
  <strong><u>div</u></strong> creates a new "block" container like the <strong><u>p</u></strong> tag does. Tags located before and after the <strong><u>div</u></strong> can’t be on the same line.
</ComplementaryMessage>

<ComplementaryMessage bordered>
  <strong><u>span</u></strong> creates a new "inline" container like the <strong><u>a</u></strong> tag does. Tags located before and after the <strong><u>span</u></strong> <em>can</em> be on the same line if they also are "inline" containers.
</ComplementaryMessage>

---
layout: dynamic-image
image: ./images/street-lamps.jpg
equal: false
---

# Important content
Sometimes you need to highlight parts of your content

<div v-click>

### Strong

<div class="flex justify-between items-center gap-x-4">

```html {*}{lines:true}
<p>
  You make a strong
  <strong>case</strong> Sherlock.
</p>
```

<div class="bg-white text-gray-800 text-sm border-2 border-teal-600 rounded-md p-2">
  <p>
    You make a strong <strong>case</strong> Sherlock.
  </p>
</div>
</div>
</div>
<div v-click>

### EM

<div class="flex justify-between items-center gap-x-4">

```html {*}{lines:true}
<p>
  Emphasis on <em>important</em>.
</p>
```

<div class="bg-white text-gray-800 text-sm border-2 border-teal-600 rounded-md p-2">
  <p>
    Emphasis on <em>important</em>.
  </p>
</div>
</div>
</div>
<div v-click>

### Mark

<div class="flex justify-between items-center gap-x-4">

```html {*}{lines:true}
<p>
  Mark my <mark>words</mark>.
</p>
```

<div class="bg-white text-gray-800 text-sm border-2 border-teal-600 rounded-md p-2">
  <p>
    Mark my <mark>words</mark>.
  </p>
</div>
</div>
</div>

<ComplementaryMessage type="alert">The default style for each tag is defined by the browser.</ComplementaryMessage>

---
layout: dynamic-image
image: ./images/structure.jpg
equal: false
left: false
---

# Structuring your content
HTML5 tags to create blocks in a meaningful way

<v-clicks>

- **HEADER**: represents introductory content, usually headings, logos, navigation menu, etc.
- **FOOTER**: well… it’s a footer (duh), self explanatory
- **SECTION**: allows you to divide ~~and conquer~~ your content in sections
- **ARTICLE**: portion of the document which could be repeated (blog post, forum message, a comment, etc.)
- **NAV**: usually contains navigation links
- **ASIDE**: complementary content somewhat related to the main content

</v-clicks>

---
layout: dynamic-image
image: ./images/structure.jpg
equal: false
left: false
---

# Structuring your content
HTML5 tags to create blocks in a meaningful way

<Transform scale="0.95">

```html {*}{lines:true}
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Document</title>
  </head>
  <body>
    <header><!-- That’s the header no? --></header>
    <nav><!-- Some links to navigate --></nav>
    <section>
      <!-- Section with article and asides -->
      <article>...</article>
      <aside><!-- Complementary content right here --></aside>
      <aside><!-- Complementary content right here --></aside>
    </section>
    <section>
      <aside><!-- Complementary content right here --></aside>
    </section>
    <footer><!-- Don’t tell me, I know this one --></footer>
  </body>
</html>
```

</Transform>
<img v-click src="/images/html5-schema.png" alt="HTML5 tags example" class="absolute right-4 top-[22%] w-1/3 h-auto border-2 border-teal-600 rounded-md" />
<ComplementaryMessage type="alert" class="!-mt-2">Without any styling, these will just be a series of blocks.</ComplementaryMessage>

---
layout: dynamic-image
image: ./images/list.jpg
equal: false
---

# Lists
To-do, shopping, cleaning, ~~killing~~, you name it

There are two main types of lists and a particular one.

<v-clicks>

1. Unordered lists
2. Ordered lists (like this one!)
3. Definitions (yep, that’s the particular one)

</v-clicks>

---
layout: dynamic-image
image: ./images/list.jpg
equal: false
---

# Lists (1/3)
To-do, shopping, cleaning, ~~killing~~, you name it

### Unordered lists
```html {*}{lines:true}
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

<div v-click class="mt-4 p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <ul class="!list-disc">
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>
</div>

---
layout: dynamic-image
image: ./images/list.jpg
equal: false
---

# Lists (2/3)
To-do, shopping, cleaning, ~~killing~~, you name it

### Ordered lists
```html {*}{lines:true}
<ol>
  <li>First</li>
  <li>Second</li>
  <li>Third</li>
</ol>
```

<div v-click class="mt-4 p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <ol>
    <li>First</li>
    <li>Second</li>
    <li>Third</li>
  </ol>
</div>

<img v-click src="/images/gru-arrested.jpg" alt="Gru’s plan" class="absolute border-2 border-teal-600 rounded-md w-1/3 left-6 top-[42%]" />

---
layout: dynamic-image
image: ./images/list.jpg
equal: false
---

# Lists (3/3)
To-do, shopping, cleaning, ~~killing~~, you name it

### Definitions
```html {*}{lines:true}
<dl>
  <dt>1st term</dt>
  <dd>1st definition</dd>
  <dt>2nd term</dt>
  <dd>2nd definition</dd>
  <dt>3rd term</dt>
  <dd>3rd definition</dd>
</dl>
```

<div v-click class="mt-4 p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <dl>
    <dt>1st term</dt>
    <dd class="ml-10">1st definition</dd>
    <dt>2nd term</dt>
    <dd class="ml-10">2nd definition</dd>
    <dt>3rd term</dt>
    <dd class="ml-10">3rd definition</dd>
  </dl>
</div>

---
layout: dynamic-image
image: ./images/tables.jpg
left: false
equal: false
---

# Tables (1/2)
With HTML you can either build very simple data tables to complex (i.e. unreadable) master pieces.
### Basic example
```html {*}{lines:true}
<table>
  <caption>Title for the table</caption>
  <tr>
    <th>Title 1</th>
    <th>Title 2</th>
  </tr>
  <tr>
    <td>Val 1 for line 1</td>
    <td>Val 2 for line 1</td>
  </tr>
  <tr>
    <td>Val 1 for line 2</td>
    <td>Val 2 for line 2</td>
  </tr>
</table>
```

<div v-click class="absolute right-20 top-[40%] p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <table class="!border">
    <caption>Title for the table</caption>
    <tr>
      <th class="!border !font-semibold">Title 1</th>
      <th class="!border !font-semibold">Title 2</th>
    </tr>
    <tr>
      <td class="!border">Val 1 for line 1</td>
      <td class="!border">Val 2 for line 1</td>
    </tr>
    <tr>
      <td class="!border">Val 1 for line 2</td>
      <td class="!border">Val 2 for line 2</td>
    </tr>
  </table>
</div>

---
layout: dynamic-image
image: ./images/tables.jpg
left: false
equal: false
---

# Tables (1/2)

<h3 class="-mt-4">Advanced example</h3>

<Transform scale="0.8">

```html {*}{lines:true}
<table>
  <!-- Title for the table -->
  <caption>Title for the table</caption>
  <!-- Table heading -->
  <thead>
    <tr>
      <th>Title 1</th>
      <th>Title 2</th>
    </tr>
  </thead>
  <!-- Table body -->
  <tbody>
    <tr>
      <td>Val 1 for line 1</td>
      <td>Val 2 for line 1</td>
    </tr>
    <tr>
      <td>Val 1 for line 2</td>
      <td>Val 2 for line 2</td>
    </tr>
  </tbody>
  <!-- Table footer -->
  <tfoot>
    <tr>
      <th>Title 1</th>
      <th>Title 2</th>
    </tr>
  </tfoot>
</table>
```

</Transform>
<div v-click class="absolute right-20 top-[35%] p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <table class="!border">
    <!-- Title for the table -->
    <caption>Title for the table</caption>
    <!-- Table heading -->
    <thead>
      <tr>
        <th class="!border !font-semibold">Title 1</th>
        <th class="!border !font-semibold">Title 2</th>
      </tr>
    </thead>
    <!-- Table body -->
    <tbody>
      <tr>
        <td class="!border">Val 1 for line 1</td>
        <td class="!border">Val 2 for line 1</td>
      </tr>
      <tr>
        <td class="!border">Val 1 for line 2</td>
        <td class="!border">Val 2 for line 2</td>
      </tr>
    </tbody>
    <!-- Table footer -->
    <tfoot>
      <tr>
        <th class="!border !font-semibold">Title 1</th>
        <th class="!border !font-semibold">Title 2</th>
      </tr>
    </tfoot>
  </table>
</div>

---
layout: dynamic-image
image: ./images/tables.jpg
left: false
equal: false
---

# Tables (2/2)
With HTML you can either build very simple data tables to complex (i.e. unreadable) master pieces.

### Merging

<img
  :class="['absolute transition-transform duration-600 h-50 rounded-md border-2 border-teal-600', { 'translate-x-200 -translate-y-200': $clicks >= 1 }]"
  src="/images/gifs/merging.webp"
  alt="Merging gif"
/>

<p v-click>Data tables can possess merged cells. There are two types of merging:</p>
<v-clicks>

- Column merging via the attribute `colspan`
- Row merging via the attribute `rowspan`

</v-clicks>

---
layout: dynamic-image
image: ./images/tables.jpg
left: false
equal: false
---

# Tables (2/2)
With HTML you can either build very simple data tables to complex (i.e. unreadable) master pieces.

### Colspan

````md magic-move {lines: true}
```html {*|all}
<table>
  <tr>
    <th>Title 1</th>
    <th>Tilte 2</th>
    <th>Tilte 3</th>
  </tr>
  <tr>
    <td>Val 1</td>
    <td>Val 2</td>
    <td>Val 3</td>
  </tr>
  <tr>
    <td>Val 1</td>
    <td>Val 2</td>
    <td>Val 3</td>
  </tr>
</table>
```
```html {*}
<table>
  <tr>
    <th>Title 1</th>
    <th>Tilte 2</th>
    <th>Tilte 3</th>
  </tr>
  <tr>
    <td>Val 1</td>
    <td>Val 2</td>
    <td>Val 3</td>
  </tr>
  <tr>
    <td>Val 1</td>
    <td colspan="2">Val 2 & Val 3</td>
  </tr>
</table>
```
````

<div v-click.hide="2" class="absolute right-30 top-[40%] p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <table class="!border">
    <tr>
      <th class="!border !font-semibold">Title 1</th>
      <th class="!border !font-semibold">Title 2</th>
      <th class="!border !font-semibold">Title 3</th>
    </tr>
    <tr>
      <td class="!border">Val 1</td>
      <td class="!border">Val 2</td>
      <td class="!border">Val 3</td>
    </tr>
    <tr>
      <td class="!border">Val 1</td>
      <td class="!border">Val 2</td>
      <td class="!border">Val 3</td>
    </tr>
  </table>
</div>

<div class="absolute h-9 w-24 bottom-22 left-29" v-mark.box.blue="[1,2]"></div>
<div class="absolute h-10 w-30 right-36 bottom-42" v-mark.box.blue="[1,2]"></div>

<div v-click="2" class="absolute right-30 top-[40%] p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <table class="!border">
    <tr>
      <th class="!border !font-semibold">Title 1</th>
      <th class="!border !font-semibold">Title 2</th>
      <th class="!border !font-semibold">Title 3</th>
    </tr>
    <tr>
      <td class="!border">Val 1</td>
      <td class="!border">Val 2</td>
      <td class="!border">Val 3</td>
    </tr>
    <tr>
      <td class="!border">Val 1</td>
      <td class="!border" colspan="2">Val 2 & Val 3</td>
    </tr>
  </table>
</div>

<div class="absolute h-4 w-56 bottom-25 left-29" v-mark.box.blue="3"></div>
<div class="absolute h-10 w-30 right-36 bottom-41" v-mark.box.blue="3"></div>

<img v-motion v-click="4" :initial="{x: 999, y: -999}" :enter="{x: 280, y: -350}" class="absolute rounded-md border-2 border-teal-600" src="/images/gifs/magic.webp" alt="Magic GIF" />

---
layout: dynamic-image
image: ./images/tables.jpg
left: false
equal: false
---

# Tables (2/2)
With HTML you can either build very simple data tables to complex (i.e. unreadable) master pieces.

### Rowspan

````md magic-move {lines: true}
```html {*|all}
<table>
  <tr>
    <th>Title 1</th>
    <td>Val 1</td>
    <td>Val 2</td>
  </tr>
  <tr>
    <th>Title 2</th>
    <td>Val 1</td>
    <td>Val 2</td>
  </tr>
  <tr>
    <th>Title 3</th>
    <td>Val 1</td>
    <td>Val 2</td>
  </tr>
</table>
```
```html {*}
<table>
  <tr>
    <th>Title 1</th>
    <td>Val 1</td>
    <td>Val 2</td>
  </tr>
  <tr>
    <th>Title 2</th>
    <td>Val 1</td>
    <td rowspan="2">Val 2 & Val 2</td>
  </tr>
  <tr>
    <th>Title 3</th>
    <td>Val 1</td>
  </tr>
</table>
```
````

<div v-click.hide="2" class="absolute right-35 top-[40%] p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <table class="!border">
    <tr>
      <th class="!border !font-semibold">Title 1</th>
      <td class="!border">Val 1</td>
      <td class="!border">Val 2</td>
    </tr>
    <tr>
      <th class="!border !font-semibold">Title 2</th>
      <td class="!border">Val 1</td>
      <td class="!border">Val 2</td>
    </tr>
    <tr>
      <th class="!border !font-semibold">Title 3</th>
      <td class="!border">Val 1</td>
      <td class="!border">Val 2</td>
    </tr>
  </table>
</div>

<div class="absolute h-4 w-24 bottom-45 left-29" v-mark.box.blue="[1,2]"></div>
<div class="absolute h-4 w-24 bottom-22 left-29" v-mark.box.blue="[1,2]"></div>
<div class="absolute h-22 w-10 right-41 bottom-42" v-mark.box.blue="[1,2]"></div>

<div v-click="2" class="absolute right-25 top-[40%] p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <table class="!border">
    <tr>
      <th class="!border !font-semibold">Title 1</th>
      <td class="!border">Val 1</td>
      <td class="!border">Val 2</td>
    </tr>
    <tr>
      <th class="!border !font-semibold">Title 2</th>
      <td class="!border">Val 1</td>
      <td rowspan="2">Val 2 & Val 2</td>
    </tr>
    <tr>
      <th class="!border !font-semibold">Title 3</th>
      <td class="!border">Val 1</td>
    </tr>
  </table>
</div>

<div class="absolute h-4 w-56 bottom-43 left-29" v-mark.box.blue="3"></div>
<div class="absolute h-22 w-25 right-31 bottom-42" v-mark.box.blue="3"></div>

<img v-motion v-click="4" :initial="{x: 999, y: -999}" :enter="{x: 180, y: -350}" class="absolute rounded-md border-2 border-teal-600" src="/images/gifs/failed-magic.webp" alt="Failed magic GIF" />

---
layout: intro
image: ./images/quiz.jpg
---

<h1 class="absolute left-12 bottom-12">Quiz time</h1>

<img v-click src="/images/gifs/deja-vu.webp" class="absolute right-12 top-[30%] border-2 border-white rounded-md" alt="Déjà vu Gif" />

---
layout: dynamic-image
image: ./images/question.jpg
equal: false
---

# ~~Riddle~~ Solve this
That’s the last straw of data.

<div v-click class="p-4 bg-gray-700 text-white dark:text-gray-800 dark:bg-white rounded-md">
  <table class="!border text-center">
    <thead>
      <tr>
        <th class="!border !font-semibold !text-center">P1</th>
        <th class="!border !font-semibold !text-center">P2</th>
        <th class="!border !font-semibold !text-center">P3</th>
        <th class="!border !font-semibold !text-center">P4</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td class="!border">Spock</td>
        <td class="!border">Bikini</td>
        <td class="!border" colspan="2">Bow</td>
      </tr>
      <tr>
        <td class="!border">Bazinga</td>
        <td class="!border">Hair buns</td>
        <td class="!border">Green</td>
        <td class="!border">Arena</td>
      </tr>
      <tr>
        <td class="!border">Knock Knock Knock</td>
        <td class="!border">Princess</td>
        <td class="!border">Hood</td>
        <td class="!border">District 12</td>
      </tr>
      <tr>
        <td class="!border" colspan="4">???</td>
      </tr>
    </tbody>
  </table>
</div>

<ComplementaryMessage>Yup, the goal is to do that. Easy right?</ComplementaryMessage>

---
layout: dynamic-image
image: ./images/time.jpg
equal: false
left: false
---

# Time’s up!
Who wants to write some code, second edition?

<Transform v-click="1" scale="0.7">

```html {*|all|14|29}{lines:true}
<table>
  <thead>
    <tr>
      <th>P1</th>
      <th>P2</th>
      <th>P3</th>
      <th>P4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Spock</td>
      <td>Bikini</td>
      <td colspan="2">Bow</td>
    </tr>
    <tr>
      <td>Bazinga</td>
      <td>Hair buns</td>
      <td>Green</td>
      <td>Arena</td>
    </tr>
    <tr>
      <td>Knock Knock Knock</td>
      <td>Princess</td>
      <td>Hood</td>
      <td>District 12</td>
    </tr>
    <tr>
      <td colspan="4">???</td>
    </tr>
  </tbody>
</table>
```

</Transform>

---
layout: intro
image: ./images/thinker.jpg
---

<div class="absolute inset-0 flex justify-center items-center">
  <h1 class="text-6xl !text-white font-500">Questions?</h1>
</div>

<div class="absolute bottom-4 right-4 opacity-50 text-sm italic">
  © Unsplash<br>© Giphy<br>© imgflip
</div>
