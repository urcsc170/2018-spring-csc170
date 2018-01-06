---
subtitle: "Due: Tuesday, October 24, 2017"
title: CSC170 Lab 10 - PHP Includes
---

For this lab, you will take your existing website from your lab assignments and
factor out some of the duplicate code, and place the duplicate code in
*Server-Side Includes* using PHP.

Part 1: Setup
=============

-   Make a copy of your lab 08 folder and name the new folder **lab09**

Part 2: Change the files from HTML to PHP
=========================================

-   Change the file extensions of all the HTML files from **.html** to **.php**

Reminder: after you change the file extensions you can no longer view your web
pages by simply double-clicking on the HTML files. From here on out, you’re
working “blind” until you upload your files to the web server.[^1]

[^1]: The exception to this is: if you load a “WAMP” stack or “MAMP” stack on
your computer. That would allow you to view PHP files on your own computer, but
that’s not necessary for CSC 170. If however, you’re interested in doing that
anyway, ask the professor!

Part 3: Setup the new “include” files
=====================================

-   Inside the **lab09** folder create a new folder named **inc**

-   In the **inc** folder create three new plain text files with these names:  
    **html-top.inc**  
    **nav.inc**  
    **footer.inc**

-   Open all the **.php** files (the files that used to be .html) in your code
    editor

-   Open all three **.inc** files in your code editor

The rest of this lab requires you to juggle a lot of open files while copying
and pasting code between them. It’s easy to make mistakes and mess thing up. Go
slowly!

Part 4: Replace the header HTML with a PHP “include” script
===========================================================

-   In the file: **start.php** *cut* the following code to your computer’s
    clipboard…

>   \<!doctype html\>

>   \<html lang="en"\>

>   \<head\>

>   \<meta charset="utf-8"\>

>   \<title\>Lab 8 – Shakespeare\</title\>

>   \<link rel="stylesheet" href="css/styles.css"\>  
>   \<link rel="stylesheet" href="css/navigation.css"\>

>   \</head\>

>   …and paste it into the file: **html-top.inc**

-   Edit the code in the **html-top.inc** file – update the Lab number

>   \<!doctype html\>

>   \<html lang="en"\>

>   \<head\>

>   \<meta charset="utf-8"\>

>   \<title\>**Lab 9** - Shakespeare\</title\>

>   \<link rel="stylesheet" href="css/styles.css"\>  
>   \<link rel="stylesheet" href="css/navigation.css"\>  
>   \</head\>

-   In the file: **start.php** type the following code in the place where you
    just made the cut …

>   \<?php include "inc/**html-top**.inc"; ?\>

-   In the four other **.php** files, delete the code…

>   \<!doctype html\>

>   \<html lang="en"\>

>   \<head\>

>   \<meta charset="utf-8"\>

>   \<title\>Lab 8 – Shakespeare\</title\>

>   \<link rel="stylesheet" href="css/styles.css"\>  
>   \<link rel="stylesheet" href="css/navigation.css"\>  
>   \</head\>

>   …and replace that code with the same line of PHP code in each…

>   \<?php include "inc/**html-top**.inc"; ?\>

Part 5: Replace the menu HTML with a PHP “include” script
=========================================================

Note: doing this step will break the "is-current" menu highlighter. That's okay.
We'll fix it in a later lab assignment.

-   In the file: **start.php** *cut* the following code to your computer’s
    clipboard…

>   \<nav\>

>   \<ul\>

>   \<li\>\<a href="cats.html"\>Cats\</a\>\</li\>

>   \<li\>\<a href="dogs.html"\>Dogs\</a\>\</li\>

>   \<li\>\<a href="fish.html"\>Fish\</a\>\</li\>

>   \<li\>\<a href="bears.html"\>Bears\</a\>\</li\>

>   \</ul\>

>   \</nav\>

>   …and paste it into the file: **nav.inc**

-   Edit the code in the **nav.inc** file:  
    - Replace every instance of **.html** with **.php**

>   \<nav\>

>   \<ul\>

>   \<li\>\<a href="cats.**php**"\>Cats\</a\>\</li\>

>   \<li\>\<a href="dogs.**php**"\>Dogs\</a\>\</li\>

>   \<li\>\<a href="fish.**php**"\>Fish\</a\>\</li\>

>   \<li\>\<a href="bears.**php**"\>Bears\</a\>\</li\>

>   \</ul\>

>   \</nav\>

-   In the file: **start.php** type the following code in the place where you
    just made the cut …

>   \<?php include "inc/**nav.inc**"; ?\>

-   In the other **.php** files, delete the code…

>   \<nav\>

>   \<ul\>

>   \<li\>\<a href="cats.html"\>Cats\</a\>\</li\>

>   \<li\>\<a href="dogs.html"\>Dogs\</a\>\</li\>

>   \<li\>\<a href="fish.html"\>Fish\</a\>\</li\>

>   \<li\>\<a href="bears.html"\>Bears\</a\>\</li\>

>   \</ul\>

>   \</nav\>

>   …and replace that code with the same line of PHP code in each…

>   \<?php include "inc/**nav.inc**"; ?\>

Part 6: Replace the footer HTML with a PHP “include” script
===========================================================

-   In the file: **start.php** *cut* the following code to your computer’s
    clipboard…

>   \<footer\>

>   \<h2\>Citations\</h2\>

>   \<p\>From Wikipedia: \<a
>   href="http://en.wikipedia.org/wiki/William_Shakespeare"\>William
>   Shakespeare\</a\> and \<a
>   href="http://en.wikipedia.org/wiki/Shakespeare%27s_plays"\>Shakespeare's
>   plays\</a\>. This webpage, by Robert M Kostin\</p\>

>   \</footer\>

>   …and paste it into the file: **footer.inc**

-   In the file: **start.php** type the following code in the place where you
    just made the cut …

>   \<?php include "inc/**footer**.inc"; ?\>

-   In the four other **.php** files, delete the code…

>   \<footer\>

>   \<h2\>Citations\</h2\>

>   \<p\>From Wikipedia: \<a
>   href="http://en.wikipedia.org/wiki/William_Shakespeare"\>William
>   Shakespeare\</a\> and \<a
>   href="http://en.wikipedia.org/wiki/Shakespeare%27s_plays"\>Shakespeare's
>   plays\</a\>. This webpage, by Robert M Kostin\</p\>

>   \</footer\>

>   …and replace that code with the same line of PHP code in each…

>   \<?php include "inc/**footer**.inc"; ?\>

Part 7: Upload your Work
========================

When you are done with your webpage, close everything and use an FTP tool to
access your account on **urcsc170.org** and upload your files:

-   In a web browser (any), go to this address to check your handiwork:  
    **www.urcsc170.org/accountname/lab09**  
    (where “*accountname*” is your account name)

When you look at your Lab 9 website in your browser as it’s being served from
the class web server:

-   All the Include statements should work on each webpage -- each page should
    look normal (as if the PHP includes didn't exist)

…if not, you have some debugging to do. Good luck! Figure it out.

Part 9: Report your work
========================

-   In our Blackboard section, in Lab 9, post a link to your webpage to receive
    credit for this Lab.
