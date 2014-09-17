---
tags: html, css, kids, todo
languages: html, css
type: to-do
level: 2
---

##Getting Jiggy With It


Let's make a box dance with CSS animations!!

You'll want to open up `index.html` in the browser. You should see a red box on the screen.

You'll code your solution in `style.css` The CSS selector that we use is the most important part about animations. 

###@keyframes
We're going to use `@keyframes` rule which takes a custom animation name as an argument. `@keyframes` sets stages in a timeline for your animation in percentages.

In `style.css`, it should look something like this

```CSS
@keyframes CUSTOM-NAME-FOR-ANIMATION{
  0% {}
  25%{}
  75%{}
  100%{}
}

```
###Vendor Prefixes
It's important to remember vendor prefixes here. Not all animations are supported by every browser, and in order to make the animations work for every browser, you'll have to declare which browser you're using.

Chrome:
```CSS
@-webkit-keyframes CUSTOM-NAME-FOR-ANIMATION{
```
}
```
Firefox:
```CSS
@-moz-keyframes CUSTOM-NAME-FOR-ANIMATION{
```
}
Opera:
```CSS
@-o-keyframes CUSTOM-NAME-FOR-ANIMATION{

}
```

###Dancing Rules
You're going to want to change the width and height properties during your animation.

0% is the starting point, so you'll want your box to start at 100px wide and 100px tall.

25% you'll want your box to change to 300px tall and 100px wide

50% you'll want your box is change to 100px tall and 300px wide

75% you'll want to change your box to 500px tall and 100px wide

100% you'll want to set your box back to 100px tall and 100px wide

###Calling The Animation
Now we actually need to call the animation. You'll want to add to the already written CSS for the id redbox. By using something like this:
```CSS
  -webkit-animation: NAME-YOUR-ANIMATION 5s infinite; /* Safari 4+ */
  -moz-animation:    NAME-YOUR-ANIMATION 5s infinite; /* Fx 5+ */
  -o-animation:      NAME-YOUR-ANIMATION 5s infinite; /* Opera 12+ */
  animation:         NAME-YOUR-ANIMATION 5s infinite; /* IE 10+, Fx 29+ */
```
The `5s` is the duration of one single animation in seconds. The `infinite` tells the animation to repeat in an infinite loop.

The animations should start as soon as your page loads without clicking anything or hovering over anything.

