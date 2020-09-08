
By Default : text styles are inherited from parent Elements to Child Elements.

eg : 
style.css

        body {
          font-size: 30px;
        }
        
index.html 

        <!DOCTYPE html>
        <body>
          <div>
            <p>hello</p>            <!-- inherits font size from body -->
          </div>
          <span>world</span>        <!-- inherits font size from body -->
        </body>
        </html>

both div.p and span both inherit font-size from body

Note: Not all styles are inherited , only styles related to text(fonts) are inherited. Borders, padding and margins are not inherited.


reference : http://tutorials.jenkov.com/css/inheritance.html  
