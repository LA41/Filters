# Filters
#Filters is a exercise written in C for CS50 Introduction to Computer Science. This is a little part of program previously written by people of CS50. This part is able to filter pictures in one of four possible ways: you can use grayscale, sepia, blur or reflection.

CS50 helped me understandv that filtering a picture is actually modifying a pixel in a particular way. For example - while working with grayscale I had to find average value of red, green and blue in each pixel, so that pixel got closer to black when mentioned values were low, or closer to white when values were high.
Sepia filter uses special formula on originally given values and then returns them in reddish-brown old-style look.
To do reflection I had to swap pixels, so that first in each row became last, second became last - 1 and so on. To do that I used temp variable.

Definitely the biggest challenge was blur effect. Firstly I created a copy of an image. Then I loop through each pixel and find its neighbours (also disregard pixels that are outside of the image). After that I need to sum value of neighbouring pixels in order to calculate the values red, green and blue in each pixel. The final value is being rounded to an integer. Last but not least - I copy new pixels into the image.

