# CIS4340 HW3 Project Summary
I first installed BeautifulSoup, which was a very straightforward process. The instructions were easy to follow, and the package installed quickly without errors. I was able to run Python scripts that used BeautifulSoup to extract and work with launch data from the Falcon 9 booster table.
I also installed ScrapeGraphAI from GitHub. This installation was a bit more complex. It required pip install -e . from the command prompt. Although it took longer and involved resolving dependencies, I was eventually able to install and import the ScrapeGraphAI .

Initially, it took some time to understand how the Wikipedia table was structured. After experimenting with some scripts, I figured out how to loop through the table rows using BeautifulSoup. I used index-based column access like cols[0] for engine numbers and ucontinued a system with that for block types and so on. 
I added  checks to only include Block 4 and Block 5 engines. For example, I filtered rows where the block column contained “F9 B4” or “F9 B5.” For the aiF9only.py script, I focused on Falcon 9 launches only, ignoring anything else. For turnaround time, I grouped launch dates by booster engine, sorted the dates, and calculated the time difference between  launches. This helped me identify the fastest and longest turnaround times.

For the ScrapeGraphAI part of the assignment, I used a precise language to get specific data from the falcon 9 and this method was useful because it didn’t require manually searching through HTML tags. It made data usage more efficient when it worked properly.

I used VS code on this assignment and python 3.1 and I used beautiful soup and ScrapeGraph AI.

The turnaround scripts sometimes failed to extract valid dates. I had to add logic to skip invalid values or empty fields. I also faced issues installing ScrapeGraphAI due to missing dependencies or import errors. I resolved this by following the GitHub README carefully and ensuring the install path was correct. Sometimes, the AI returned data that skipped important details. I improved the results by refining my prompt to be more specific.
