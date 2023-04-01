#Bootstrap Demo
This is my first time using Bootstrap. These are my notes and code as I am learing how this system works.

## Resources
[Bootstrap CSS Framework Course](https://www.youtube.com/watch?v=-qfEOE4vtxE) from freeCodeCamp.org

[Popper JS](https://popper.js.org/)

[Bootsrap v5.0 Documentation](https://getbootstrap.com/docs/5.0/getting-started/introduction/)

[Column breaks and reordering](https://getbootstrap.com/docs/5.0/layout/columns/#column-breaks)

[Gutters](https://getbootstrap.com/docs/5.0/layout/gutters/#how-they-work)

[Buttons](https://getbootstrap.com/docs/5.0/components/buttons/)

[Cards](https://getbootstrap.com/docs/5.0/components/card/)

[Typography and Lists](https://getbootstrap.com/docs/5.0/content/typography/)

[Utilities](https://getbootstrap.com/docs/5.0/utilities/api/) - holds nearly everthing needed to style and position elements

[Utilities API](https://getbootstrap.com/docs/5.0/utilities/api/#using-the-api) - how to customize Bootstrap





## Notes

- Went with a CDN istallation. Not making a complex website with a lot of backend so going with the least amount of downloading, ie using NPM or doing a complete local download. This means I will have to be connected to the internet to work on this site. Also counting on  most browsers having bootstrap/popper already cached so the load performance of this site shouldn't be a huge problem. I do want to think about loading time because I am learning bootstrap for my portfolio site.

- You have to use Popper with Bootstrap. If you link(CDN install) to the bundled version of Bootstrap then Popper is included. You can opt for having that bundle speparated as well. If you do an NPM install you also have to included a separate Popper install.

- Must have three elements to use grid system. 
    ```
    <div class="container"> 
        <div class="row"> 
            <div class="col">
    ```
- There are min-width break points for all the classes

| Breakpoint | Class infix | Dimensions |
| --- | --- | --- |
| X-Small | None | <576px |
| Small | sm | ≥576px |
| Medium | md | ≥768px |
| Large | lg | ≥992px |
| Extra large | xl | ≥1200px |
| Extra extra large | xxl | ≥1400px |

- Three different types of contianers
    - .container, which sets a max-width at each responsive breakpoint
    - .container-fluid, which is width: 100% at all breakpoints
    - .container-{breakpoint}, which is width: 100% until the specified breakpoint 

- vertical align ```align-items-center``` or ``` align-self-center ```
- horizontal align ```justify-content-between ```
- for breaking a columns to a new line must use ```class="w-100"```
- gutters are a way of getting some padding on the rows but without changing the inward size of the row. There is padding and then a negative margin applied which is confusing. Gutter start at 1.5 rem by default or 24px.
- Buttons have many pre-defined classes. Not sure how good some of the options are for accessibility.
- Cards have three ways to be contained to a specific width: use grid system with row and columns e.g.row/col-4, use card class and specific width e.g. card w-50% or set max-width with css styles e.g. style="max-width: 18rem"
- Horizontal cards can be made by removing the grid gutters with .g-0 and using .col-md-* classes
- Typography in Bootstrap is automatically responsive. If you want to have the same style as heading without using the html div then you can just call it as a class e.g. don't want```<h1>``` then use it as a class, e.g. ```<p class="h1"> ```
- There is also a display class that makes for larger font stylings that are opiniinated
- Use -start and -end to align text. As opposed to -left and -right.
- Inline semantic html tags available such as ``` <mark>, <small>, <s>, <del> ```. These stylings can also be applied as classe without the extra importance being given to them.
- block quote options are really nice looking and include citations and block-footers, etc.
- two types of list styles, ul and li but also inline 
- There are lots of nice features to handle images. To keep an image contained inside of a div us the class="img-fluid" 
- shorthand for spacing (margin, padding, gutter) is {property}{sides}-{size} or {property}{sides}-{breakpoint}-{size} e.g mt-5 is margin top size 5. Size is based off of $spacer that is a default setting. Size 5 is actually $spacer * 3 adn Size 1 is $spacer * .25. You can add more sizes by adding entries to the $spacers Sass map variable.
- Using auto on spacers is helpful. Using mx-auto on a div with paragraphs will center the div.
- There are several border classes, e.g. class="border border-1 border-dark" but just class="border" also give a border
- To use flex just add d-flex class
- Adding shadows around elements is easy e.g. shadow-lg
- Everthing is customizable so if you have a set style you can change defaults on the classes. You can do this with the Utilites API. The theme colors you want are then put into a Sass map and looped over them to generate the utilities, component modifiers, and more. So text-light would be what ever you wanted light to be.




