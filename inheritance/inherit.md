by default text related styles are inherited.   (padding,margin,color not inherited)

In some cases, a specific property may not be inheritable but you might still want it to be inherited from the parent element.   
This can be achieved by setting the value of that property to inherit for the child element:  


The inherit keyword specifies that a property should inherit its value from its parent element.  

eg : span tag color inherit .extra class color

        .extra span {
            color: inherit;
        }
