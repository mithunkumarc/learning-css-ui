if you have two elements one above other,  
bottom margin of top element and Top margin of bottom element merge.  
if two elements has different margin, bigger one wins  
finally there will be only one margin  


        <!DOCTYPE html>
          <body>
          <h2>First</h2>  <!-- bottom margin will merge with h1-->
          <h1>Second</h1> <!-- top margin will merge with h2-->
          </body>
        </html>


#### this behaviour cannot be changed, this is how css works
#### best practice , use either top or bottom margin according to requirement


### Rules of margin collapsing 

1. happens only vertically
2. happens only with block line elements
3. happens only if two elements directly in contact with each other
