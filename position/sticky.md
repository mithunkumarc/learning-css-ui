postion behaviour studied with respect to top/bottom or left/right.

case 1 : when parent container is outer screen/viewport
    
          sticky element , when reaches its top/bottom or left/right positio, its position become fixed. it will not move on scrolling.
          
          example : 
          
          .box {
              height: 40px;
              width: 40px;
              border-style: solid;
              border-color: green;
              position: sticky;
              top: 30px;      /*on reaching top 30px, its position becomes fixed, will not scroll/move */
            }

case 2 : when parent is another container like div. (parent need not to have position property)

          sticky element, when reaches its top/bottom or left/right position, its position becomes fixed. if
          if parent container disappears on scrolling, sticky element also disappears along with parent.
          
          
          html 

            <div class="container">
              <div class="box"></div>
            </div>
          
          
          style.css  : 
          
          .container {
              height: 400px;
              width: 400px;
              border-style: solid;
              border-color: red;
            }

            .box {
              height: 40px;
              width: 40px;
              border-style: solid;
              border-color: green;
              position: sticky;
              top: 30px;    /* element becomes fixed at top 30px , but if parent container disappears, sticky box also disappear with parent */
            }
