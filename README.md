# HTML-and-CSS concepts
     Box Model     Inline versus Block Elements. Examples.     Positioning: Relative/Absolute     Common CSS structural classes     Common CSS syling classes     CSS Specificity     CSS Responsive Queries     Flexbox/Grid     Common header meta tags     Any other topic you like.
## Box  Model
- When laying out a document, the browser's rendering engine represents each element as a rectangular box according to the standard CSS basic box model. 
- CSS determines the size, position, and properties (color, background, border size, etc.) of these boxes.

- Every box is composed of four parts (or areas), defined by their respective edges: 
  - the content edge, 
  - padding edge, 
  - border edge, and margin edge.
  ![box model](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model/boxmodel-(3).png)

#### Content area:
- The content area, bounded by the content edge, contains the "real" content of the element, such as text, an image, or a video player. 
- Its dimensions are the content width (or content-box width) and the content height (or content-box height). 
- It often has a background color or background image.

#### Padding area:
- The padding area, bounded by the padding edge, extends the content area to include the element's padding. 
- Its dimensions are the padding-box width and the padding-box height.
  
#### Border area:
- The border area, bounded by the border edge, extends the padding area to include the element's borders. 
- Its dimensions are the border-box width and the border-box height.
  
#### Margin area:
- The margin area, bounded by the margin edge, extends the border area to include an empty area used to separate the element from its neighbors. 
- Its dimensions are the margin-box width and the margin-box height.

## Inline versus Block Elements
#### Inline Elements:
- Inline elements are those which only occupy the space bounded by the tags defining the element, instead of breaking the flow of the content.
#### Examples of Inline Elements:
    <a>: This tag is used for including hyperlinks in the webpage.
    <br>: This tag is used for mentioning line breaks in the webpage where ever needed.
    <script> : This tag is used for including external and internal JavaScript codes.
    <input>: This tag is used for taking input from the users and is mainly used in forms.
    <img>: This tag is used for including different images in the webpage to add beauty to the webpage.
    <span>:  This is an inline container that takes necessary space only.
    <b>:  This tag is used in places where bold text is needed.
    <label>: The tag in HTML is used to provide a usability improvement for mouse users i.e, if a user clicks on the text within the <label> element, it toggles the control.
#### Block Elements:
- block-level element always starts on a new line and takes up the full width available (stretches out to the left and right as far as it can).
  
#### Examples of Block elements:

    <h1>-<h6> : This element is used for including headings of different sizes ranging from 1 to 6.
    <div>: This is a container tag and is used to make separate divisions of content on the web page.
    <hr>: This is an empty tag and is used for separating content by horizontal lines.
    <li>: This tag is used for including list items of an ordered or unordered list.
    <ul>: This tag is used to make an unordered list.
    <ol>: This tag is used to make an ordered list.
    <p>: This tag is used to include paragraphs of content in the webpage.
    <table>: This tag is used for including the tables in the webpage when there is a need for tabular data.
#### HTML 5 Semantic block elements:
    <header>: This tag is used for including all the main things of the webpage like navbar, logos, and heading of the webpage.
    <nav>: This tag helps to navigate through different sections by including different blocks of hyperlinks in the webpage.
    <footer>:  This contains all information about the authorization, contact, and copyright details of the webpage.
    <main>: The main content of the webpage resides in this tag.
    <section> : This is used separate different sections in the webpage.
    <article>: This tag is used to include different independent articles on the webpage.
    <aside>: This tag is used to mention details of the main content aside.

## Positioning: Relative/Absolute:

- The position CSS property sets how an element is positioned in a document. The top, right, bottom, and left properties determine the final location of positioned elements.

