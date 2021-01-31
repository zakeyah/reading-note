# CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

##  A CSS rule contains two parts: a selector and a declaration.

### Selectors indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.

### Declarations indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon

## CSS declarations sit inside curly brackets and each is made up of two parts: a property and a valu

![](https://www.w3schools.com/css/selector.gif)
### There are three options for styling HTML elements. You can style HTML elements by using :

- using inline css
-  using InternaL css
-  using externaL css

## cSS SeLectorS
- unIverSaL SeLector   *{}
- type SeLector    h1, h2, h3 {} 
- cLaSS SeLector    .note {} 
- Id SeLector    # {} 
- chILd SeLector li>a {} 
- deScendant SeLector p a {} 
- adjacent SIBLIng SeLector h1+p {} 
- generaL SIBLIng SeLector h1~p {} 


# Color
### The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:
- rgb values 
- hex Codes 
- Color names 

## understanding Color
#### Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.
#### understanding Color Computer monitors are made up of thousands of tiny squares called pixels (if you look very closely at your monitor you should be able to see them).

# understanding Color

- rgb values (Values for red, green, and blue are expressed as numbers between 0 and 255. )
- hex Codes (Hex values represent values for red, green, and blue in hexadecimal code.)
- Color names (olors are represented by predefined names. However, they are very limited in number.)
- Hue (Hue is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue.)
- satuRatioN (Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray.)
- BRiGHtNess (Brightness (or "value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the color would be very dark)

## Contrast
### css3  opacity 
#### CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).


### Css3: hsl Colors
#### CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values

### Css3: hsl & hsla
The hsl color property has been introduced in CSS3 as an alternative way to specify colors. The value of the property starts with the letters hsl, followed by individual values inside parentheses for:
hue This is expressed as an angle (between 0 and 360 degrees).
saturation This is expressed as a percentage.
lightness This is expressed as a percentage with 0% being white, 50% being normal, and 100% being black.
The hsla color property allows you to specify color properties using hue, saturation, and lightness as above, and adds a fourth value which represents transparency (just like the rgba property). The a stands for:
alpha This is expressed as a number between 0 and 1.0. For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency






