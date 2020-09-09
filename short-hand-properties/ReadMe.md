Shorthand properties are CSS properties that let you set the values of multiple other CSS properties simultaneously. 
Using a shorthand property, you can write more concise (and often more readable) style sheets, saving time and energy.

example : 

        p {
          border-style: solid;
          border-width: 3px;
          border-color: black;
          height: 30px;
          width: 100px;
          text-align: center;
        }

border is redundant so it can be written as 

        p {
          border: 3px solid black;
          height: 30px;
          width: 100px;
          text-align: center;
        }



shortand for margin :

        p {
          margin-top: 5px;
          margin-bottom: 5px;
          margin-left: 5px;
          margin-right: 5px;
        }

        /* above can be written as */
        p {
          margin: 5px 5px 5px 5px;
        }

        /* top bottom and left right */
        p {
          margin: 5px 5px;
        } 


        /* all sides margin */
        p {
          margin: 5px;
        }