#### Absolute:
- The element is removed from the normal document flow, and no space is created for the element in the page layout. 
- It is positioned relative to its closest positioned ancestor, if any;
- otherwise, it is placed relative to the initial containing block. Its final position is determined by the values of top, right, bottom, and left.
- This value creates a new stacking context when the value of z-index is not auto. 
- The margins of absolutely positioned boxes do not collapse with other margins.
 ![Absolute](https://miro.medium.com/max/686/1*XDqGjAEa_sNL1OlPQhEb7A.png)'
#### Relative:
- The element is positioned according to the normal flow of the document, and then offset relative to itself based on the values of top, right, bottom, and left. 
- The offset does not affect the position of any other elements; thus, the space given for the element in the page layout is the same as if position were static.
  ![Relative](https://miro.medium.com/max/910/1*3N2ousp3yth9ovHA8TpDZw.png)

#### common structural classes:
- Structural pseudo classes allow access to the child elements present within the hierarchy of parent elements. 
- We can select first-child element, last-child element, alternate elements present within the hierarchy of parent elements.
#### The following is the list of structural classes.
  1.  :first-child 
  2.  :nth-child(n)
  3.  :last-child
  4.  :nth-last-child(n)
  5.  :only-child
  6.  :first-of-type
  7.  :nth-of-type(n)
  8.   :last-of-type
  9.  :nth-last-of-type(n)

#### common styling classes:

#### CSS Specificity:
- Specificity is the algorithm used by browsers to determine the CSS declaration that is the most relevant to an element, which in turn, determines the property value to apply to the element. 
- The specificity algorithm calculates the weight of a CSS selector to determine which rule from competing CSS declarations gets applied to an element.
  
- The specificity algorithm is basically a three-column value of three categories or weights - ID, CLASS, and TYPE - corresponding to the three types of selectors. 
- The value represents the count of selector components in each weight category and is written as ID - CLASS - TYPE. The three columns are created by counting the number of selector components for each selector weight category in the selectors that match the element.

#### CSS Responsive Queries
- we use media Queries for Responsive Queries.
- The @media rule is used in media queries to apply different styles for different media types/devices.

- Media queries can be used to check many things, such as:

   -  width and height of the viewport
   -  width and height of the device
   -  orientation (is the tablet/phone in landscape or portrait mode?)
   - resolution
- Using media queries are a popular technique for delivering a tailored style sheet (responsive web design) to desktops, laptops, tablets, and mobile phones.
- You can also use media queries to specify that certain styles are only for printed documents or for screen 

#### Flexbox/Grid
- The basic difference between CSS Grid Layout and CSS Flexbox Layout is that flexbox was designed for layout in one dimension - either a row or a column. 
- Grid was designed for two-dimensional layout - rows, and columns at the same time. 
- The two specifications share some common features, however, and if you have already learned how to use flexbox, the similarities should help you get to grips with Grid.
  
### Common header meta tags:
- The `<title>` element is metadata that represents the title of the overall HTML document.
- Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document — the <meta> element.
- Specifying your document's character encoding `<meta charset="utf-8">`
- Adding an author and description(`<meta name="author" content="Chris Mills">`
- `<meta name="description" content="The MDN Web Doc">`)
- Active learning: The description's use in search engines
- Adding custom icons to your site(`<link rel="icon" href="favicon.ico" type="image/x-icon">
`)
- Applying CSS and JavaScript to HTML(`<link rel="stylesheet" href="my-css-file.css">`
)
- Setting the primary language of the document(`<html lang="en-US">`
)

















## References:
#### Box model:
- [w3.org](https://www.w3.org/TR/2016/WD-CSS22-20160412/box.html#box-dimensions)
- [mdn web docs](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Box_Model/Introduction_to_the_CSS_box_model#bord)

#### Box model:
- [Geek4Geeks](https://www.geeksforgeeks.org/difmference-between-block-elements-and-inline-elements/)
- [mdn web docc](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements#block-level_vs._inline)

#### position Absolute/Relative:
- [mdn](https://developer.mozilla.org/en-US/docs/Web/CSS/position)
- [css tricks](https://css-tricks.com/absolute-relative-fixed-positioining-how-do-they-differ/)
- [medium article](https://leannezhang.medium.com/difference-between-css-position-absolute-versus-relative-35f064384c6)
#### common structural classes:
- [web4college](https://www.web4college.com/css/web4-css-structural-classes.php)
- [mdn](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)
 
#### Flexbox/Grid
- [flexbox/grid](https://blog.bitsrc.io/css-flexbox-vs-grid-layout-5ae41e28d1d2)
#### CSS Responsive Queries:
- [Responsive Queries](https://www.w3schools.com/cssref/css3_pr_mediaquery.asp)
### Common header meta tags:
- [head meta tags](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)