/* 
  by default flex items (child elements) dispaly side by side ,if you want you can change it to column by using flex-direction: column 
  using media query if the screen size is 40rem and below, flex items made appear one below other. (flex-direction: column)
*/


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

          /* 
            1 rem = 16 px 
            40 rem = 640 px
            rem is flexible with browser settings
           */
           /* portrait - default : if screen width is upto 40rem, apply this */
          @media screen and (max-width: 40rem) {
            .container {
              flex-direction: column;
            }
          }
