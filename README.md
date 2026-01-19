# imgd-5010-s26-assignment1.binary.md
# Simple Binary For Creating Radially Symmetric Rangoli
In Tamil Nadu, the southern most state of India on Jan 14 the holiday of Pongal is celebrated. This is a harvest festival which often includes the creation of radially symettric art made from different vibrantly colored powders
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
9 1001 - reserved
10 1010 - white outline
11 1011 - pattern
12 1100- move radially in
13 1101 - move radially out
14 1110- color wheel clockwise
15 1111 - color wheel counter clockwise
```
## Code Syntax
The code is read from left to right. Each code starts at a radius of 0, then using 13 the code moves outwards a single level. 
 For each level the user can enter a symbol.
After the symbol, the color is defined. This is done by moving clockwise along the color wheel starting at 90 deg/ 12 o'clock. If no color is entered, the color white is used. 
If 10 is entered, the symbol is outlined in white
### Color Wheel
![Color Wheel](https://www.w3schools.com/colors/pic_rgb_wheel.gif)
Then enter the pattern word as many times as desired The symbols will be spaced equally apart starting at 90 deg/12 o'clock then moving clockwise. If no pattern is entered, a single instance of the symbol will be placed. 
If multiple symbols are on the same level they are evenly spaced out

## Example 1



```
