element height indicates height of content. border and margin adds extra height to element.

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

By default, when you set height of an element, you are setting for content. 
if you add border and padding, the element size becomes bigger.  

To solve this issue, box-sizing property helps you keep element height same 
even if you add border and padding.(border and padding takes height of content).    


example : 

html : 

        <!DOCTYPE html>
          <body>
            <p>hello world</p>
            <div>hello earth</div>
          </body>
        </html>


style.css

                /* 
                  both styles are same.
                  but as soon as we add padding to tag p, the size of p tag grows.
                  so, by default height means , content height of element.
                  adding paddng and border makes element bigger.
                  if you keep element size same event after adding border and padding 
                  use box sizing property.
                */


                p {
                  font-size: 30px;
                  background-color: yellow;
                  height: 100px;
                  width: 300px;
                  padding: 5px;
                  margin:0px;
                }

                div {
                  font-size: 30px;
                  background-color: red;
                  height: 100px;
                  width: 300px;
                  margin:0px;
                  /* uncomment below to apply border box, you can see element dont grow bigger even after adding padding, becuase of box sizing property */
                  /* padding: 5px;
                  box-sizing: border-box; */
                }
