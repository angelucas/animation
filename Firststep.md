# animation
Example of CSS animation:

This example is very simple and it will be usefull to exercising the criativity for future CSS animations.
It's a title, introduction text and button animation.

# Structure
### animation
- index.html
- css
  - landing.css
## HTML
This is the html body that we're going to use for this example.
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
        <a href="javascript:history.go(0)" class="btn">Read More</a>
    </body>
</html>
```
# CSS
## First
We're going to reset the all margins and paddings. Add a font, background-color, text-color, line-height and text-align to center.
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
```
We're going to define the attributes to the class called "container" that we have already created, with the max-width that we want, margin and padding.
```css
.container {
    max-width: 960px;
    margin: auto;
    padding: 0 30px;
}
```
## Second part
Now, we're gonna to set the height to our "showcase" ID from the main content.
```css
#showcase {
    height: 300px;
}
```
Add some attributes to our "h1 title".
```css
#showcase h1 {
    font-size: 50px;
    line-height: 1.3;
    position: relative;
}
```
Set ID="content" to "relative".
```css
#content {
    position: relative;
}
```
And set some nice attributes to let our button with a better look.
```css
.btn {
    display: inline-block;
    color: #fff;
    text-decoration: none;
    padding: 1rem 2rem;
    border: #fff 1px solid;
    margin-top: 40px;
}
```
