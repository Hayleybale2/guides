# WTF is bloat?

In this guide we talk a lot about 'bloatware', but what is bloatware?  
Sadly the exact definition may vary on context, so for this project I have decided to 'create' may own definition of bloatware to explain and elaborate on how do I choose software to add to this guide.  

## How this guide was build in the past

The original creator of this project mayfrost stated: > The list is built pointing to software that has alternatives with less dependencies, and addressing dependencies was the easy thing. Some tools in particular were included because they add less dependencies overall while keeping a system functional. One such example is imagemagick and ffmpeg, by which you can do a lot of work and replace many tools by just using those with scripts and replace something like a screenshot utility. Certainly it would be great to have a comparative on resource usage. However, a new revision now includes software that was previously discarded for better comparison and featured recommendations will not be highlight for the moment.  

From this we can see that the criteria in the biginning of the project was:  
1. For each piece of software, it must have as little dependencies as possible.
2. To have a fully functional system with as little installed packages as possible. (So if a program had 3 dependencies, but it can replace 5 or more different programs, it gets priority).  

This is a good start, but for the second version (my fork) of the project, I gave priority to overall installation size (including dependencies).

So thus far, we have 2 ways of measuring bloat (by number of dependencies and by installation size).

Ok, so we have a way to measure bloat... right?  

Well, yes and no.  

Yes, because we have a way of measuring some sort of software bloat, but it does not tackle the principle problem with software bloat: user experience.  

## How I will measure bloat in the future

Who, literary WHO CARES if a program has too many dependencies, or if it takes 20 or 50 MB more of space? What we The Users care about is:
1. Do the program runs smoothly on an average system? If yes, then good else BLOAT.
2. Do the program takes more resources than necessary, be for general usage or general runtime (for daemons)? If yes, then BLOAT else good.  

So measuring this is important. You can even see in the mayfrost quote that he was thinking about it. But measuring this implies taking a lot more measures.  
To start, we will define my system as the 'average system'.  
Then we will define the 3 following resources:
1. % of CPU usage
2. MB of RAM
3. MB of SSD or HDD  
The priority of the resources follows the order in which they are defined (CPU gets the highest priority, HDD the lowest) this because that order follows the general price for those things.
