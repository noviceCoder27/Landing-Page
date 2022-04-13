# Landing-Page
A test webpage

## HTML

div classes used to create the containers where we use flexbox properties on the children elements(.i.e flex items)

**div** tag-> creates a container in which we can place our elements inside

[![div](https://i.stack.imgur.com/vTEAj.jpg)](https://i.stack.imgur.com/vTEAj.jpg)

**a** tags used to create the links

```sh

<a href = "#"></a>

```

`href = "#" means the link will take us to the top of the current webpage`

**Linking the css file**

```sh

<link rel = "stylesheet" href = "path/style.css">

```

**blockquote** ->  specifies a section that is quoted from another source.

**figcaption** -> defines a caption for the element

The two of these are used together to create the quote in our webpage

```sh 

<blockquote>
    <em>The quote </em>
</blockquote>
<figcaption> &mdash; <strong>Thor,God of Thunder</strong>  </figcaption>               

```
*Note we don't specify any outside source(link) for the quote in our given example*


## CSS

```sh

body {

    min-height: 100vh;
}

```

Otherwise the footer will not be pushed down towards the bottom of the screen instead it will be placed according to the height of the content above it

``` sh 

body {

    flex-direction:column;
}

main-body {

    flex:1
}

```

We assign the flex-direction as column in the body to push the footer down by adding flex:1 meaning flex-grow will be one so the items will grow in order to fill the container

```sh 

    .container {
        display: flex;
        justify-content: center;
        align-items: center;
    }


```

We wan't the content our our page to be in the center so we set the display to flex and justify-content(horizontal) & align-items(vertical) to center

` Note -> Since the flex direction by default is row so the main axis is horizontal & cross axis is vertical`

We also add margin and padding in our items inside the div classes

*To create the boxes*

We use empty div elements and add height width and solid border of color ##3882f 

```sh

.box {
    border-radius: 8px;
    width: 60px;
    height: 70px;
    border: 3px solid #3882f6;
}

```

`The border-radius property will decide the roundness of the element's corner which in our case are the boxes`

The text below it is places in the center using the *text-align:center;* property

We also add color, height & padding to our buttons to make them look better.The button's border radius is set to 8px

**Flexbox** 

```sh 

.parent {
    display: flex;
    justify-content:center;
    align-items:center;
    flex-direction:column;
}

.chilren {
    flex-grow:1;
    flex-shrink:1;
    flex-basis:auto;
}

```

For reference purposes -> 

- [Flexbox Cheatsheet](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)