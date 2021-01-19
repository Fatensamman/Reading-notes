# CSS Transforms, Transitions, and Animations
##  CSS Transforms
- With CSS3 came new ways to position and alter elements. All of these new techniques are made possible by the transform property. The transform property comes in two different settings, two-dimensional and three-dimensional. In this lesson we'll take a look at both two- dimensional and 3-dimensional transforms. We'll also look at how to use the transforms in Chrome's nightly version to see them in action.

- Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transform work on both the x, y and z axes, as well as the z axis. The rotate value provides the ability to rotate an element from 0 to 360 degrees. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how to change this default point.

- The translate value works a bit like that of relative positioning. It can be used to push and pull an element in different directions without interrupting the normal flow of the document. To set both the x and y axis values at once, declare the x axis value first, followed by a comma, and then the y axis value.

- Skew is used to distort elements on the horizontal axis, vertical axis, or both. Distance calculation of the skew value is measured in units of degrees. Length measurements, such as pixels or percentages, do not apply here. The syntax is very similar to that of the scale and translate values.

- Multiple transforms can be combined together. List the transform values within the transform property one after the other without the use of commas. Using multiple transform declarations will not work, as each declaration will overwrite the one above it.

- In order for three-dimensional transforms to work the elements need a perspective from which to transform. The perspective of an element can be set in two different ways. One way includes using the perspective value within the transform property on individual elements. The other is to use the perspective property on the parent element residing over child elements being transformed.

-3D Transforms allows us to change elements on the z axis. The z axis gives us control of depth as well as length and width. We use three new transform values, including rotateX, rotateY, and rotateZ. The rotateX value allows you to rotate an element around the x axis, as if it were being bent in half horizontally, while the rotateY value allows the element to be rotated around the y axis. negative values will rotate the element counterclockwise.

![transform](https://tipsmake.com/data/images/3d-transform-in-css-picture-1-jtznOkrOW.jpg)

##  CSS Transitions & Animations:

- With CSS3 you can design interactions between elements and each other within HTML and CSS. Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. For a transition to take place, an element must have a change in state, and different styles must be identified for each state. In the example below the background color will change its background color over the course of 1 second in a linear fashion. The ability to write behaviors for transitions and animations has been a long-requested feature of CSS3.
![transition](https://miro.medium.com/max/900/1*_6MfwckxNfQTca9SiG8MdQ.png)

## 8 simple CSS3 transitions:
- 1. Fade in
- 2. Change color
- 3. Grow & Shrink
- 4. Rotate elements
- 5. Square to circle
- 6. 3D shadow
- 7. Swing
- 8. Inset border
![transition](https://www.css3transition.com/wp-content/uploads/2017/10/Bounce-text-animation.gif)