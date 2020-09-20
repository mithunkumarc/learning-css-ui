### styles can be combined to apply specific style

#### index.html

        <div class="container">
          <div class="item"></div>
          <div class="item special"></div>     /* class item and special combined here to apply specific style*/
          <div class="item"></div>
        </div>

style.css

          /*parent container*/
          .container {

          }

          .item {
            /*normal child style */
          }

          .special {
            /*special child style */
          }

