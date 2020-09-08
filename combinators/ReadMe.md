combinators : 

                CSS combinators are explaining the relationship between two selectors. 

general example (descendants exmple) style.css

        div p {   /* combintaion of tags to increase specificity, if p tag present inside div , apply this style */
          /* 
            by default p has 20px because of below style declare <p> as 20px
            but div p is overriding 20px by 40px 
           */
          font-size: 40px;
        }
        p {
          font-size: 20px;
        }
        
        
index.html :

        <!DOCTYPE html>
        <body>
          <div>
            <p>hello</p>
          </div>
          <p>world</p>
        </body>
        </html>
