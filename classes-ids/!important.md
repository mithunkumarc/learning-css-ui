style.css

        .first {
          color: red !important;
          font-size: 30px;
        }

        /* assuming both styles first and second applied to tag p , check html*/
        /* by default second yellow color has high priority, but !important overriding to red  */
        .second {
          color: yellow;
          font-size: 30px;
        }


index.html

        <!DOCTYPE html>
          <body>

              <div class="first second"> hello </div>       /* red applied because of !important value*/

          </body>
        </html>
        
        
#### !important: dont use more often        
