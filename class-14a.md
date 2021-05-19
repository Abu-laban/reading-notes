# CSS Transforms, Transitions, and Animations

## Transforms

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the **transform property**.

The transform property comes in two different 
settings

1. two-dimensional.

2. three-dimensional.

Each of these come with their own individual properties and values.

### Transform Syntax

The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

        div {
        -webkit-transform: scale(1.5);
        -moz-transform: scale(1.5);
         -o-transform: scale(1.5);
          transform: scale(1.5);
    }

### 2D Transforms

Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.

* 2D Rotate

The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. 

HTML

        <figure class="box-1">Box 1</figure>

CSS

        .box-1 {
         transform: rotate(20deg);
        }

![rotate](https://uploads.sitepoint.com/wp-content/uploads/2018/09/1536069016TransformRotate.png)

* 2D Scale

Using the scale value within the transform property allows you to change the appeared size of an element.

HTML

        <figure class="box-1">Box 1</figure>

CSS

        .box-1 {
     transform: scale(.75);
    }

![scale](https://user.oc-static.com/upload/2019/01/29/15487607542807_pt02ch03_06_scale_v001.gif)

* 2D Translate

The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.

HTML

        <figure class="box-1">Box 1</figure>

CSS

        .box-1 {
     transform: translateX(-10px);
    }

![translate](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/translate()/translate.png)

* 2D Skew

The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both.

HTML

        <figure class="box-1">Box 1</figure>

CSS

        .box-1 {
    transform: skewX(5deg);
    }

![skew](https://1.bp.blogspot.com/-BFB3ZB18I0g/WE5kxxjky3I/AAAAAAAADkU/dxEMzStkSMQLnMX_J5RhgBBYJcc6rNNkwCLcB/s640/oISrXv4.gif)

### 3D Transforms

* 3D Rotate

With three-dimensional transforms we can rotate an element around any axes. To do so, we use three new transform values, including rotateX, rotateY, and rotateZ.

* 3D Scale

By using the scaleZ three-dimensional transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale.

* 3D Translate

Elements may also be translated on the z axis using the translateZ value. A negative value here will push an element further away on the z axis, resulting in a smaller element.

* 3D Skew

Skew is the one two-dimensional transform that cannot be transformed on a three-dimensional scale.

![3d](https://polypane.app/blogs/transforms/transforms.svg)

## Transitions & Animations

### Transitions

a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

### Transitional Properties

> It is important to note, **not all properties may be transitioned**

only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another. The display property, for example, may not be transitioned as it does not have any midpoint. A handful of the more popular transitional properties include the following.

background-color

background-position

border-color

border-width

border-spacing

bottom

clip

color

crop

font-size

font-weight

height

left

letter-spacing

line-height

margin

max-height

max-width

min-height

min-width

opacity

outline-color

outline-offset

outline-width

padding

right

text-indent

text-shadow

top

vertical-align

visibility

width

word-spacing

z-index

### Transition Duration

The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). 

### Transition Timing

The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the transition-timing-function property include linear, ease-in, ease-out, and ease-in-out.

### Transition Delay

On top of declaring the transition property, duration, and timing function, you can also set a delay with the transition-delay property. The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing. As with all other transition properties, to delay numerous transitions, each delay can be declared as comma separated values.

![transition](https://miro.medium.com/max/960/1*R2IxrEjMVm6QiRYdEo-lvQ.png)

## Animations

Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where **animations** pick up where transitions leave off.

### Animations Keyframes

To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

### Animation Name

Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.

### Animation Duration, Timing Function, & Delay

They include a duration, timing function, and delay if desired.

animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.

A timing function and delay can be declared using the animation-timing-function and animation-delay properties respectively. The values for these properties mimic and behave just as they do with transitions.

![animation](https://res.cloudinary.com/practicaldev/image/fetch/s--GZYZPBSr--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://res.cloudinary.com/practicaldev/image/fetch/s--HLCG8XKx--/c_imagga_scale%2Cf_auto%2Cfl_progressive%2Ch_720%2Cq_auto%2Cw_1280/https://dev-to-uploads.s3.amazonaws.com/i/54ydb37tzyny06ac8xdf.jpg)

## Customizing Animations

Animations also provide the ability to further customize an element’s behavior, including the ability to declare the number of times an animation runs, as well as the direction in which an animation completes.

### Animation Iteration

By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the animation-iteration-count property may be used. Values for the animation-iteration-count property include either an integer or the infinite keyword. Using an integer will repeat the animation as many times as specified, while the infinite keyword will repeat the animation indefinitely in a never ending fashion.

### Animation Direction

the direction an animation completes using the animation-direction property. Values for the animation-direction property include normal, reverse, alternate, and alternate-reverse.

### Animation Play State

The animation-play-state property allows an animation to be played or paused using the running and paused keyword values respectively. When you play a paused animation, it will resume running from its current state rather than starting from the very beginning again.

### Animation Fill Mode

The animation-fill-mode property identifies how an element should be styled either before, after, or before and after an animation is run. The animation-fill-mode property accepts four keyword values, including none, forwards, backwards, and both.
