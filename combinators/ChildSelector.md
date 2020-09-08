style is applied only to direct child tags, not nested child tags


        The following example selects all <p> elements that are children of a <div> element:

        div > p {
          background-color: yellow;
        }


style.css

          div > p {     /* direct p tag child of div tag gets style */
            font-size: 30px;
            background-color: yellow;
          }
          p {
            font-size: 20px;
          }

index.html

          <!DOCTYPE html>
            <body>
              <div>
                <p>First</p> <!-- child selected applied : direct child-->
                <artice>
                  <p>Second</p>       <!-- not applied: nested child -->
                </artice>
                <p>Third</p> <!-- child selected applied : direct child -->
              </div>

              <p>Third</p>    <!-- not applied: outside -->

            </body>
          </html>
