example:

.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 50px 50px;
    grid-gap: 3px;
}
            
    same thing as:
    
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 50px);
    grid-gap: 3px;
}


    and same thing as:
    
.container {
    display: grid;
    grid-template: repeat(2, 50px) / repeat(3, 1fr);
    grid-gap: 3px;
}


-----


.header {
    grid-column-start: 1; <--! first column line -->
    grid-column-end: 3;   <--! third column line -->
}


and same thing:


.header {
    grid-column: 1 / 3;
}


------


.footer {
    grid-column: 1 / span 2; <--! star at frst collumn line and span across 2 collumns -->
}


--------


.footer {
    grid-column: 1 / -1; <--! star at frst collumn line and targets the last collumn line -->
}

