lets say there is a container. container consists of an element.   
if you move element in such a way that its position goes out of container, you can control its visibitliy by using overflow property.  
overflow property is set to parent.   

values of overflow  

        visible: by default
        hidden : The overflow is clipped, and the rest of the content will be invisible
        scroll : The overflow is clipped, and a scrollbar is added to see the rest of the content
        auto : Similar to scroll, but it adds scrollbars only when necessary
        
example : index.html

        <!DOCTYPE html>
          <body>
            <div>Google News is a news aggregator service developed by Google. It presents a continuous flow of articles organized from thousands of publishers and magazines. Google News is available as an app on Android, iOS, and the Web. Google released a beta version in September 2002 and the official app in January 2006. Wikipedia</div>

            <div class="container">
              <div class="box"></div>
            </div>

          </body>
        </html>
        
style.css

        .container {
          height: 400px;
          width: 400px;
          border-style: solid;
          border-color: red;
          position: relative;       /*if child is absolute, this container becomes parent*/
          overflow: scroll;         /* overflow content will be scrolle */
        }

        .box {
          height: 40px;
          width: 40px;
          border-style: solid;
          border-color: green;
          position: absolute;       /*is is aboslute, parent has position property. its position based on parent continer*/
          top: 370px;               /* this box will move 370px away from top of container, some part will be clipped , but visible on scrolling */
          left: 0px;
        }


#### Note; If element parent is body, if overflow not working after declaring in body, try adding overflow property in html too.
