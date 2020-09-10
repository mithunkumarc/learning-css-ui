height propery = height of content(includes border and padding), excludes margin.


width of the block line element can be varied , but it still takes full line. 
so change display property to inline, now element width equal to the width value we have set

eg : section is a block line

        section {
          border-style: dotted;
          width: 40px;              /* size set for 40 px */
          background-color: yellow;
          margin: 0px;
          display: inline;          /* changed to inline */
        }
        
height : if you want to set height of element relative to height of parent. 

If the height of the containing block is not specified explicitly, and the element is not absolutely positioned, 
the value of its height computes to auto (it will be as tall as the content inside it is, or zero if there is no content). 
If the elements content portion requires more vertical space than available from the value assigned, the elements behavior is defined by the overflow property.

When using the keyword auto, height is calculated based on the elements content area unless explicitly specified. 
This means a value based on a percentage is still that of the elements content area. 
Similarly, if the height of the container is set to a percentage value, a child elements percentage height is still based on the content area of that child element.


parent : 100%
child : 50% : half of parent height


example

        <!DOCTYPE html>
          <body>
            <main>
              <section>hello</section>
            </main>
          </body>
        </html>

        section {
          height: 50%;
          background-color: yellow;
        }
        main {
          background-color: red;
          height: 50%;
        }
        body {
          height: 50%;
          background-color: darkturquoise;
        }
        html {
          height: 100%;
          background-color: blue;
        }

#### height and width property sets the height and widht of content. It doesn't include border, padding or margin.

#### auto vs 100%

height: 100% gives the element 100% height of its parent container.  
height: auto means the element height will depend upon the height of its children.  
