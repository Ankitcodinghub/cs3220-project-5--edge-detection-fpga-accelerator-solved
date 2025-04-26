# cs3220-project-5--edge-detection-fpga-accelerator-solved
**TO GET THIS SOLUTION VISIT:** [CS3220 Project 5- Edge detection FPGA accelerator Solved](https://www.ankitcodinghub.com/product/cs3220-project-5-10-pts-edge-detection-fpga-accelerator-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;126103&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3220 Project 5- Edge detection FPGA accelerator Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Description

In this assignment, you will develop an edge detection mechanism using FPGA. The edge detection mechanism is based on the Sobel edge algorithm. You can read the background introduction about the Sobel operator on Wikipedia.

The Sobel edge algorithm is built on top of a convolution function and we are offloading convolution operations to the FPGA. The convolution operations are implemented using Vitis HLS and the rest of interface code and overlay is running on Python.

The provided convolution operation is a basic implementation which is not scalable. Optimizing the convolution operation is your main task in this project.

Part-1: Improving the provided Convolution Operation (10 pts)

To optimize the code, understanding the HLS compiler’s outcome reports are critical.

In this design, you will optimize your code to handle bigger image sizes or faster.

The possible options of code are:

[1] Remove copy loops (It will improve the performance)

[2] Convert the code to use tiled convolution operation. (it will provide the scalability)

[3] Convert the code to use line buffers (or sliding window). ( It will provide the scalability)

In you report, you should report a screenshot of latency table and the total latency (sum of the latency) . You should also show BRAM and DSP unit usage for your designs.

Draw three charts (y-axis: total latency, BRAM usage, DSP usage), x-axis different designs.

Grading Policy * (10 pts) : improves performance and supports scalalbe image

(8 pts) : improves performance or support scalable image

Details on the grade distrubition based on implementation: 1. Removing loops only 3 pts 2. Removing loops + other significant optimizations 5 pts

3. Tiled or line buffer implementation 8 pts 4. Line buffer + other optimizations 10 pts

Part-2 Produce Bit-stream and running it on Pynq boards (Bonus 2 pts)

In this step you will use Vitis and Vivado to build the FPGA block diagram as you did in project #4. This Sobel accelerator uses DMA to transfer images between CPU and the FPGA, so you need to use a different interconnect. Please refer to DMA instructions provided in the DMA directory for instructions on how to set up DMA.

Now, we provide two different notebooks to test your vitis design.

To synthesize the file you need to reduce TEST_IMAGE_ROW/TEST_IMAGE_COL/TEST_IMAGE_SIZe as 30,30, 900. (make it run 100,100,10000) cv_edge_arm.ipynb and cv_edge_fpga.ipynb.

cv_edge_arm performs sobel edge detection using ARM processors. Every operations are performed using python code. In cv_edge_fpga, convolution operations are offloaded to FPGA.

The provided jupyternotebook code is a minimum code to start. It requires for you to update to take new filter values.

Grading Policy* (2 pts): complete the design and demonstrate the edge detection (1 pt): see gray/solid box

What to submit

[1] project5_report.pdf: Max 3 pages (including all figures) describing the designs you have tried. [2] bit stream of the best performing design &amp; tcl &amp; hwh [3] source code of your example.cpp [4] Vivado project (please include the source code) [5] A screenshot of the notebook jupyter included in the report. [6] modified ipynb file

FAQ

*[Q]: Where can I find the compiler’s optimization results?

*[A]: It’s shown on console window or go to your vitis directory and under solution1, you will see solution1.log

*[Q]: what should I discuss in the report?

*[A]: Discuss what optimizations you did and how the latency has been changed.
