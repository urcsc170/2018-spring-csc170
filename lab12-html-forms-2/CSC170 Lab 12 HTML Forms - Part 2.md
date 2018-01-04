---
subtitle: "Due: Tuesday, October 31, 2017"
title: "CSC 170 Lab 12: HTML Forms, Part 2"
---

In this lab, you will create a "form processor" script that processes the data
from your HTML form from Lab 10, and sends it to yourself via email.

Part 0: Setup
=============

-   Make a copy of your **lab10** folder. Call it **lab11**

-   Download the ZIP'd starter file (**form-processor.zip**) from the assignment
    in Blackboard. Expand the file: **form‑processor.php** and open it in your
    code editor.[^1]

    [^1]: The file **form-processor (prof's example).php** is included for your
    review. Hopefully it helps.

Part 1: Attach the form processor
=================================

-   In the HEAD of *each* HTML file, change the title in the \<title\> tag to
    "Lab 11 - …" [^2]  
    e.g. \<title\>**Lab 11** - Shakespeare\</title\>

    [^2]: If you're still using PHP includes, this is a snap!

-   In your **contact.html** page (or contact.php), edit action attribute of the
    FORM tag - change it from"\#" to:  
    \<form method="post" action="**form-processor.php**"\>  
    ...

-   Leave your contact.html page open in your editor. You'll need to reference
    things in there as you do the rest of this lab.

Part 2: Edit the form processor
===============================

In the **form-processor.php** file, the exact code you need to fill-out the
missing parts of the form processor depends on how exactly you coded the HTML
form. You'll need to use *your* email address, plus remember all the NAME
attributes you used in your HTML form.

-   Fill out and/or create new \$_POST fields in the provided PHP code and edit
    the sections as indicated so it captures all the user input that you created
    in your HTML form, and properly sends all the input in an email to yourself
    when it's installed on a web server.

Remember: when you're working on your contact form and the form processor, they
will not work not work when you click the submit button.[^3] The form processor
only works when you install it on a web server that has an email server attached
(which our web server does).

[^3]: Unless you're using a MAMP or WAMP server. BTW - even if you're using MAMP
or WAMP, the email part may or may not work depending on your configuration.

-   Edit the provided **form-processor.php** file to work with your HTML form

    -   Set the \$emailFrom and \$emailTo variables

    -   Set the \$_POST variables to capture all the input data from your HTML
        Form

    -   In the area where the data is concatenated into the \$body variable, set
        all the labels and variables appropriately

Part 3: Create the "thank you" webpage
======================================

-   Create a simple **contact-thanks.html** (or .php) webpage - do *not* stitch
    it into your navigation system

-   Your *Thank You* webpage should use all the layout and styles as the rest of
    your website so it looks like it belongs there.

-   Have the Thank You page say an appropriate message (like "Thank you for
    filling out the form. We'll get right back to you" …or something like that),
    AND provide a link back to the contact form.

Part 4: Test and Submit the Lab
===============================

-   Upload the lab 11 files to the webserver and test it.

-   In a web browser, go to this address to check your handiwork:  
    **www.urcsc170.org/accountname/lab11/contact.html** (…or .php)  
    (where “*accountname*” is your account name)

-   Remember: Use the W3C validators to check your work before you report it!

-   In our Blackboard section, in Lab 11, post a link to your webpage to receive
    credit for this Lab.
