https://www.youtube.com/watch?v=sanswTlz4ZY

space between can be created using flex: 1 1 auto;  
flex: grow shrink basic_size_of_content;  
 
for space(divider in this case) is allowed to grow(1) and shrink(1) and basic size is auto.  
if grow is 1, item will take available space pusing logo and options to ends of screen left and right.  

      
      <div class="container">
              <div class="logo">logo</div>
              <div class="divider"></div>
              <div class="options">options</div>
          </div>
      
      
          
      .divider {
          flex: 1 1 auto;
      }
      
      .container {
          display: flex;
      }
