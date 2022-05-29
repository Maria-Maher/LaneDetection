# LaneDetection
Steps of the project:
   
   1-Apply a perspective transform to rectify binary image ("birds-eye view").
   2-Use color transforms, gradients, etc., to create a thresholded binary image.
   3-Detect lane pixels and fit to find the lane boundary.
   4-Determine the curvature of the lane and vehicle position with respect to center.
   5-Warp the detected lane boundaries back onto the original image.
   6-Output visual display of the lane boundaries and numerical estimation of lane curvature and vehicle position.


when we use prespective transformation a bird eye view is applyed by using a function cv2.getPrespectiveTransform(), then it convert the picture from front view to top view to extract lane features, and it turns it back to front view.

![image](https://user-images.githubusercontent.com/106494037/170893480-4295097a-a660-44cc-bac8-8480f12bae81.png)


 we can extract features and find lane pixels from a binary wraped image, and by using a function called fit_poly() it can find the lanes and draw it and returns the RGB image that have lane line drawn on that.

