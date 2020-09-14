Units : 
1. pixels :           px
2. percentages :      %
3. root em :          rem : fontsize
4. em :               em : fontsize
5. viewport height :  vh (instead of 100% height to conver screen u can use 100vh)
6. viewport widht :   vw (instead of 100% width to conver screen u can use 100vw)

questions:  
1. how is the size calculated
2. what is the right unit to choose
3. which properties can i use in connection with these units?

1. Absolute lenghts : 
these are fixed sizes examples : px, cm , mm . we should avoid use these.
use only when you need absolute lengths.

2. Viewport lenghts : 
vh, vw. vmin , vmax.

3. Font Relative lenghts ; 
adjust to default font size : 

rem
em

4. percentages : with respect to parent

#### max width , max height : if u keep on increasing screen size percentage image also keep increase ,so u can restrict using max width pixels

### if fonts are changed in browser settings, the unset fontsize in css will change according to browser settings.
### if u have set the size for fonts in css, browser fontsize settings will not have any impact.
### if u want to change your font with respect to browser settings use em or rem
### drawback of em : inherits parent size and multiplies, use em when there is no inheritance complexity.
### use rem when there is complexity issues. caluculation : browsersetting fontsize multiplied by (number)rem.

## Rules to remember : 

1. if the element has position fixed then parent might be viewport. so use width/height as %. pixel varies when screen resized so use %.

2. if the element has position absolute, check parent element(includes padding) position property ; absolure, relative, fixed and sticky. use percentage in child.

3. if the element position is static/relative ancestor migth be block level element or viewport(outer screen)  

### which unit i use : 

1. font size : rem( em : children only)
2. padding/margin : rem (dynamic size with respect to user font setting)
3. border : px (fixed size, px doesnt vary with respect to user font setting)
4. width height : % or vw, % or vh
5. top bottom left right : %



