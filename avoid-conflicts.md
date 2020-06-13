#### How to avoid conflicts

        While writing your CSS, it’s easy to write conflicting rules, where the same property is applied several times.

#### only use classes: 

        use .introduction instead of #introduction, even if that element only appears once in your webpage

#### avoid applying multiple classes on a single HTML element: 

        don’t write 
        <p class="big red important"> 
        but rather 
        <p class="title"> which is more semantically descriptive

#### don’t use inline styles like 

        <div style="background: blue;">
