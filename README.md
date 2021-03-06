# Weekly nerd
I have learned a lot during the minor web development, some things from working with JavaScript mot most from working with HTML and CSS. Because I study software engineering and I already knew some things about coding I have chosen to focus this minor more on the creative classes. For this reason I want to write three articles about things I found most interesting of the things I have learned during this minor.

## Article 1: Display attribute
### Display block
The display attribute is a very handy CSS tool you can use to modify the behavior of an element. Most of the common elements are a block element which means they have the same width as their parent width, and appear as a list under each other with their siblings. Some examples of common block elements are: main, article, section, div, h1 and p.

![Display block](img/display-block.png)  
Figure 1: Three block elements under each other.

### Display inline
There are some exceptions, some elements are not block elements, these are inline elements. This means that they are not 100% of their parent width and appear next to each other. Some examples of common inline elements are: a, span, image, input, script and button.

![Display inline](img/display-inline.png)  
Figure 2: Three inline elements next to each other.

Pro tip: You can also use the "display:inline-block" attribute, this is a combination between a block element and a inline element. It uses most of the properties of an inline element but can just like a block element you can change the height and width property of the element.

### Display none
The last classic display property that I have used during this course is the display none. Display none is pretty simple, it removes an element from the page completely like it did not exist at all. I used this a lot for switching between pages when a user presses a button. Be warned using display none uses a lot of resources from your browser because it has to redrawn the entire page, as you can see in figure 1 and figure 3, the next elements after the removed element are moved upwards to the spot of the removed element.

![Display none](img/display-none.png)  
Figure 3: The second block element is missing and the page has been redrawn.

Pro tip: if you can effort it, it can sometimes better to use opacity: 0, because as you can see in figure 4, the entire page does not have to be redrawn. Opacity also works fantastic with transitions so you can do some cool things with it.

![opacity](img/opacity.png)  
Figure 3: The second block element is missing again however now the page has not been redrawn.

### Display flex
Over the years new display properties have appeared, these properties are not standard bound to some elements, but just as with display none, you have to assign this property to an element yourself. One of these properties is the flexbox property, a flexbox is a very cool property because it is initially a block element. However, it changes the behavior of its children so that they are all inline. Then you can customize the children even further with other flexbox properties, you can center or put the children on the right side of the screen, you can even play with the space between the elements to create something great. With "flex-wrap: wrap" It is also possible to break the children if the child elements are bigger than your flexbox container (or your screen), this is cool because with this it is much easier to make parts of your website responsive.

![flex](img/flexbox.PNG)  
Figure 4: Three flexboxes, one regular, the second one with flex-wrap and the last one with its space between evenly divided.

In figure four, I made three flexboxes, the first one is a regular flexbox with its children next to each other with a some of its children outside of the parent container. The second flexbox has the property "flex-wrap: wrap" so its children are positioned nicely after the screen is too small. The last flexbox has fewer children and has the property "justify-content:space-evenly", this means that its children are kinda centered because all the space between the children and the parent are perfectly evenly divided.

### Display grid
The last display property I would like to discuss is the grid, you can almost compare a grid with a flexbox, except that it is 2 dimensional instead of 1 dimensional and you can declare a grid with the "display:grid" property. A grid has rows and columns, rows are the vertical children and columns are the horizontal children. A grid is really handy in my opinion because you can design your entire website with one big grid and if you need to swap children around you can use "grid-column-start" and "grid-row-start" to flip the designs of you website around.

![grid](img/grid.png)  
Figure 5: Something you can do with a grid, it could be used as the skeleton for a website.

### Conclusion
The display attribute is very handy, I would use grids as your website base or to center stuff instead of using a flexbox, because you can do so many more things with it. However, grids and flexboxes only work with modern browsers. So try to work on a fallback with both block and inline elements. It does not have to be something fancy, only functional in my opinion.

### Sources
https://www.w3schools.com/html/html_blocks.asp
https://developer.mozilla.org/en-US/docs/Web/CSS/display
https://www.w3schools.com/css/css_inline-block.asp
https://css-tricks.com/snippets/css/a-guide-to-flexbox/
https://css-tricks.com/snippets/css/complete-guide-grid/
https://caniuse.com/

