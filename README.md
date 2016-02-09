Tool to create high resolution ascii art.

Usage: python ascii.py <image filename> <horizontal resolution>

If horizontal resolution is not specified, it defaults to the smallest of 400 and the original image horizontal resolution.

The image is downsampled, and each pixel is replaced with the printable character closest in brightness to the original pixel, after normalization. Character brightnesses were previously calculated by, for each character, producing an image containing only that character and calculating the mean pixel brightness.




