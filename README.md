# csci3753-assignment-2-solved
**TO GET THIS SOLUTION VISIT:** [CSCI3753 Assignment 2 Solved](https://www.ankitcodinghub.com/product/csci3753-9-25-21-442-pm/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;118652&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI3753 Assignment 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (2 votes)    </div>
    </div>
Programming Assignment Two

Introduction

In this assignment we will explore file I/O and how to implement a basic device driver inside a Loadable Kernel Module (LKM). First, you will write a user-space C program that takes commands from the user to read, write and seek on a file. You will use this program to test the functionality of a custom device driver that you’ll create in Part B.

Part A – User-Space Test Program

Write an interactive test program that will allow you to read from, write to and seek in a file. Your program should accept the name of the file on the command line:

./pa2test filename

If the filename doesn’t exist, or isn’t readable/writeable, your program should print an error message, and terminate with a non-zero exit status.

Once successfully invoked, your interactive program should open filename for reading/writing, prompt the user with the string Option (r for read, w for write, s for seek): and then accept the following input, followed each time by the carriage return/enter key:

r – Your test program should immediately ask for the number of bytes to read using the prompt:

Enter the number of bytes you want to read:

Making sure you create a large enough buffer using malloc(), read the file starting from it’s current position. Then, print the returned data out to the console (stdout), followed by a newline (” “).

w – Your program should ask for the data to be written to the file, using the prompt:

Enter the string you want to write:

https://canvas.colorado.edu/courses/74858/assignments/1089929?module_item_id=2973991 1/2

9/25/21, 4:42 PM PA2 – Part A

The user then enters the desired data terminated by a carriage return. Your program should then write this data to the file.

s – Your program should prompt for values for offset and whence:

Enter an offset value:

Enter a value for whence (0 for SEEK_SET, 1 for SEEK_CUR, 2 for SEEK_END):

Your program should then set it’s position in the file according to the offset and whence. See the lseek manpage (https://man7.org/linux/man-pages/man2/lseek.2.html) for more info.

control+d – Terminate the program, and return the success exit status.

Other – If the user enters something other than listed above, ignore it and prompt the user again.

We’ve included a precompiled pa2test for you to use as an example. Download it from here, and then chmod +x ~/Downloads/pa2test to make it executable.

Submission

You are required to submit the following to Canvas:

pa2test.c

https://canvas.colorado.edu/courses/74858/assignments/1089929?module_item_id=2973991 2/2
