Challenges

shredded

This Challenge presented you with 27 .png files some of which contained horizontal slices of a QR-Code and 6 slices that were completely white, thus not belonging to the QR-Code.

IMAGE HERE

The natural first thing to do was throwing all the pieces into gimp and try to rearrange them to get a valid QR-Code. Some shadows on the front and backside of the horizontal bars of the Finder Pattern made it possible to determine the exact position of some of the slices. What i realized very early on in the research is that the position of many of the slices is not uniquely identifiable. This is bad, because all of the QR-Code readers didn't report which decoding step failed but rather did not recognize the QR-Code at all. So now we know there might be some bruteforcing involved. As of now we have placed 9 of 21 tiles by only ensuring valid finder patterns.

IMAGE HERE

This leaves us with (21-9)! = 12! options to arrange the remaining slices... Thats a total of 479001600 combinations. Lets see if we can get this number down to more reasonable values. First of all, for our 12! approach we are also trying to match patterns to spot where they dont make sense. For example the slices belonging to the middle of the finder pattern can be identified, but their order can not, for the empty spaces 3,4 and 5 we have only 3 .png files that can fill the slots according to QR Specification, same holds for slices

IMAGE HERE

