# assignment-4-virtual-memory-simulation-csc-139-operating-system-principles--c-language-solved
**TO GET THIS SOLUTION VISIT:** [Assignment 4: Virtual Memory Simulation CSC 139 Operating System Principles -C language Solved](https://www.ankitcodinghub.com/product/assignment-4-virtual-memory-simulation-csc-139-operating-system-principles-c-language-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;12983&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Assignment 4: Virtual Memory Simulation CSC 139 Operating System Principles -C language Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (3 votes)    </div>
    </div>
1 Objectives

This programming assignment is to simulate a simple virtual memory system using the three page replace- ment policies studied in class: First-In First-Out (FIFO), Optimal, and Least Recently Used (LRU). Your program reads an input file containing a sequence of page requests (page numbers) and generates an output that shows how the requested pages are mapped into physical frames.

2 Description

The page replacement algorithms to implement in this assignment are First-In First-Out (FIFO), Optimal, and Least Recently Used (LRU). The detailed algorithms are already described in class slides and textbook Chapter 10.

2.1 Task Information

The page request information will be read from an input file. The first line in the input file has three integers. The first integer is the number of pages, the second integer is the number of frames, and the third integer is the number of page access requests. The remaining lines in the input file are page access requests (page numbers), with each page request appearing on a separate line. In an interesting input, the number of frames is less than the number of pages; otherwise, the problem is trivial. Furthermore, in an interesting input, some pages are requested multiple times (the same page number appears multiple times in the sequence). Because the number of frames is typically smaller than the number of pages, the same page may be mapped to a different frame each time it is requested.

In your simulation, assume pure demand paging, that is, pages are loaded into physical frames only when they are requested. So, initially, no pages are loaded, and all frames are free. If the number of frames is x, the first x pages accessed will be trivially mapped to the x frames without having to replace any pages. When a request to access the (x+1)-th page arrives, your program must find one of the x pages that have been loaded into physical frames and replace it with the new page. The selection of the page to be replaced depends on the page replacement policy.

• In the FIFO policy, the first page loaded into a physical frame is selected for replacement.

• In the Optimal policy, the page that will not be accessed for the longest time in the future is selected for replacement. This policy may be implemented by associating with each page table entry a number indicating its next-use time in the future. When replacement is needed, replace the page with the greatest next-use number. If a page is not referenced in the future, set its next-use time to INFINITY.

If there are multiple pages with infinite next-use times, replace the page that is currently in the smallest frame number.

• IntheLRUpolicy,thepagethathasn<wbr>otbeenaccessedforthelongesttim<wbr>eisselectedforreplacement. This policy may be implemented by associating with each page table entry a time stamp indicating the latest time at which the page was accessed. When replacement is needed, replace the page with the smallest time stamp.

The output will have one line for each page request, indicating how that page request is handled. The last line for each algorithm reports the total number of page faults. You may write your implementation in C.

2.2 Command-line Usage

Usage: proj4 input file [FIFO|LRU|OPT]

where input file is the file name with page request information. FIFO, LRU, and OPT are names of page replacement policies.

2.3 Sample Inputs and Outputs

Sample input file and expected outputs are shown below. You can use it to verify your results.

Example: Here is an example input file and the corresponding outputs. The input has 8 pages, 4 frames,

and 12 page requests. Input:

% more input1.txt

8&nbsp; 4&nbsp; 12

4

3

4 6 1 6 4 5 2 4 6 1

Output: (FIFO)

Page 4 loaded into Frame 0

Page 3 loaded into Frame 1

Page 4 already in Frame 0

Page 6 loaded into Frame 2

Page 1 loaded into Frame 3

Page 6 already in Frame 2

Page 4 already in Frame 0

Page 4 unloaded from Frame 0, Page 5 loaded into Frame 0

Page 3 unloaded from Frame 1, Page 2 loaded into Frame 1

Page 6 unloaded from Frame 2, Page 4 loaded into Frame 2

Page 1 unloaded from Frame 3, Page 6 loaded into Frame 3

Page 5 unloaded from Frame 0, Page 1 loaded into Frame 0

9 page faults

(Optimal)

Page 4 loaded into Frame 0

Page 3 loaded into Frame 1

Page 4 already in Frame 0

Page 6 loaded into Frame 2

Page 1 loaded into Frame 3

Page 6 already in Frame 2

Page 4 already in Frame 0

Page 3 unloaded from Frame 1, Page 5 loaded into Frame 1

Page 5 unloaded from Frame 1, Page 2 loaded into Frame 1

Page 4 already in Frame 0

Page 6 already in Frame 2

Page 1 already in Frame 3

6 page faults

(LRU)

Page 4 loaded into Frame 0

Page 3 loaded into Frame 1

Page 4 already in Frame 0

Page 6 loaded into Frame 2

Page 1 loaded into Frame 3

Page 6 already in Frame 2

Page 4 already in Frame 0

Page 3 unloaded from Frame 1, Page 5 loaded into Frame 1

Page 1 unloaded from Frame 3, Page 2 loaded into Frame 3

Page 4 already in Frame 0

Page 6 already in Frame 2

Page 5 unloaded from Frame 1, Page 1 loaded into Frame 1
