example from scrimba:

```

.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr; <--! 3 columns, fr for responsivness -->
    grid-template-rows: 50px 50px;
    grid-gap: 3px;
}


```
         ![](https://i.imgur.com/ZGNhB2y.png)

    same thing as:

`.container {`
    `display: grid;`
    `grid-template-columns: repeat(3, 1fr); <--! same thing, first parameter is the no. of collumns, second the value height, weight -->`
    `grid-template-rows: repeat(2, 50px);`
    `grid-gap: 3px;`
`}`


    and same thing as:

`.container {`
    `display: grid;`
    `grid-template: repeat(2, 50px) / repeat(3, 1fr);   <--! shorthand method; starts with rows, ends with collumns -->`
    `grid-gap: 3px;`
`}`



------

`.container {`
    `display: grid;`
    `grid-gap: 3px;`
    `grid-template-columns: repeat(2, 1fr);`
    `grid-template-rows: 40px 200px 40px;`
`}`

`.header {`
    `grid-column-start: 1;`
    `grid-column-end: 3;     <--! 2 columns and 3 column lines, one separates the first and last -->`
`}`

--------

`.header {`
    `grid-column-start: 1; <--! first column line -->`
    `grid-column-end: 3;   <--! third column line -->`
`}`


`and same thing:`


`.header {`
    `grid-column: 1 / 3;`
`}`



------

`.footer {`
    `grid-column: 1 / span 2; <--! star at first column line and span across 2 columns -->`
`}`

--------

`.footer {`
    `grid-column: 1 / -1; <--! star at frst column line and targets the last column line -->`
`}`
