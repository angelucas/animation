# animation CSS

## Third part
Here we go! Let's start with the magic of Animations.
Now we'll define a animation name, animation duration and animation fill mode to our "#showcase h1"
```css
#showcase h1 {
    animation: heading;
    animation-duration: 3s;
    animation-fill-mode: forwards;
}
```
Set the @keyframes to animation heading from our h1 title.
Where it's starts and it ends
```css
@keyframes heading {
    0% {top: -50px}
    100% {top: 200px}
}
```
Now we're going to set the animation atributes to the main content.
```css
#content {
    animation-name: content;
    animation-duration: 3s;
    animation-fill-mode: forwards;
}
```
And the same here, where it's starts and ends.
```css
@keyframes content {
    0%   {left: -1000px}
    100% {left: 0;}
}
```
The last element is the button.
We'll set opacity zero to the magic happens, animation name, duration, delay and fill mode.
And here we'll use a transition transform too.
```css
.btn {
    opacity: 0;
    animation-name: btn;
    animation-duration: 3s;
    animation-delay: 3s;
    animation-fill-mode: forwards;

    transition-property: transform;
    transition-duration: 1s;
}
```
The transform on the hover that we're going to use is rotate de Y axis 180 degrees.
```css
.btn:hover {
    transform: rotateY(180deg);
}
```
The animation @keyframes for the button that we'll use is the opacity 0 to 1. Making it appers from nothing.
```css
@keyframes btn {
    0%   {opacity: 0}
    100% {opacity: 1;}
}
```
### Well done ;)
### Hope it could be usefull to somebody. 

# Usefull links
- animate.css - https://daneden.github.io/animate.css/
