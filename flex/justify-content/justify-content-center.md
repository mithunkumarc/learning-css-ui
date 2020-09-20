justify-content: center;

            this will bring flex items to the center on the main axis.
            if flex-direction is row, flex items will appear at the center horizontally.
            if flex-direction is column, flex items will appear at the center horizontally.

style.css

            .container {
              display: flex;
              flex-direction: row;
              height: 350px;
              border-style: solid;
              border-width: 2px;
              justify-content: center;   /* this will brind flex items(children) to the center on main axis */
            }

            .container > .item {
              background-color: yellow;
              border-style: solid;
              border-width: 2px;
              margin: 5px;
              padding: 5px;
              width: 200px;
              height: fit-content;
              display: flex;
              flex-direction: initial;
            }

index.html

            <!DOCTYPE html>
              <head>
                <meta name="viewport" content="width=device-width, initial-scale=1.0">
              </head>
              <body>
                  <div class="container">
                    <div class="item">
                      Content : ONE : This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
                    </div>
                    <div class="item">
                      Content : TWO : This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
                    </div>
                    <div class="item">
                      <div>one</div>
                      <div>two</div>
                      <div>three</div>
                    </div>
                  </div>
              </body
            </html>
