#### reference
	
		https://www.youtube.com/playlist?list=PLbGui_ZYuhij_HswuaGK-ABs1vfC5HTKn

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




#### auto column size : takes auto size : supports all devices 

                as long as there are 12columns
                
                ex : 12 col divided to 3cols each 
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>
                <div class="col"></div>

                exg :
                below example : first two and last takes 2 cols each
                third div takes 6 cols
                
                <div class="col"></div>
                <div class="col"></div>
                <div class="col-6"></div>
                <div class="col"></div>


### column break : taking column to next line

                <div class="col-4></div> // first row
                <div class="col-4></div> // first row 
                <div class="w-100"></div> // break row 
                <div class="col-4></div> // next row

### order-first : giving priority to columns

        column can make appear first 

### order-last : makes column to appear last in row

### order-number : 

        if you use this , you should give order to all columns


### offset columns : creating margin left side of col(empty)

        ex : 
                <div class="col-md-3"></div>
	        <div class="col-md-3 offset-md-6"></div> // creating 6 col margin to the left side

	        first div takes 3 col in md, 6 col offset(margin), second div takes 3 col md
	 
	 

#### using responsive col 

 	<div>
		<div class="col-sm-3"></div> <!-- 1 -->
 		<div class="col-sm-9"></div> <! -- 2 -->
	</div>
 
	1. takes 3 cells in grid out of 12 above small devices
 	less than it become responsive 
 	2. takes 9 cells in grid out of 12 above small devices

  	1 and 2 shows in rows above small devices
   	1 and 2 shows in columns below samll devices
