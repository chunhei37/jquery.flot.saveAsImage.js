jquery.flot.saveAsImage.js
==========================

Flot plugin that adds a function to allow user save the current graph as an image by right clicking on the graph and then choose "Save image as ..." to local disk.

Copyright (c) 2013 http://zizhujy.com.
Licensed under the MIT license.

Usage:
    Inside the <head></head> area of your html page, add the following lines:
    
    <script type="text/javascript" src="http://zizhujy.com/Scripts/base64.js"></script>
    <script type="text/javascript" src="http://zizhujy.com/Scripts/drawing/canvas2image.js"></script>
    <script type="text/javascript" src="http://zizhujy.com/Scripts/flot/jquery.flot.saveAsImage.js"></script>

    Now you are all set. Right click on your flot canvas, you will see the "Save image as ..." option.

Online examples:
    http://zizhujy.com/FunctionGrapher is using it, you can try right clicking on the function graphs and
    you will see you can save the image to local disk.

Dependencies:
    This plugin references the base64.js and canvas2image.js.

Customizations:
    The default behavior of this plugin is dynamically creating an image from the flot canvas, and then puts the 
    image above the flot canvas. If you want to add some css effects on to the dynamically created image, you can
    apply whatever css styles on to it, only remember to make sure the css class name is set correspondingly by 
    the options object of this plugin. You can also customize the image format through this options object:

    options: {
        imageClassName: "canvas-image",
        imageFormat: "png"
    }
