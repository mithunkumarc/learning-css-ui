### container vs container-fluid

        container : fixed size, takes margin on either sides
        container-fluid: full screen

### grid system: each row can be divided into 12 columns

        if you add 13th column it will appear in next line as if it belong to next row.

### check responsiveness of your site

        * check responsiveness of bootstrap running in server
        * you may not see responsiveness when u open page directly

        check your page how much respon it is
        https://responsivedesignchecker.com/

### breakpoints : 

1. extra large : .col-xl-number : 	>=1200px
2. large :  .col-lg-number :  >=992px
3. medium :  .col-md-number : >=768px	
4. small : .col-sm-number : >=576px	
5. extra-small : .col-number : <576px	

## extra-large : >=1200px : col-xl-number

        if your screen size is >=1200px grid system works
        if screen size is < 1200px , grid system breaks, each column will
        show one below other vertically



## large : >=992px : col-lg-number

        supports both large and extra large screens.
        if your screen size is >=992px grid system works.
        if your screen size is < 992px grid system breaks, each column
        appear one below other , like all belong to single column.


## medium : >=768px : col-md-number 

        supports medium , large, extra large
        if your screen size is >=768px, grid system works.
        if your screen size is < 768px, grid breaks, each column
        display one above other vertically.

## small :  >= 576px : col-sm-number

        supports small, medium, large, extra large 
        if screen size is >=576px grid system works 
        if screen size is < 576px grid system breaks each column appear 
        one above other vertically.

## extra small : < 576 : col-number 

        supports all 
        grid never breaks



## supporting multiple breakpoints 

        eg : col-lg-2 col-xl-3
        col-lg-2 : 6 columns in row : 6 * 2 = 12 (grid consists of 12 col)
        col-xl-3 : 4 columns is row : 3 * 4 = 12 (grid consists of 12 col)
        in large screen >=992px : all colums appear in single row 
        in extra large screen >=12000 : four column appear in single row 
        remaining will go to next line(each line can have 4 columns) 

        <div class="col-lg-2 col-xl-3"></div>
        <div class="col-lg-2 col-xl-3"></div>
        <div class="col-lg-2 col-xl-3"></div>
        <div class="col-lg-2 col-xl-3"></div>
        <div class="col-lg-2 col-xl-3"></div>
        <div class="col-lg-2 col-xl-3"></div>
