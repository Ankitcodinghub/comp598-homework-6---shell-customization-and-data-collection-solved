# comp598-homework-6---shell-customization-and-data-collection-solved
**TO GET THIS SOLUTION VISIT:** [COMP598 Homework 6 – Shell Customization and Data Collection Solved](https://www.ankitcodinghub.com/product/comp-598-homework-6-shell-customization-and-data-collection-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;118614&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP598 Homework 6 – Shell Customization and Data Collection Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
Non-standard (i.e., built-in) python libraries you can use:

– pandas

– requests

Task 1: Inspiration on login

What if every time you logged into your EC2, it printed out a nice, inspirational word of wisdom? Now that we know about .bash_profile and .bashrc, we can do that!

Add code to your .bash_profile script that picks a random quote out of the inspirational quotes file below and prints it to out (i.e., echos it). The location of the inspirational quotes file:

https://gist.github.com/JakubPetriska/060958fd744ca34f099e947cd080b540

To do this assignment, you’ll need to download this file. Store it as ~/.data/quotes.csv (you can assume that it will be here as well when we test your script).

Your script should print the quote out on one line (it should be surrounded by quotes) and then the author underneath following a tilde. For example:

“An apple a day keeps the doctor away.”

~ Some Body

Spacing on the line itself is entirely up to you.

A couple tips as you work on this:

• In the file, some of the quotes don’t have an author on that line. In this case, it’s fine – you should just print a blank author (but the tilde will still be there).

• bash &lt;script_name&gt; will run a script file. For example, “bash .bash_profile” will run your bash script. “source .bash_profile” will also do this.

• You’ll need to write this script entirely in bash shell script… no python here! This also means no supporting libraries or methods. The only thing you’ll use are (1) shell script, (2) pipes, and (3) standard unix commands (e.g., cut, head, tail, etc…)

• To select the line, take a look at the $RANDOM bash environment variable, head, and tail.

• To get the quote, check out the cut command.

• One thing you should read up on as you work on this are the shell evaluation techniques `…` and $(…).

Task 2: Election Data Analysis (20 pts)

We’re in the final days of the presidential election, let’s collect some data about this from Reddit. We’d like to get a sense for the hottest content in the /r/politics subreddit over three consecutive days. You’re welcome to pick whichever three days you want, but it will be the most interesting on Nov 2, Nov 3, and Nov 4.

Write a script “collect_hottest.py” that collects the 500 hottest posts in the subreddit specified. It should run as follows:

For this task, you’ll use the /r/politics subreddit. So it would be run with &lt;subreddit&gt; set to “/r/politics”.

Run it at roughly the same time on three consecutive days, saving the files as &lt;yyyy&gt;&lt;mm&gt;&lt;dd&gt;_politics.json. Save one post per line – where the post is the dictionary under the “data” key.

Keep this data around – we’ll use it in our assignment next week (HW 7).

Submission Instructions

Your MyCourses submission must be a single zip file entiled HW6_&lt;studentid&gt;.zip. It should contain the following items:

– scripts/ o .bash_profile – the script for Task 1. This script ONLY has to print out a random inspirational quote when run. It should assume that the file ~/.data/quotes.csv is available.

o collect_hottest.py – the script for Task 2
