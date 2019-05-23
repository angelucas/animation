# animation
Example of CSS animation:

This example is very simple and it will be usefull to exercising the criativity for future CSS animations.
It's a title, introduction text and button animation.

# Structure
### animation
- index.html
- css
  - landing.css
#### HTML
```html
<!DOCTYPE html>
<html lang="pt-br">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <meta http-equiv="X-UA-Compatible" content="ie=edge">
        <link rel="stylesheet" href="css/landing.css">
        <title>Animation</title>
    </head>
    <body>
        <header id="showcase">
            <h1>My Web Page</h1>
        </header>
        <div id="content" class="container">
            Lorem ipsum dolor sit amet consectetur, adipisicing elit.
            Mollitia assumenda, debitis ex quisquam veritatis voluptas harum vero
            perspiciatis sunt ad ullam nemo ipsum accusamus! Rem similique repellat labore 
            possimus repellendus.
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto ipsa, earum odit quos, 
            excepturi voluptates dolorem, expedita sequi minus fugiat voluptatibus impedit. 
            Voluptas, eveniet placeat facilis optio nisi culpa corporis!
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Recusandae totam laboriosam aut? Laboriosam impedit cum non earum numquam beatae, 
            maiores quod eaque placeat reprehenderit nesciunt illo voluptas vitae ut harum?
        </div>
        <a href="javascript:history.go(0)" class="btn">README</a>
    </body>
</html>
```
### CSS
```css
* {
    margin: 0;
    padding: 0;
}
body {
    font-family: Arial, Helvetica, sans-serif;
    background-color: #12475f;
    color: #fff;
    line-height: 1.6;
    text-align: center;
}
.container {
    max-width: 960px;
    margin: auto;
    padding: 0 30px;
}
#showcase {
    height: 300px;
}
#showcase h1 {
    font-size: 50px;
    line-height: 1.3;
    position: relative;
    animation: heading;
    animation-duration: 3s;
    animation-fill-mode: forwards;
}
@keyframes heading {
    0% {top: -50px}
    100% {top: 200px}
}
#content {
    position: relative;
    animation-name: content;
    animation-duration: 3s;
    animation-fill-mode: forwards;
}
@keyframes content {
    0%   {left: -1000px}
    100% {left: 0;}
}
.btn {
    display: inline-block;
    color: #fff;
    text-decoration: none;
    padding: 1rem 2rem;
    border: #fff 1px solid;
    margin-top: 40px;
    opacity: 0;
    animation-name: btn;
    animation-duration: 3s;
    animation-delay: 3s;
    animation-fill-mode: forwards;

    transition-property: transform;
    transition-duration: 1s;
}
.btn:hover {
    transition: rotateY(180deg);
}
@keyframes btn {
    0%   {opacity: 0}
    100% {opacity: 1;}
}
```

# Usefull links
- animate.css - https://daneden.github.io/animate.css/
