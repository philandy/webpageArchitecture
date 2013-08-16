# Character Sets
This document contains proposals for character sets, addresses this repository's development of character sets, and lists some popular character sets.

## Proposals

### "Bicontrol"
I propose using a binary set of codes to control character sets, meaning 2 codes to control the rest of the codes.

For example, 8-bit bicontrol would use 2 of the 256 codes as control codes, and leave the rest alone. 00 would be one, and FF would be the other. These 2 codes would allow nesting, essentially allowing an infinite amount of control with only 1/128 loss.

### "Monocontrol"
I propose using a single code to control character sets.

For example, 8-bit monocontrol would use 1 of the 256 codes as a control code, and leave the rest alone. It should be FF. This would allow for creativity to surround the code to create whatever is needed. As an 8-bit code, it would have 1/256 loss.

### "The Rest"
While discussing control codes, the actual "content" codes have not been described. This should boil down to interfacing, meaning they can be whatever one wishes them to be. A default standard should be included in the final solution for the webpage architecture project.

### "Less Bits"
English uses 26 letters, so each can be represented by limiting to a range of 2^5 (or 32) codes. This gives room for a few symbol codes plus the control code. This could be useful for small alphabet languages (such as Rotokas which uses 12 letters).

### "More Bits"
Due to higher amount of bits reducing loss of value, potentially any amount of bits could be used to represent content, plus the control code. For example, aligning to 32 bits would give you only 1/(2^32) loss (but you would have to find useful unique values for 2^32 codes!)

## Development

### n/a
Nothing has been developed at this time.

## Some popular character sets are
* UTF
* ASCII
* ANSI
