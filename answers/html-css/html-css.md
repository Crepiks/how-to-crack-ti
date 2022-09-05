# HTML and CSS Interview Answers

## What is Critical Rendering Path?

Critical Rendering Path is a collection of steps that make a path between the time browser gets an HTML page and starts building the webpage for users to visualize.

## What is the DOM? How does the DOM work?

DOM stands of Document Object Model. DOM is a tree structural representation of web page elements needed to allow JavaScript interact with web application.

## Explain the difference between layout, painting and compositing?

Layout - browser determines how much space each element requires and where it needs to be placed.
Painting - the process of filling pixels and drawing out elements.
Compositing - browsers draws elemments in a correct order.

## What are the Benefits of Server Side Rendering (SSR) Over Client Side Rendering (CSR)?

SSR allows applications to be SEO friendly. By creating first render of the page and sending it to the client it allows SEO bots to fully analyze content. Furthermore, creation of first render on server-side decreases time to first contentful paint.

## How can I get indexed better by search engines?

There are two types of SEO optimizations: internal and external. Internal optimization includes increasing loading speed, optimizing assets, including target keywords in to the content of web page and following semantic markup rules. External optimization is about making your service trustworthy by making others web sites refer to the target.

## Ways to improve website performance

1. Usage of optimized file extensions (png replaced by svg of jpeg)
2. Usage of GZIP
3. Caching external data sources on client-side
4. Minimizing JavaScript and CSS resources
5. Usage of Web Workers for parallelizing computation
6. Dividing client resources into chunks

## What does async and defer refer in script tag? Describe the difference between `<script>`, `<script async>` and `<script defer>`

`<script async>` and `<script defer>` changes the behavior of script loading to the web page. Both attributes makes script load despite on HTML content loading. `<script async>` loads script completely asynchronously with no dependecy on other scripts. `script defer>` loads script asynchronously but preserves the order of other defered scripts. `<script defer>` executes script only after DOM tree is built.

## What is desktop first and mobile first design approach?

Desktop first is the approach when desktop version of the web application is built first and only then the content is adapt to mobile screens. The mobile first approach is the opposite.

## How to make page responsive?

We can web page responsive using media queries. This is the most common approach. Also, the markup of web page can be changed from JavaScript depending on screen size.

## What are the building blocks of HTML5?

HTML5 is well known for its semantic approach to markup. For building block in HTML5 tags with specific semantic meaning are used.

## What is difference between Select and Datalist?

Select does not allow values different from those in the list. Datalist allows use manualy enter the different value of choose specific from presets.

## What are the semantic tags available in html5?

1. `<section` - content for grouped content
2. `<main>` - the main content
3. `<article>` - independent content
4. `<header` and `<footer>` - for header and footer respectively

## Why you would like to use semantic tag?

Semantic tags allow better search engine optimization by dividing content into meaningful parts. Also, usage of semantic tags improves accessibility of the web page (screen readers).

## What is accessibility? ARIA role means in a web application

Accessibility is the measurement of comfortability of the web page for different types of content consumption. For instance, for consuming the content of web page through screen readers. ARIA is a set of tools allowing better accessibility. In web ARIA refers to several attributes adding meta information for page elements.

## What is the purpose of the `alt` attribute on images?

`alt` attribute's content is shown when image for some reason could not be loaded. Also, the content of `alt` attribute is used by screen readers to describe picture over voice.

## Define semantic markup. What are the semantic meanings for `<section>`, `<article>`, `<aside>`, `<nav>`, `<header>`, `<footer>` and when/how should each be used in structuring html markup?

1. `<section>` is used for grouping related content
2. `<article` is used to define card with indepdented content
3. `<aside>` is used to define unrelated content positioned on the side
4. `<nav>` is used to define block with navigation links
5. `<header>` is used to define persistent top part of the page
6. `<footer>` is used to define persistent bottom part of the page

## When should you use `section`, `div` or `article`?

1. `section` is for wide (usually full-width) grouped content
2. `article` is for independent card
3. `div` is for all cases when no semantic tag is applicable

## What is an iframe and how it works?

`iframe` is a tag which allows to load inside it independent HTML documents.

## Describe the difference between a `cookie`, `sessionStorage` and `localStorage`?

Despite obvious difference in the storage volume, `cookie` can store content for specific period of time. `sessionStorage` stores content as long as session in the browser exists. `localStorage` stores content as long as it is not deleted. Also, `cookie` stores data on the server side and are sent with every request.

## What are the possible ways to apply CSS styles to a web page?

1. By using `style` attribute.
2. By using `<style>` tag.
3. By linking stylesheet through `<link>` tag.
4. By applying styles from JavaScript.

## What does the cascading portion of CSS mean?

Cascading means that the impact of several style rules will be overrided by rules with higher priority.

## New features in CSS3

Gradients, opacity, transitions, keyframes, variables.

## What is CSS preprocessor?

Preprocessor is a language used to define style with specific extensions which is compiled into usual CSS.

## What are media queries?

Media queries are used to defined portion of styles which should be applied on specific screen types and sizes.

## What does box-sizing do?

`box-sizing` changes the way the size of the content is calculated (whether to include borders and paddings or not).

## Explain some pros and cons for CSS animations versus JavaScript animations

CSS animations are simpler and easy to apply. JavaScript animations are more difficult in implementation and requires more perfomance, however, they allow complex animations.

## What is CSS flexbox?

CSS Flexbox is a set of css rules which allows wide range control under the positioning of the element and its children. In comparison to CSS Grid CSS Flexbox controls children elemenets only over one main axis.

## What is the difference between the “nth-child()” and “nth-of-type()” selectors?

`nth-child()` applies rule to element which are located right after each other. `nth-of-type()` applies rules to elements even if there are other elements between them.

## When to use css grid and flexbox?

The difference between CSS Grid and CSS Flex is that CSS Flexbox enables control over only one axis while CSS Grid can manipulate children over two axis. CSS Flexbox is simpler and if your goal is to center element or position children over main axis it is better to use it. In more complex cases CSS Grid is more appropriate.

## What is CSS BEM?

CSS BEM is a naming convention made by Yandex. It restricts how css selectors can be named and allows more predictable way of managing style reusability accross the project.

## How do you specify units in the CSS?

Units are used right after the number literal. Example `10px` or `50vh`.

## What is the difference between RGBa, HEX and HSLa?

Those are different ways to specify color in CSS. RGBa uses declaration of red, green and blue parts of the color in couple with alpha (opacity). HEX is a hexadecimal representation of the color which is similar to RGBa but uses hexadecimal numbers in its structure. HSLa uses combination of hue, saturation and lightness.

## What is the difference between class selectors and id selectors?

They use different attributes to target the element on the page. Futhermore, according to the rule of id attribute usage there should not be elements with the same ids as a result the id selector usually targets only one element.

## What is the difference between Pseudo-classes and pseudo-elements?

Pseudo-classes define different states of the targeted element while pseudo-elements define additional structures which are appended to the targeted element.

## What are the css selectors?

CSS selectors are the expressions aimed to locate elements on the page and apply css rules to them.

## What does CORS stand for and what issue does it address?

CORS is a Cross Origin Resource Sharing. It is a policy of the most web browsers which prevents client side JavaScript to make requests to server which did not explicitly allow to send requests to them.

## Explain the use of rel="nofollow", rel="noreferrer", rel="noopener" attribute?

`nofollow` specifies for Search Engines to prevent page from being endorsed by the current page. `noreferrer` hides refering page information when followed by link. `noopener` prevents new tab from being able to get information of origin tab.
