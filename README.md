# imgd-5010-s26-assignment1.binary.md
# Simple Binary For Creating Radially Symmetric Rangoli
In Tamil Nadu, the southern most state of India on Jan 14 the holiday of Pongal is celebrated. This is a harvest festival which often includes the creation of radially symettric art made from different vibrantly colored powders
```
## Binary words
1 - circle/dot
2 - round petal
3 - pointed leaf
4 - line
5 - reserved
6 - reserved
7 - reserved
8 - reserved
9 - reserved
10 - reserved
11 - white outline
12 - pattern
13 - move radially in
14 - move radially out
15 - color wheel clockwise
16 - color wheel counter clockwise
```
## Code Syntax
The code is read from left to right. Each code starts at a radius of 0, then using 13 the code moves outwards a single level. 
 For each level the user can enter a symbol.
After the symbol, the color is defined. This is done by moving clockwise along the color wheel starting at 90 deg/ 12 o'clock. If no color is entered, the color white is used. 
If 11 is entered, the symbol is outlined in white
### Color Wheel
![Color Wheel](https://www.w3schools.com/colors/pic_rgb_wheel.gif)
Then enter the pattern word as many times as desired The symbols will be spaced equally apart starting at 90 deg/12 o'clock then moving clockwise. If no pattern is entered, a single instance of the symbol will be placed. 
If multiple symbols are on the same level they are evenly spaced out





