#### An HTML element can be targeted by multiple CSS rules.

         inline                                   first
         #id selectors are worth 100              second priority
        .class selectors are worth 10             third priority
        tag selectors are worth 1                 fourth priority eg : <h1> <p>


#### priority

         inline > id > class/pseudoclass/attribute selectors > tag/pseudo element selectors


#### Order of CSS rules

        If similar selectors are in your CSS, the last one defined will take priority.

        p{ color: green;}
        p{ color: red;}       # this style wins
         
class will have high priority in this case

        .mycolor { color: blue}    
        p{ color: green;}
        p{ color: red;}       # if <p> uses class mycolor, mycolor always wins 

         
