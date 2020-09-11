any tag with class message has parent div, will get this style

tag with message class position doesn't matter ,as long as they are inside div tag. refer combinators for more info

        div .message {
          font-size: 40px;
          color: yellow;
        }
        
index.html

        <!DOCTYPE html>
          <body>

              <div>

                <p class="message">First</p>          <!-- style applied -->
                <p>Second</p>
                <section>
                  <p class="message">Third</p>        <!-- style applied -->
                </section>
              </p>

          </body>
        </html>
