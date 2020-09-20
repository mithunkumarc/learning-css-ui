flex container is parent, flex items are children.  
each flex children can become flex container on their own.

index.html

          <!DOCTYPE html>
            <head>
              <meta name="viewport" content="width=device-width, initial-scale=1.0">
            </head>
            <body>
                <div class="container">   <!-- this is flex container -->
                  <div class="item">      <!-- flex item: children -->
                    Content : ONE : This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
                  </div>
                  <div class="item">      <!-- flex item: children -->
                    Content : TWO : This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
                  </div>
                  <div class="item special">    <!-- flex item: children, but this is also flex container, having own children -->
                    <div>one</div>                <!-- flex item: children -->
                    <div>two</div>                <!-- flex item: children -->  
                    <div>three</div>              <!-- flex item: children -->
                  </div>
                </div>
            </body
          </html>
          
#### style.css

          .container {
            display: flex;
            height: 350px;
            border-style: solid;
            border-width: 2px;
          }

          .container > .item {
            background-color: yellow;
            border-style: solid;
            border-width: 2px;
            margin: 5px;
            padding: 5px;
            width: 200px;
            height: fit-content;
          }

          .special {
            display: flex;
            justify-content: space-between;
          }
