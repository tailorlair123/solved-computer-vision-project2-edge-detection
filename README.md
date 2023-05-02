Download Link: https://assignmentchef.com/product/solved-computer-vision-project2-edge-detection
<br>
To practise edge detections

<ol>

 <li>Write edge detection routines for Sobel Edge, Prewitt Edge and Canny Edge operators.</li>

</ol>

                        

<ul>

 <li>Apply Sobel Kernel    <sub> </sub> and   <sub></sub> for Sobel Edges with a</li>

</ul>

                                   

reasonable threshold.

                                 

<ul>

 <li>Apply Prewitt Kernel   <sub></sub> and                <sub> </sub> for Prewitt Edges with a</li>

</ul>

                      

resonable threshold.

<ul>

 <li>Canny Edge Detector requires longer multiple steps discussed in class.

  <ol>

   <li>Create a 1D Gaussian mask G to convolve with your image (I). The standard deviations(s) of this Gaussian is a parameter to the edge detector (call it &gt;0).</li>

   <li>Create a 1D mask for the first derivative of the Gaussian in the x and y directions; call these G<sub>x</sub> and G<sub>y</sub>. The same &gt;0 value is used as in step a)</li>

   <li>Convolve your image I with G along the rows to give the x component image (I<sub>x</sub>) and down the columns to give the y component image (I<sub>y</sub>).</li>

   <li>Convolve I<sub>x</sub> with Gx to give I’<sub>x</sub>, the x component of I convolve with the derivative of the Gaussian, and convolve I<sub>y</sub> with G<sub>y</sub> to give I’<sub>y</sub>, y component of I convolved with the derivative of the Gaussian.</li>

   <li>Compute the magnitude of the edge response by combining the x and y components. The magnitude of the result can be computed at each pixel (x, y) as:  <sub></sub><sup></sup><sub></sub><sup>′ </sup><sup> </sup><sup></sup><sub></sub><sup>′</sup><sup> </sup>.</li>

   <li>Implement non-maximum suppression algorithm (the center pixel must have a larger gradient magnitude than its neighbors in the gradient direction) that we discussed in the lecture. Pixles that are not local maxima should</li>

  </ol></li>

</ul>

be removed with this method. In other words, not all the pixels indicating strong magnitude are edges in fact. We need to remove false-positive edge locations from the image.

<ol>

 <li>Finally apply Hysteresis thresholding to obtain the final edge-map.</li>

</ol>

<ol start="2">

 <li>You need to generate intermediate images for each step to check how your algorithm works.</li>

 <li>Try images uploaded to class page and your favorite images. For more images, refer</li>

</ol>

<a href="https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/BSDS300/html/dataset/images.html">https://www2.eec</a><u>s.berkeley.edu/Research/Projects/CS/vision/bsds/BSDS300/html/datas </u><a href="https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/BSDS300/html/dataset/images.html">et/images.html</a><a href="https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/BSDS300/html/dataset/images.html">.</a> You may calculate precision and recall for Berkeley data.

<ol start="4">

 <li>Report your experiments with analytic document.</li>

</ol>

<strong>Discussions</strong>:

<ol>

 <li>Analyze result images from three different implementation</li>

 <li>What are effects of  to images?</li>

 <li>Does Canny Edge Detector achieve the three goals?</li>

</ol>