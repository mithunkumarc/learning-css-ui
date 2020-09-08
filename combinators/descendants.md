The descendant selector matches all elements that are descendants of a specified element.  


      The following example selects all <p> elements inside <div> elements:  

      div p {
        background-color: yellow;
      }
      
      if p tag exists inside div tag, style will be applied, it doesn't matter how deep p tag is present. as long as p inside div , style always applied

index.html 


        <!DOCTYPE html>
        <body>
          <div>
            <p>hello</p>  <!-- div p style applied here  -->
            <p>css</p>  <!-- div p style applied here  -->
            <span>
              <p>inner tag</p>  <!-- div p style applice here too -->
              <h1><p>deep inner tag</p></h1> <!-- div p style applice here too -->
            </span>
          </div>
          <div>
            <artice>
              <p>another example</p><!-- div p style applice here too -->
            </artice>
            </div>
          <p>world</p> <!-- div p style not appliec -->
        </body>
        </html>
