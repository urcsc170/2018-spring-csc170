---
subtitle: "Due: Tuesday, November 21, 2017"
title: CSC 170 Lab 16 - Menu Highlighter
---

Just like Lab 9: Website Construction, Part 1, you will take your existing
website from your lab assignments and factor out some of the duplicate code, and
place the duplicate code in *Server-Side Includes* using PHP. Then you will use
a jQuery plugin to automatically apply a *current menu highlighter* to the
website navigation element.

Step 1: Setup
=============

**IMPORTANT: If you've been using PHP includes since Lab 9, you may skip this
section and jump to Step 2.**

Follow all the instructions from Lab 9, "Part 1" through "Part 6", except
instead of making a copy of your **lab08** folder, you will make a copy of your
**lab14** folder. (And all the instructions that refer to "Lab 9" or "lab09"
should be "Lab 14" or "lab14" respectively)

Also, notice that the number of CSS files you use on certain pages has grown
since Lab 9, so instead of this in "Part 4" on page 2:

>   \<!doctype html\>

>   \<html lang="en"\>

>   \<head\>

>   \<meta charset="utf-8"\>

>   \<title\>**Lab 9** - Shakespeare\</title\>

>   \<link rel="stylesheet" href="css/styles.css"\>  
>   \<link rel="stylesheet" href="css/navigation.css"\>  
>   \</head\>

>   The code you should place in your inc/html-top.inc file should be this:

\<!doctype html\>

\<html lang="en"\>

\<head\>

\<meta charset="utf-8"\>

\<title\>**Lab 15** - Shakespeare\</title\>

\<link rel="stylesheet" href="css/styles.css"\>

\<link rel="stylesheet" href="css/navigation.css"\>

\<link rel="stylesheet" href="css/form.css"\>

\<link rel="stylesheet" href="css/hero.css"\>

\<link rel="stylesheet" href="sss/sss.css"\>

\<link rel="stylesheet"
href="http://code.jquery.com/ui/1.11.4/themes/smoothness/jquery-ui.css"\>  
\</head\>

Step 2: Install the Menu Highlighter Plug-in
============================================

-   From Blackboard, download the ZIP containing the file:
    **menu-highlighter.js** and install the JS file in a folder name **js** in
    your **lab15** folder

Note: The **menu-highlighter.js** file will automatically insert the
"is-current" class on the appropriate menu item in the navigation. But you have
to install the **menu-highlighter.js** file on every page to make it work. But
instead of doing that on every page…

-   Create a new *include* file in the **inc** folder named **scripts.inc**  
    

-   In the **scripts.inc** file, install jQuery (because the menu highlighter
    plugin uses jQuery) and then install the plugin like this:

\<script
src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.0/jquery.min.js"\>\</script\>

\<script src="js/menu-highlighter.js"\>\</script\>

-   Then in the appropriate place on each webpage (directly above the closing
    BODY tag) use the PHP code to include the scripts.inc file like this:

>   \<?php include "inc/**scripts.inc**"; ?\>

-   Note that the **index** page, the jQuery installation already exists. You
    must never install the same library twice on the same page! So…

-   In the **index** file, REMOVE the SCRIPT tag that installs jQuery. And then
    insert the PHP include that points to the **scripts.inc** file in its place,
    *above* the other JS files (like SSS, jQuery UI, et cetera)

Part 3: Upload your Work
========================

When you are done with your webpage, close everything and use an FTP tool to
access your account on **urcsc170.org** and upload your files:

-   In a web browser (any), go to this address to check your handiwork:  
    **www.urcsc170.org/accountname/lab15**  
    (where “*accountname*” is your account name)

When you look at your Lab 15 website in your browser as it’s being served from
the class web server:

-   All the Include statements should work on each webpage -- each page should
    look normal (as if the PHP includes didn't exist)

-   The current menu highlighter should work

…if not, you have some debugging to do. Good luck! Figure it out.

Part 4: Report your work
========================

In our Blackboard section, in Lab 15, post a link to your website to receive
credit for this Lab.
