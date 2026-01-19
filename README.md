# imgd-5010-s26-assignment1.binary.md
# Simple Binary For Creating Radially Symmetric Rangoli
In Tamil Nadu, the southern most state of India on Jan 14 the holiday of Pongal is celebrated. This is a harvest festival which often includes the creation of radially symettric art made from different vibrantly colored powders.
![Simple Rangoli](https://i.pinimg.com/736x/8a/f9/e0/8af9e05e9b38a5f1943f57414b79a639.jpg)

A set of 4 bit words can be used to create simple rangoli
```
## Binary words
0 0000 - blank
1 0001 - circle/dot
2 0010 - round petal
3 0011 - pointed leaf
4 0100 - line
5 0101 - spiral
6 0110 - reserved
7 0111 - reserved
8 1000 - reserved
9 1001 - offset clockwise
10 1010 - outline
11 1011 - pattern
12 1100- reserved
13 1101 - move radially out
14 1110- color wheel clockwise
15 1111 - color wheel counter-clockwise
```
## Code Syntax
The code is read from left to right. Each code starts at a radius of 0, then using 13 the code moves outwards a single level. 
 For each level the user can enter a symbol.
After the symbol, the color is defined. This is done by moving clockwise along the color wheel starting at 90 deg/ 12 o'clock. Both color wheel clockwise and counter clockwise start with red. If no color is entered, the color white is used. 
If 10 is entered, the symbol is outlined in white. Color can be applied again to change the color of the outline from white to something else.
### Color Wheel
![Color Wheel](https://www.w3schools.com/colors/pic_rgb_wheel.gif)

Then enter the pattern word as many times as desired The symbols will be spaced equally apart starting at 90 deg/12 o'clock then moving clockwise. If no pattern is entered, a single instance of the symbol will be placed. 
If multiple symbols are on the same level they are evenly spaced out

symbol color outline color offset pattern radialout

## Example 1
![simple rangoli example](https://i.pinimg.com/736x/2c/45/46/2c454627104d642313a41a1664c8bf66.jpg)
```
0001(circle) 1110 1110 (orange) 1101 (radial out)
0001(circle) 1110 1110 1110 (yellow) 1101 (radial out)
0010 (round petal) 1110 1110 (orange) 1011  1011  1011  1011  1011  1011  1011  1011  1011  1011  1011  1011 (pattern 12 times) 1101 (radial out)
0010 (round petal) 1111  1111  1111  1111  1111  1111 (light blue) 1010 (white outline) 1011 1011 1011 1011 1011 1011 1011 1011 (pattern 8 times) 1101 (radial out)
0011 (pointed leaf) 1111 1111 1111 1111 1111 (blue) 1010 (white outline) 1011 1011 1011 1011 1011 1011 1011 1011 (pattern 8 times) 1101 (radial out)
0011 (pointed leaf) 1110  1110  1110  1110  1110 (green) 1010 (white outline) 1001 (offset) 1011 1011 1011 1011 1011 1011 1011 1011 (pattern 8 times)
```
