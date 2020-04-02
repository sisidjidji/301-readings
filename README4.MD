# READ4

## 1. Grid : 

- CSS Grid Layout (aka “Grid”), is a two-dimensional grid-based layout system that aims to do nothing less than completely change the way we design grid-based user interfaces

- we can  define a container element as a grid with **display: grid**, set the column and row sizes with **grid-template-columns** and **grid-template-rows**, and then place its child elements into the grid with **grid-column** and grid-row

- display Defines the element as a grid container and establishes a new grid formatting context for its contents.

                          .container {
                           display: grid | inline-grid;
                                    }
- **grid-template-columns ,grid-template-rows** :Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.
                            .container {
                           grid-template-columns:  ... |   ...;
                           grid-template-rows:  ... |   ...;
                                       }
                    
- **grid-template-areas** :Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property. 
                            .container {
                            grid-template-areas: 
                            " | . | none | ..."
                            "...";
                                        
- **grid-template** :A shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.

- **grid-column-gap,grid-row-gap** :Specifies the size of the grid lines. You can think of it like setting the width of the gutters between the columns/rows.
                            .container {
                            grid-column-gap: ;
                            grid-row-gap: ;
                                       }

- **grid-gap**: A shorthand for grid-row-gap and grid-column-gap

- **justify-items:**Aligns grid items along the inline (row) axis (as opposed to align-items which aligns along the block (column) axis). This value applies to all grid items inside the container.

- **align-items**:Aligns grid items along the block (column) axis (as opposed to justify-items which aligns along the inline (row) axis). This value applies to all grid items inside the container.

- **place-items**: place-items sets both the align-items and justify-items properties in a single declaration.

- **place-content**:place-content sets both the align-content and justify-content properties in a single declaration.

 # 2. RegExr:
 
 - Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).
                    