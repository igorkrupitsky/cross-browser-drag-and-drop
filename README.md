# Cross-browser drag and drop

Originally posted here:
https://www.codeproject.com/Articles/226193/cross-browser-drag-and-drop

This article explains how to make drag and drop work across multiple browsers.

## Introduction
I could not find a good Drag and Drop JavaScript example that would work in all browsers (including iPad). So I wrote one myself. I hope someone might find it useful. Please note that this example shows how to “capture” the element so that you don’t lose it if you move outside of the element or outside of the browser window.

Unfortunately, I could not find a good way how not to lose capture over an iFrame in Chrome and Safari. The best approach I found is to cover all iFrames with DIVs while the dragging is taking place. Any suggestions on how to do this better are welcome.

This article is for those that like nuts and bolts and are not using third party libraries like jQuery. There is nothing wrong with using third party libraries – I just like more flexibility. For example, you can use this example to resize elements.

![](img/DragDrop.gif)

## Using the code
To use this script, use the MakeDragable JavaScript function. It accepts only one parameter: the ID of the element you want users to drag. 
