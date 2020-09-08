style applied to all sibling which comes after not before


        div ~ p {   /* all p tags which are siblings and appear after div applied */
          background-color: yellow;
        }
        
        
Example : style.css

        div ~ p {
          font-size: 30px;
          background-color: yellow;
        }
        
index.html

        <!DOCTYPE html>
          <body>
            <p>before text</p>    <!-- not applied : comes before div -->
            <div>
            </div>
            <p>after text</p>     <!-- applied here, its immediate sibling to div -->
            <article>some article</article> 
            <p>final text</p>     <!-- applied here, general sibling -->
          </body>
        </html>
