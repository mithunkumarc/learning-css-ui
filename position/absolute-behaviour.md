#### aboslute element always come out of normal flow of document, its space will be taken by below element.  
#### if your element is aboslute, its movement (top/bottom left/right) will be with respect to its parent.  
#### condition : parent must be with position relative. or else outer screen will be considered as parent.  

example : index.html

          <!DOCTYPE html>
            <body>
              <div>Google News is a news aggregator service developed by Google. It presents a continuous flow of articles organized from thousands of publishers and magazines. Google News is available as an app on Android, iOS, and the Web. Google released a beta version in September 2002 and the official app in January 2006. Wikipedia</div>

              <div class="container">
                <div class="box"></div>
              </div>

            </body>
          </html>


style.css : case 1 : parent element is not relative

          .container {
            height: 400px;
            width: 400px;
            border-style: solid;
            border-color: red;
            /* position: relative; */     /* here u can see parent container is not reative*/
          }

          .box {
            height: 40px;
            width: 40px;
            border-style: solid;
            border-color: green;
            position: absolute;       /*parent container is not relative, so box will move with respect to outer screen*/
            top: 0px;                 /* box will move to top 0px left 0px with respect to outer screen */ 
            left: 0px;
          }



style.css : case 2 : parent element is relative


            .container {
              height: 400px;
              width: 400px;
              border-style: solid;
              border-color: red;
              position: relative;     /* parent container is relative */
            }

            .box {
              height: 40px;
              width: 40px;
              border-style: solid;
              border-color: green;
              position: absolute;   /* parent conatiner is relative*/
              top: 0px;             /* box will move top left of parent container*/
              left: 0px;
            }
