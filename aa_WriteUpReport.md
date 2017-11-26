
# **Finding Lane Lines on the Road** 

## Writeup 

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 4 steps. 

First, I converted the images to grayscale and applied Gaussian Blur with kernel size of 5.

Second, I found the edges using Canny method with (low threshold, high threshold) = (50, 150).

Third, I drew a four-sided polygon mask, and applied it to the image.

Finally, I applied Hough transform and draw lines.


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when there is sharp turn, for example, in the challenge video.


### 3. Suggest possible improvements to your pipeline

Possible improvement to address the sharp turn issue involves more adaptive way for mask definition.
