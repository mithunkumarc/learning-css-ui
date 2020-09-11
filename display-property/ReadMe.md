
inline : takes width equal to content, if you try to set height and width, they are ignored.  
block : takes full line, you can set height and width to element.  
inline-block : normarlly inline element ignores height and width, but you can set height and width to inline-block element.   
none : element will be hidden from view but can be seen in dom.  

inline-block: important : you can use this property to bring two inline or block elements in same line and partition the screen. but bootstrap has better solution.

        .left {
          width : 30%;
          background-color: yellow;
          height: 100%;
          display: inline-block;
        }

        .right {
          width : 60%; 
          background-color: red;
          height: 100%;
          display: inline-block;
        }

        body {
          height: 100%;
        }

        html {
          height: 100%;
        }
