# 4 ways to center a div using CSS

### **What is A div?**

A div is a block-level element that can contain other elements such as text, images, links, etc. It is often used to create sections or layouts on a web page. Sometimes, you may want to center a div using CSS to make it look more appealing or balanced. In this blog, I will show you four ways to center a div horizontally and vertically using CSS:

1. **CSS positioning using *margin:auto***  
    To center a div horizontally and vertically using CSS positioning, set its position property to absolute so that it is removed from the normal document flow and positioned relative to its parent div, body. or viewport. 

    After that, to stretch it across the entire width of its parent element or viewport, set its left and right properties to 0. Then set its top and bottom properties to 0 so that it’s stretched across the entire height of its parent element or viewport. 

     Finally, use the margin property with an auto value on all sides to center it within its parent element or viewport.

    Code example:
    ```
     div {
       position: absolute; 
       left:0;
       right:0;
       top:0;
       bottom:0;
       margin:auto; /* centers the div */
      }
    ```

    Let’s check it out in the Codepen:
    {% codepen src="https://codepen.io/muzhcode/pen/ExeXwVw" /%} 
 
2. **CSS positioning using *transform property***  
    To center a div using transform property, first set its position property to absolute or fixed. Then set its top and left properties to 50% so it moves down and right by half of its own height and width plus half of its parent’s height and width, respectively, from its normal position. 

    Finally, to make it in the exact center position of the parent element or viewport set a -50% value to the transform property.
    
    For example:
    ```
         div {
             position: absolute; 
             left:0;
             right:0;
             top:0;
             bottom:0;
             margin:auto; /* centers the div */
        }
    ```
    
    Let’s check it out in the Codepen:
    {% codepen 
src="https://codepen.io/muzhcode/pen/ZEMyJZO" /%}  
<br> 

3. **CSS Flexbox**  
    Flexbox is a powerful one-dimensional layout model that will help you create responsive elements within a container. 
    
    To center a div using CSS flexbox, set the parent div a display property of flex, so it becomes a flex container that can contain other elements as flex items. Then set a value of center to justify-content to center horizontally all the elements inside the parent div. Finally, set a value of center to align-items as well, to center vertically all the elements inside the parent div. 
    
    Code for it:
    ```
      div {
         display: flex; 
         justify-content: center; /* center div horizontally */
         align-items:center;  /* center div vertically */
       }
    ```
    
    Let’s check it out in the Codepen:
    {% codepen src="https://codepen.io/muzhcode/pen/abawyRW" /%} 

    
4. **CSS Gird**  
    CSS grid is a powerful two-dimensional layout model that will help you create complex responsive web design layouts.
    
    To center a div using the CSS grid, set the parent’s div as a display property of the grid so that it becomes a grid container that can contain other elements as grid items. Then you can use a place-items which is a shorthand property for align-items and justify-items that will center the grid items (div) vertically and horizontally.  
    
      Code for it:
    ```
       div {
	       display: grid;
	       align-items: center;
	       place-items: center; 
         }
    ```

    Let’s check it out in the Codepen:
     {% codepen src="https://codepen.io/muzhcode/pen/WNgOZGQ" /%}

In conclusion, there are multiple ways to center a div. The above methods have their own pros and cons depending on the specific use case. It is important to choose the method that best fits your needs.

I would love to hear about other ways you might have found of centering a div. Please feel free to share them in the comments section.

If you have any questions or feedback, please leave them in the comments below as well.

I appreciate you taking the time to read this 😃!
 
