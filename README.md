# icdesign-homework-4-solved
**TO GET THIS SOLUTION VISIT:** [ICDesign Homework 4 Solved](https://www.ankitcodinghub.com/product/icdesign-homework-4-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93488&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ICDesign Homework 4 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Design a circuit with reset that computes the square root of an integer. There is one input, i.e., i_radicand with 10 bits, and there is one output o_root with 5 bits. Note that both radicand and root are unsigned integers(小數點後無條件捨去). The relation between inputs and outputs is

𝑟𝑜𝑜𝑡 = 𝑓𝑙𝑜𝑜𝑟 (𝑎𝑏𝑠(√𝑟𝑎𝑑𝑖𝑐𝑎𝑛𝑑)).

</div>
</div>
<div class="layoutArea">
<div class="column">
Note that the two output signals: “o_root [4:0]” and “o_finish” must be registered, i.e., they are outputs of DFFs (use module FD2 (positive edge) in lib.v ).

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
A possible architecture is as follows (not the best design):

</div>
</div>
<div class="layoutArea">
<div class="column">
Timing Diagram

Since a design can either be recursive or pipelined, the testbench provides two input strategies, i.e., recursive and pipeline.

1. Recursive

In the recursive input strategy, the circuit would be reset before every new radicand is input. Note that the radicand would be input at the next cycle right after reset.

</div>
</div>
<div class="layoutArea">
<div class="column">
2. Pipeline

In the pipeline input strategy, the circuit would only be reset once. After reset, a new radicand would be input every cycle. Also, o_finsh should maintain high once it was pulled up, and the order of input radicands and their corresponding roots should not be changed (First in, first out.).

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Signals Description

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Signal name

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
I/O

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Width

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Simple description

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
clk rst_n i_radicand o_root o_finsih number

</div>
<div class="column">
Input 1 Input 1 Input 10

Output 5 Output 1 Output 51

</div>
<div class="column">
Clock signal.

Active low asynchronous reset. Radicand number.

The square root of the radicand. Indicate that the calculation was finished. The number of transistors.

</div>
</div>
<div class="layoutArea">
<div class="column">
Design Rules

Those who do not design according to the following rules will not be graded.

➢ LUT-based designs are not allowed.

<ul>
<li>➢ &nbsp;There should be a reset signal for the register.</li>
<li>➢ &nbsp;You are free to add pipeline registers.</li>
<li>➢ &nbsp;You can loosen your simulation timing first, (i.e., `define CYCLE XXXX in
the testbench.v), then shorten the clock period to find your critical path.
</li>
<li>➢ &nbsp;Your design should be based on the standard cells in the lib.v. All logic operations in your design MUST consist of the standard cells instead of using
the operands such as “+”, “-”, “&amp;”, “|”, “&gt;”, and “&lt;”.
</li>
<li>➢ &nbsp;Design your homework in the given “sqrt.v” file. You are NOT ALLOWED to
change the filename and the header of the top module (i.e. the module name

and the I/O ports).

➢ If your design contains more than one module, don’t create a new file for them,

just put those modules in “sqrt.v.”

Grading Policy

1. Gate-level design using Verilog (70%)

Your score will depend on both the correctness and performance of your design.

(a) Correctness Score (40%)

At this stage, we will only evaluate whether the function of the sqrt module is correct. Time and area are not considered. We provide a testbench with 1000 patterns which automatically grades your design. Your score in this part will be

40 × 𝑐𝑜𝑟𝑟𝑒𝑐𝑡 𝑛𝑢𝑚𝑏𝑒𝑟. 1000

(b) Performance Score (30%)

At this stage, you need to add up the number of transistors of all used cells in the sqrt module and connect it to number [50:0].
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Only in this section, you are allowed to use “assign” and “+” to help with calculations.

We will rank all students who pass (a) and have no connection errors on number [50:0] port. There will be a ranking according to A*T, where A represents the number of transistors and T represents the total execution time. Your performance score will be according to your ranking as the table below.

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Percentage of passing students

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Performance Score

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
If your ranking &gt; 80% ~ 90% 70% ~ 80% 60% ~ 70% 50% ~ 60% 40% ~ 50% 30% ~ 40% 20% ~ 30% 10% ~ 20%

0% ~ 10%

</div>
<div class="column">
90 % 30 27 24 21 18 15 12

</div>
</div>
<div class="layoutArea">
<div class="column">
2. Report

(a) Simulation

</div>
</div>
<div class="layoutArea">
<div class="column">
Write down your minimum cycle time and which strategy you used. If you do not provide these information, “1. Gate-level design using Verilog (70%)” will not get any score. This minimum cycle time would be verified by TAs. Also, put the screenshot of the summary provided by the testbench in the report.

(b) Circuit diagram

You are encouraged to use software to help draw architecture instead of hand drawing. Plot it hierarchically so that readers can understand your design easily. All of the above will improve your report score.

(5%) Plot the gate-level circuit diagram of your design.

</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
(c)

</div>
<div class="column">
Discussion

Discuss your design.

➢ (3%) Introduce your design.

➢ (2%) How do you cut your pipeline?

➢ (5%) How do you improve your critical path and the number of transistors? ➢ (5%) How do you trade-off between area and speed?

➢ (5%) Compare with other architectures you have designed (if any).

</div>
</div>
<div class="layoutArea">
<div class="column">
(5%) Plot critical path on the diagram above.

</div>
</div>
<div class="layoutArea">
<div class="column">
Notification

Following are the files you will need (available on the class website) HW4.zip includes

◼ HW4_2020.pdf: This document.

◼ HW4_tutorial_2020.pdf: Tutorial in class.

◼ sqrt.v:

Dummy design file. Program the design in this file.

The header of the top module and the declaration of the I/O ports are predefined in this file and you are not allowed to change them.

<ul>
<li>◼ &nbsp;lib.v: Standard cells.</li>
<li>◼ &nbsp;tb.v:
The testbench for your design.

◼ pattern/radicand.dat:

Input patterns for the testbench. Please keep the hierarchy when simulation.

◼ pattern/golden.dat:

Patterns of correct answers for the testbench. Please keep the hierarchy when simulation.

Submission

All students who do not submit files according to the rules will get a 20% penalty. ➢ You should upload a zip file to CEIBA, the file name is “HW4_Student ID_vx”,

vx represents the version you submitted. Ex: HW4_b07901001_v1.zip ➢ Your file must conform to the following structure.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
Testbench

1. Description

<ul>
<li>➢ &nbsp;The output waveform will be dumped to file “sqrt.fsdb”, you can use nWave to examine it.</li>
<li>➢ &nbsp;You can change the number of test data to debug, but the final score will still test 1000 data. (`define PATTERN 1000)</li>
<li>➢ &nbsp;You can enable the debug function, which will display the data sent and received.</li>
<li>➢ &nbsp;If you passed the simulation, you should see:
Otherwise, you would see:

You would also see the summary:

Note that the performance score is the A*T value that would be used in ranking.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
2. Simulation command

(a) Recursive

&gt; ncverilog tb.v sqrt.v lib.v &gt; ncverilog tb.v sqrt.v lib.v

(b) Pipeline

&gt; ncverilog tb.v sqrt.v lib.v

&gt; ncverilog tb.v sqrt.v lib.v +access+r +define+DEBUG+PIPELINE

</div>
</div>
<div class="layoutArea">
<div class="column">
+access+r +access+r

</div>
<div class="column">
+define+DEBUG

</div>
</div>
<div class="layoutArea">
<div class="column">
+access+r

</div>
<div class="column">
+define+PIPELINE

</div>
</div>
</div>