## Article 2: Position atribute
### Position static
The second thing I would like to discuss is the position attribute, with the position attribute you can do some cool things. You can use this attribute to move elements from their original position, or align an element to the top, right, bottom, left and stick an element to the view port. First of all I want to talk about the static position. The static position is a position that every element standard has. So this means that all elements are a static element so there is nothing special.

![Position static](img/static.png)  
Figure 6: Position static, also known as the regular element.

### Position relative
An element with position relative property is exactly the same as a static element, except that it reacts to the "top", "left", "bottom" and "right" properties. Each of these properties moves the element away from the selected property, so "top:1px" moves the element downwards by 1px.

![Position relative](img/relative.PNG)  
Figure 6: The child element is moved 10 px to the left with the right property.

### Position absolute
My favorite position, I used to use a grid for this but since I have learned about it I never stopped using it. An absolute element sticks to the first parent it can find with another position that static, then with the "top", "left", "bottom" and "right" properties the absolute element sticks to the parent side of the selected property. So "left:0" sticks the child element on the right side. This is not everything you can do, you can even increase the pixels so that it moves away from the parent side with that around of pixels. This means you can do very cool things with it. What I like to do is making a parent element relative, and not changing the "top", "left", "bottom" and "right" properties. Then I can make one of its child elements absolute and apply the "bottom: 0; right:0" properties to it. Now you have a child element that has something in the bottom right of the parent element you could add something like an icon.

![Position absolute](img/absolute.png)  
Figure 7: Some amazing things you can do with the absolute property.

### Position fixed
Position fixed works kinda the same a position absolute, there is one difference though, a fixed element does not stick to the first relative element but to the view port. This means you can make some cool things like a alert box or add a logo in the bottom left of the screen. This also means that if you scroll the element that is position fixed stayed in place because it is fixed to the view port.

![Position fixed](img/fixed.png)  
Figure 8: The child element is fixed to the viewport with position fixed.

### Position sticky
Lastly you also have position sticky, position sticky is a combination between position fixed and position relative. It starts as a normal element, but if you scroll past it, it sticks to the view port like a fixed element. This can be cool for things like menus.

### Conclusion
With the position attributes you can do a lot of cool things. You can change the default HTML behavior completely. I would use position absolute to reposition elements in their container, like buttons or so. And I would use position fixed and sticky for menus and instead of alert messages.

### Sources
https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning

## Article 3: CSS selectors
The last thing that I want to discuss are some CSS selectors. CSS selectors are pretty cool, before this minor I had some experience wit JQuery, I used classes where ever I could. But during the CSS to the rescue course I learned that you do not need those CSS classes, and can do a lot with only CSS selectors which I will soon tell you more about. During the master course I started working with components. This way I learned that if you split of your HTML, CSS and JavaScript in several components, you can give an id to that component, then you can use CSS selectors to the children of that component with the id to keep a clean CSS file.

### element&gt;element
With this selector it is possible to select all the children of a specific element inside a parent. I think this is quite useful because you can be really specific what element you want to select without ugly CSS classes in combination with

### :nth-child()
:nth-child() is a handy selector, you can use it to select one of the children of a parent. First you have to select an element, in figure 9 you can see that we have selected a div element. Then we need to declare the number of the child. So in this case we need the second child so the CSS would look like this: "div:nth-child(2)". You could even be more specific by targeting the ID of the component and the parent element like this: "#component&gt;article&gt;div:nth-child(2)".

![:nth-child()](img/nth-child.png)  
Figure 9: the second child is selected with div:nth-child(2).

### :nth-of-type()
:nth-of-type() is something new I just learned today. It looks a lot like nth-child, but there is one difference. "div:nth-of-type(2)" selects the second div in the parent regarded of its position. "div:nth-child(2)" also selects the second div but only if the second child of a parent is a div element. This is handy because you can add a complete different child element to a parent later without destroying your CSS. It has to be another element or else it would not work.

![:nth-of-type()](https://i0.wp.com/css-tricks.com/wp-content/csstricks-uploads/relationalpseudos2.png?resize=570%2C541)  
Figure 10: An example of :nth-of-type() and :nth-child() (css-tricks.com)

### Conclusion
I like CSS selectors a lot. I have learned so much this semester and these CSS selectors with components makes my HTML and CSS so readable for me. I would give each component an id and target all the items inside of that component with semantic HTML and if necessary with :nth-of-type().

### Sources
https://css-tricks.com/pseudo-class-selectors/
https://www.w3schools.com/cssref/css_selectors.asp
