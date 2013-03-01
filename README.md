prolano - a PROgrammer's LAboratory NOtebook
============================================

Providing the scripts and tools for someone to maintain their own personal
programmer's laboratory notebook.


The Need for _Something_
------------------------

In my own experience I've found that I've run across, mused upon, and created
lots of data and interesting tidbits in the process of developing the ideas for
my various programming ambitions.  Those things I've bothered to keep track of
have ended up scattered across various bookmark files, wikis, copies of old
home directories, and so on.  Those bits of data are effectively _lost_ as I
have no capability to find and make use of them.

Eventually, I stumbled across the concept of a Laboratory Notebook as it is
used in the research sciences.  In research science the laboratory notebook is
simulatneously a daily record of what was done, the basis for future work, the
source material for publications, and a means of communicating with other
researchers.


What is a Programmer's Laboratory Notebook?
-------------------------------------------

In _Sharing the Art of IP Management_ [Thomson][1] JA Thomson defines
a laboratory notebook as:
* a daily record of every experiment you do, think of doing, or plan to do
* a daily record of your thoughts about each experiment and the results thereof
* the basis of every paper and thesis you write
* the record used by patent offices and, in the case of disputes, courts of law
  (in the event you file patents on your findings)
* a record that would enable successive scientists, working on the same
  project, to pick up where you left off or reproduce your results

[1]: http://www.iphandbook.org/handbook/ch08/p02/ "Thomson"

Starting with those ideas and modifying them for the art of programming, I came
up with the following definition for a programmer's laboratory notebook:
* a daily record of every program you write, think of writing, or plan to write
* a daily record of your thoughts about each program and the results thereof
* the basis for every programming blog and article you write
* possible evidence should you find yourself having to defend against patent
  litigation (providing you have a way to prove the dates and your work would
  constitute prior art)
* a record that would enable other programmers to pick up where you left off


Some Additional Ideas
---------------------

That definition leaves a lot of room for implementation choices. Here are some
additional requirements that I've added to help narrow things down (and why):
* notebook can be maintained using a simple text editor - personal philosophy
* notebook isn't tied to any one computer - multi-computer reality
* automatic table of contents and topical index - if it isn't automated it won't get done
* automatically turned into a set of web pages - so it's usable


How will it work?
-----------------

Here's the plan:
* git repository based, single-branch; every edit starts with a git pull and
  ends with a git push
* a process on my website that uses the repository, builds the TOC and index,
  and makes them available to the web server
* after quite a bit of research, non of the TeΧ variants have the features that I view as required for the project, so I've started designing a new format specifically to implement those features.  I'm calling it "annotated text".
* The "annotated text" format will be specified as part of this project
