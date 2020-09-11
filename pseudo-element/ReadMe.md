A CSS pseudo-element is used to style specified parts of an element.

        For example, it can be used to:

        Style the first letter, or line, of an element
        Insert content before, or after, the content of an element

syntax: 

        selector::pseudo-element {
          property: value;
        }

example : first letter has 30px font size and text color is red

        p::first-letter {
          color: red;
          font-size: 30px;
        }
        
        /*Adds text Teacher after <p> tag content*/
        p::after {
          content: ' Teacher';
          color: red;
        }
