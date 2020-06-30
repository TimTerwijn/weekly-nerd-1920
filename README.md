# Weekly nerd
I have learned a lot during the minor webdevelopment, some things from working with Javascript mot most from working with HTML and CSS. Because I study software enginering and I already knew some things about coding I have chosen to focus this minor more on the creative classes. for this reason I want to write three articles about things I found most intresting of the things I have learned during this minor.

## Display attribute
### Display block 
The display attribute is a very handy css tool you can use to moddify the behavour of an element. Most of the common elements are a block element which means they have the same width as their parent width, and apear as a list under eachother with their siblings. Some examples of common block elements are: main, article, section, div, h1 and p.  

![Display block](img/display-block.png)  
Figure 1: Display block

### Display inline
There are some exeptions, some elememts are not block elements, these are inline elements. This means that they are not 100% of their parent width and apear next to eachother. Some examples of common inline elements are: a, span, image, input, script and button.  

![Display inline](img/display-inline.png)  
Figure 2: Display inline

### Display none
The last classic display propety that I have used during this cource is the display none. Display none is pretty simple, it removes a element from the page compleetly like it did not existed at all. I used this a lot for switching between pages when a user presses a button. Be warned using display none uses a lot of resources from your browser because it has to redrawn the enteire page, as you can see in figure 1 and figure 3, the next elements after the removed element are moved upwards to the spot of the removed element. 

![Display none](img/display-none.png)  
Figure 3: Display none

If you can affort it, it can somethimes better to use opacity: 0, because as you can see in figure 4, the entire page does not have te be redrawn. Opacity also works fantastic with transitions so you can do some cool things with it.

![opacity](img/opacity.png)  
Figure 3: Opacity 0

### Display flex
Over the years new dipslay propeties have apreared, these propeties are not standard bound to some elements, but just as with display none, you have to assign this proppety to a element yourself. One of these propeties is the flexbox propety, a flexbox is a verry cool propety because it is initialy a block element. However, it changes the behaviour of its children so that they are all inline. Then you can customize the children even further with other flexbox propeties, you can center or put the children on the right side of the screen, you can even play with the space between the elements to create some thing great. With "flex-wrap: wrap" It is also possible to break the children if the child elements are bigger than your flexbox container (or your screen), this is cool because with this it is much easier to make parts of your website responseable.

![flex](img/flexbox.PNG)  
Figure 4: Flexbox 0

In figure four, I made three flexboxes, the first one is a regular flexbox with its children next to eachother with a some of its chilldren outside of the parent container. The second flexbox has the propety "flex-wrap: wrap" so its children are possisioned nicely after the screen is too small. The last flexbox has fewer children and has the propety "justify-content:space-evenly", this means that its children are kinda centred because all the space between the children and the parend are perfectly evenly devided.

### Display grid
The last display propety I would like to discuss is the 


### Sources
https://www.w3schools.com/html/html_blocks.asp
https://developer.mozilla.org/en-US/docs/Web/CSS/display



## Position atribute

## Components
