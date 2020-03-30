# 301-readings
# Summary
# 1.What is "Float"?
# 2.Clearing the Float
# 3.Techniques for Clearing Floats
# 4.Flexible Layouts



# 1.What is "Float"?

- Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called "text wrap". 

- There are four valid values for the float property. **Left** and **Right** float elements those directions respectively. **None** (the default) ensures the element will not float and **Inherit** which will assume the float value from that elements parent element.

# 2.Clearing the Float:
 An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float. 

 - Clear has four valid values as well. **Both** is most commonly used, which clears floats coming from either direction. **Left** and **Right** can be used to only clear the float from one direction respectively. **None** is the default, which is typically unnecessary unless removing a clear value from a cascade. **Inherit** would be the fifth, but is strangely not supported in Internet Explorer. 

 # 3.Techniques for Clearing Floats

 * The Empty Div Method
 * The Overflow Method
 * The Easy Clearing Method 


# 4.Flexible Layouts

CSS3 introduced some new relative length units, specifically related to the viewport size of the browser or device. These new units include 

* vw: Viewports width 
* vh: Viewports height
* vmin :Minimum of the viewport’s height and width
* vmax: Maximum of the viewport’s height and width


The formula is based around taking the target width of an element and dividing it by the width of it’s parent element. The result is the relative width of the target element.

**target ÷ context = result**