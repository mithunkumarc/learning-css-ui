The following example selects all <p> elements that are placed immediately after <div> elements:


        div + p {     /* any p tag next to div tag will get style, only immediate p tags which appear after div */
          font-size: 30px;
          background-color: yellow;
        }
        
        
example : style.css

        div + p {
          font-size: 30px;
          background-color: yellow;
        }
        
        
index.html 

        <!DOCTYPE html>
          <body>

            <p>Heading</p> <!-- not applied here as p tag comes before div -->
            
            <div>
              <p>First</p>   <!-- not applied here , not adjacent to div , this is inside div -->
              <p>Second</p>  <!-- not applied here -->
            </div>
            
            <p>Third</p>   <!-- tyle applied here , this tag is adjacent to div -->
          </body>
          
        </html>
