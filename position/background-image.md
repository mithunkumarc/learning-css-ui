style.css : position is used to set background image

        .background {
          background: url("https://upload.wikimedia.org/wikipedia/commons/thumb/3/3e/The_cricket_legend_Sachin_Tendulkar_at_the_Oval_Maidan_in_Mumbai_During_the_Duke_and_Duchess_of_Cambridge_Visit%2826271019082%29.jpg/260px-The_cricket_legend_Sachin_Tendulkar_at_the_Oval_Maidan_in_Mumbai_During_the_Duke_and_Duchess_of_Cambridge_Visit%2826271019082%29.jpg")
          ;
          height: 100%;         /* bg image taking full screen */ 
          width: 100%;          /* bg image taking full screen */
          position: fixed;      /* comes out of normal flow, appear above other elements */
          z-index: -1;          /* bg image pushing below other elements */
        }


index.html

        <!DOCTYPE html>
          <body>
            <div class="background"></div>    <!-- inserting background image -->
            <div>hello world</div>            <!-- all these content appear above image -->
            <div>hello world</div>
            <div>hello world</div>
            <div>hello world</div>
            <div>hello world</div>
            <div>hello world</div>
            <div>hello world</div>
          </body>
        </html>


refer : https://www.w3schools.com/cssref/css3_pr_background-size.asp
https://www.w3schools.com/cssref/pr_background-position.asp
