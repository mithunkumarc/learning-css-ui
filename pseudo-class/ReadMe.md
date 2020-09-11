Pseudo-Class : used to define a special state of an element.

For example, it can be used to:

        Style an element when a user mouses over it
        Style visited and unvisited links differently
        Style an element when it gets focus

syntax : 

        selector:pseudo-class {
          property: value;
        }

reference:  https://www.w3schools.com/css/css_pseudo_classes.asp

example : 

                p {
                  font-size: 30px;
                  font-weight: bold;
                }

                /* when element is hovered */
                p:hover {
                  color: red;
                  font-size: 30px;
                  font-weight: bold;
                }

                /* when element is clicked */
                p:active {
                  color: yellow;
                  font-size: 30px;
                  font-weight: bold;
                  background-color: red;
                }


#### pseudo class vs pseudo element : 

A CSS pseudo-element is used to style specified parts of an element.

        For example, it can be used to:

        Style the first letter, or line, of an element
        Insert content before, or after, the content of an element


### Grouping pseudo classes : if two pseudo class has same style then group them together

#### example : grouping hover and active together since they need same functionality

        p:hover,active {
          color: red;
          font-size: 30px;
          font-weight: bold;
        }

