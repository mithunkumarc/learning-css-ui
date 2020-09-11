style.css : both styles will be applied

      .mainheader {
        font-size: 40px;
        color: yellow;  
      }
      .importance {
        color: red;      /*if both style has same color : this has high priority*/
      }


index.html

      <!DOCTYPE html>
        <body>

            <p class="mainheader importance">Hello</p>            <!-- font size 40px and color red-->

        </body>
      </html>
