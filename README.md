IDEA:
- Get user to input 16 bits (1 or 0).
- Store all of them to an array (start in p3, go to p5, etc. to account for parity bit locations)
   - Store all values individually instead? (could be clunky)
- Write an XOR program to determine if the parity bit is 0 or 1, then add it to the base value.
   - ex: if the input is 150, a parity bit at position 4 (2^2) is 150 + 4
   - looks something like: getP1, load data 
     subt X2
     skipcond 400 (if they are both 1 then it'll be zero, else, it'll pass)
     ... handle that (WHAT SHOULD HAPPEN IS THAT IT SKIPS TO THE NEXT FUNCTION IF ONE OF THE VALUES IS THE SAME)
     Load X2
     Subt X3
     skipcond 400
     .. same thing until all positions have been handled
   - if all true, add number
   - if false, it won't add anything cause it will skip
- Display final number (what we send)
