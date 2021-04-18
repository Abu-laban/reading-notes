# Colors in CSS
** Color can really bring your pages to life. **

* Foreground Color

*The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:*

1. rgb values

2. hex codes

3. color names

* Background Color

*CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.*

## Understanding Color

> Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.

## Contrast
> When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.

**CSS3** has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA. also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.

* The hsl color property has been introduced in CSS3 as an alternative way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for:

> background-color: hsl(0,0%,78%)

1. hue
This is expressed as an angle (between 0 and 360 degrees).
2. saturation
This is expressed as a percentage.
3. lightness
This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black.

The hsla color property allows you to specify color properties using hue, saturation, and lightness as above, and adds a fourth value which represents transparency (just like the rgba property). The a stands for:

**alpha**

This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency.