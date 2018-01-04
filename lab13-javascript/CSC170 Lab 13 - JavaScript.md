---
subtitle: "Due: Tuesday, November 7, 2017"
title: "CSC 170 Lab 13: JavaScript"
---

For this lab, you will take a set of HTML and CSS **starter files**, downloaded
from Blackboard, and add JavaScript using three techniques: external; embedded;
and event

In the starter files, to help you find the places where you install the
JavaScript, look for the HTML comments in the files provided that say, “PART
1…”, “PART 2…” et cetera.

Part 0: Setup
=============

-   Download the ZIP of starter files from the Lab 12 assignment in our CSC 170
    Blackboard section, and expand the files on your computer or thumb drive
    into a folder named **lab12**

Part 1: Add an embedded script
==============================

-   Near the bottom of the HTML document, just above the closing body tag, add
    an embedded JavaScript block using the \<script\> tag, and write a line of
    JavaScript that pops open a dialog box that says a message.

-   After you've confirmed that the pop-up dialog box works, comment-out the
    JavaScript inside the \<script\> tags using "//" (two slashes) at the
    beginning of the line so it doesn’t work anymore (because it’s annoying).

Part 2: Connect to an external script
=====================================

-   Near the bottom of the HTML document, just above the embedded JavaScript you
    created in Part 1, using the \<script\> tag, connect an external JavaScript
    file named: **js/scripts.js**

Part 3: Use a JavaScript event to change an image
=================================================

Apply the following events to the first IMG element near the top of the HTML
document:

-   Add the following JavaScript event to the image element to change the source
    (the “src”) to **images/cat2.jpg** when a mouse hovers over that element

    -   **onmouseover="this.src='images/cat2.jpg';"**

-   Add the following JavaScript event to the *same image element* to change the
    source (the “src”) to **images/cat1.jpg** when a moves out from hovering
    over that element

    -   **onmouseout="this.src='images/cat1.jpg';"**

Part 4: Use JavaScript to run a function
========================================

-   Within the second \<figure\> element in the HTML document, add an ID
    attribute to the image to uniquely identify it in the HTML document (you
    pick the name of the ID)

-   Also add an ID attribute to the BUTTON element to uniquely identify it in
    the HTML document (you pick the name of the ID)

-   In the attached JavaScript file, follow the comments in the code to power
    the script to make the button work as intended.[^1]

    [^1]: You need to *replace* the blanks (____________) with the proper
    JavaScript code. Everything you need to know was covered in great detail
    during the lecture on Thursday, November 2.

Part 5: Check and Upload your Work
==================================

-   Validate the HTML file (**http://validator.w3.org/**)

When you are done with your webpage, close everything and use an FTP tool (like
*WinSCP*) to access your account on **urcsc170.org** and upload your files:

-   In a web browser (any), go to this address to check your handiwork:  
    **www.urcsc170.org/accountname/lab12/index.html**  
    (where “*accountname*” is your account name)

Part 6: Report your work
========================

-   In our CSC 170 Blackboard section in the Lab 12 assignment, post a link to
    your webpage to receive credit for this Lab.
