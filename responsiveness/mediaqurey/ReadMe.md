you can target style for specific screen size : test below styles in developer tools by reducing screen size

html
         
          <div class="candidate_name">Ravi Shankar</div>

style.css : put all media queries at the bottom of style sheet: bestpractice

          /*style for desktop*/
          .candidate_name {
            font-size: 20px;
            font-weight: bold;
            color: #33aa11;
            width: 100%;
            text-align: center;
          }


          /*for screensize 880px and below i want fontsize of candidate name is 15px and color is rebeccapurple */
          @media(max-width:880px) {
            .candidate_name {
              font-size: 15px;
              color: rebeccapurple;
            }
          }


          /*for screensize 880px and above i want fontsize of candidate name is 15px and color is rebeccapurple */
          @media(min-width:880px) {
            .candidate_name {
              font-size: 15px;
              color: rebeccapurple;
            }
          }
          
#### handling responsiveness with portrait and landscape : 


                  @media(max-width:880px) and (orientation:portrait){
                              .candidate_name {
                                font-size: 15px;      /*change according values*/
                                color: rebeccapurple;
                              }
                            }


                  @media(max-width:880px) and (orientation:landscape){
                              .candidate_name {
                                font-size: 15px;    /*change according values*/
                                color: rebeccapurple;
                              }
                            }
