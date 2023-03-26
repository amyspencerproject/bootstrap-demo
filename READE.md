#First time using Bootstrap Demo

## Resources
[Bootstrap CSS Framework Course](https://www.youtube.com/watch?v=-qfEOE4vtxE) from freeCodeCamp.org
[Popper JS](https://popper.js.org/)
[Bootsrap v5.0 Documentation](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
[Column breaks and reordering](https://getbootstrap.com/docs/5.0/layout/columns/#column-breaks)
[Gutters](https://getbootstrap.com/docs/5.0/layout/gutters/#how-they-work)



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

3/25 stopped at  on video