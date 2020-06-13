#### An HTML element can be targeted by multiple CSS rules.


         #id selectors are worth 100              first priority
        .class selectors are worth 10             second priority
        tag selectors are worth 1                 third priority


#### Order of CSS rules

        If similar selectors are in your CSS, the last one defined will take priority.

        p{ color: green;}
        p{ color: red;}       # this style wins
