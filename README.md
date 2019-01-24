# Finding-Lane-Lines-P1_KPIT-Udacity-Self-Driving-Car
Finding Lane Lines on the Road

The goals / steps of this project are the following:

Make a pipeline that finds lane lines on the road
Reflect on your work in a written report

Reflection
1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.
My pipeline consisted of 5 steps. 
    1. Image to grayscale
    2. grayscale to gaussian blur
    3. applied canny on gaussian blur to get edges
    4. filled a quadrilateral portion of image and got masked image 
    5. detected the lines using hough transformation
    6. put the lines i got on original image using weighted_img

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by changing the thickness and varying other parameters


2. Identify potential shortcomings with your current pipeline

One potential shortcoming would be that id doesnt work well on challenging problem

Another shortcoming is that the lines dont remain much stable.

3. Suggest possible improvements to your pipeline
A possible improvement would be to make the lines even more stabilise.

Another potential improvement could be to fill color between the lane lines
