#LESS - Checkbox Mixin

##Overview

This is a very simple mixin allowing you to style checkboxes with pure CSS.

##Requirements

This is a LESS mixin so you have to add it to your file or include the file using 

```
@import "lch-checkbox.less";
```

And you also need to have a means to compile the files. 
There are several tools around, like the original js compiler ( http://lesscss.org/ ) and it's tools lessc. 
Also there are a number of apps which you can use to pcompile your LESS code. 
I am on windows and use WinLESS ( http://winless.org/ ). SimpLESS ( http://wearekiss.com/simpless ) is another great option.
I am pretty sure there are similar tools for other platforms too.


##Usage

There's a set of default values for the checkbox but you can configure it in a variaty of ways with the mixin arguments.

**This is a sample call with clarification of the arguments in the same order:**

```
    //    @background - Checkbox background
    //    @color - Text color
    //    @fontSize - Font size
    //    @width - Width of the checkbox
    //    @height - Height of the checkbox
    //    @lineHeight - Line height for the checkbox
    //    @textAlign - Text align for the text 
    //    @display - Display type
    //    @border - Border style/color/size
    //    @borderRadius - Border radius
    //    @hoverColor - Text color for hover state
    //    @hoverBackground - Background for hover state
    //    @activeColor - Text colro for active state
    //    @activeBackground - Background for active state

    .lch-checkbox(#fff, #333, 13px, 50px, 20px, 20px, center, block, 1px solid #ccc, 5px, #666, #efefef, #fff, #27b4ff);
```

This call generates this CSS code when compiled:

```
    .demo-checkbox {
      position: absolute;
      top: -9999em;
    }
    .demo-checkbox + label {
      background: #ffffff;
      color: #333333;
      font-size: 13px;
      width: 50px;
      height: 20px;
      line-height: 20px;
      text-align: center;
      display: block;
      border: 1px solid #cccccc;
      border-radius: 5px;
      cursor: pointer;
    }
    .demo-checkbox + label:hover {
      color: #666666;
      background: #efefef;
    }
    .demo-checkbox:checked + label {
      background: #27b4ff;
      color: #ffffff;
    }
    
```

##The future

~~If I have enough time I might expand this tiny project into a little library of mixins~~
When I have enough time ( hopefully in the near future ) I will expand this tiny project into a little library of mixins. 
I've alreay created a public Trello board where you can track the progres, vote and comment, should you wish so.

***Link to Trello: https://trello.com/board/less-interface-mixing-library/511f4eaf3ded8bbb6100172f***