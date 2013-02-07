#LESS - Checkbox Mixin

##Overview

This is a very simple mixin allowing you to style checkboxes with pure CSS.

##Requirements

This is a LESS mixin so you have to add it to your file or include the file using 

```
@import "lch-checkbox.less";
```

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
##The future

If I have enough time I might expand this tiny project into a little library of mixins