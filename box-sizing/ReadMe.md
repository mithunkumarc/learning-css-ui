element height indicates height of content. border and margin adds extra height.  
inspecting element p shows height as 120.  
content height we set is 100px. see box model.    
20px comes padding top and bottom.  
border and margin takes extra 10px each.  

style.css

        p {
          font-size: 30px;
          border-width: 10px;
          margin: 10px;
          padding: 10px;
          height: 100px;
        }

index.html

        <!DOCTYPE html>
          <body>
            <p>hello world</p>
          </body>
        </html>

       
#### CSS box-sizing Property
