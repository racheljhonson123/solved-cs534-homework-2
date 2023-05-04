Download Link: https://assignmentchef.com/product/solved-cs534-homework-2
<br>
This assignment involves Texture Synthesis and Image Inpainting . The goal is to implement and evaluate the idea of Texture Synthesis by Non-Parametric Sampling proposed by Efros and Leung, ICCV99, and region filling by Criminisi et al “Region Filling and Object Removal by Exemplar-Based Image Inpainting”, TIP 2004

<h2>1.1.    Paper and Code</h2>

Efros and Leung paper can be found at: <a href="http://graphics.cs.cmu.edu/people/efros/research/EfrosLeung.html">http://graphics.cs.cmu.edu/people/efros/research/EfrosLeung.html </a>A pseudo-code for their work is provided in: <a href="http://graphics.cs.cmu.edu/people/efros/research/NPS/alg.html">http://graphics.cs.cmu.edu/people/efros/research/NPS/alg.html</a>

The algorithm is also described in Forsyth and Ponce textbook in Chapter 6, and in Szeliski’s textbook in Section 10.5.

Criminisi’s paper can be found in <a href="http://research.microsoft.com/apps/pubs/default.aspx?id=70029">http://research.microsoft.com/apps/pubs/default.aspx?id=70029</a>

<h1>2.     Main Task</h1>

<h2>2.1.    Preliminaries</h2>

You will be given five images that you are going to use for synthesis.

Download the test images from Sakai resources

<h2>2.2.    Implementation and Experiments</h2>

<h3>2.2.1.   Texture Synthesis</h3>

Write a Python code, implementing Efros and Leung’s approach, to synthesize a 200×200 pixel image for each of the five example images T1,T2,…, T5.gif. Show synthesized images for T1,T2,…, T5.gif by changing the WindowSize parameter to 5, 9,11 pixels around the center.

<h3>2.2.2.   Image Inpainting</h3>

Use your code (with modification if necessary) to fill in the gaps (black regions) in the images test_im1.bmp, test_im2.bmp. Try different parameter settings 5, 9, 11, and others if necessary, to see which one give you the best results. Comment about it in your report.

<h3>2.2.3.   Object Removal</h3>

A better image inpainting approach was proposed in Criminisi, Perez and Toyama, “Region Filling and Object Removal by Exemplar-Based Image Inpainting”, Download and read that paper. Write your own implementation of the algorithm in Python.

The goal of this experiment is to compare Efros and Leung approach, which you implemented in 2.2.1, and this newer algorithm, for the task of object removal. The task is removing three objects/regions from the image test_im3 (the man on the left, the sign and pole on the bottom right, and the oversaturated area on the ground). Use and compare both approaches for this task. This is a color image, so first you need to convert it to a grayscale image. Run both codes on the image, with one of the regions marked to be filled at a time, and compare the results.

<h3>2.2.4.   Image Quilting</h3>

In another paper by Efros and Freeman titled “Image Quilting for Texture Synthesis and Transfer”, SIGGRAPH 2001, another texture synthesis approach was proposed. Read that paper and <u>download an implementation</u> of that algorithm (or write your own) and compare its performance with Efros and Leung’s algorithm on the example images. Write a short essay (up to 1 page) summarizing the Imaging Quilting approach and describing in what ways it is similar or difference from Efros and Leung’s, and how they are compared quantitatively and/or qualitatively.

<h3>2.2.5.   About Efficiency</h3>

It is very important to write an efficient code. To achieve that, avoid using for/while loops and try to use array and matrix operations instead, which are much faster. Also try to write your code using built-in functions, whenever possible. Report the running time.

<h3>2.2.6.   Submitting the Code</h3>

You will submit all your code to Sakai. There should be at least two files; one for texture synthesis and one for image inpainting/region filing.

<h2>2.3.    Report</h2>

Write a report with all necessary images properly labeled. Submit only a softcopy of your report to Sakai.

<h3>2.3.1.   Images</h3>

Show synthesized images for T1,T2,…, T5.gif by changing the WindowSize parameter to 5, 9,11 pixels around the center.

In total you will have 21 synthesized images (7 images x 3 parameter settings). If you find a different better parameter set for inpainting part, submit result of that as well and comment about it in the report.

Show the output of the two region filling approaches on the three regions in image test_im3