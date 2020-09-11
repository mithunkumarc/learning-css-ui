The :not(selector) selector matches every element that is NOT the specified element/selector.

#### example: if div tag has not having first class, yellow color is set to text

        div {
          font-size: 30px;
        }

        .first {
          color: blue;
        }

        .second {
          color: red;
        }

        /* any div tag which don't have first class, will get text as yellow */
        div:not(.first) {
          color: yellow;
        }

index.html

        <!DOCTYPE html>
          <body>

              <div class="first"> hello </div> <!-- yellow not applied -->
              <div class="second"> world </div> <!-- yellow applied -->
              <div>css</div> <!-- yellow applied -->
          </body>
        </html>


