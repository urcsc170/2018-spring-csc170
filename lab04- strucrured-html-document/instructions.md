# Lab 04: Structured HTML Document
*Due: xxx, xxx xx, 2018 at 9:00 AM (before the next lab comes out)*

This assignment tests your ability to take "real" content and mark it up using
semantically correct HTML. You will use the content you prepared from Wikipedia
and fulfill the requirements as described in this document.

1: Setup your Work Environment
==============================

-   Create your initial files:

    1.  Create a folder named **lab04** and inside it create a new HTML document
        named **start.html**

-   Inside the **start.html** file, setup a new HTML5 template.

-   In addition to the usual HTML5 template, inside the \<body\> tags, create a
    set of tags that will be used as your layout blocks. You must use the
    following tags in your HTML document:  
    **HEADER, ARTICLE, ASIDE, and FOOTER**

Here’s a template you can use to get your layout elements started:

\<!doctype html\>

\<html\>

\<head\>

\<meta charset="utf-8"\>

\<title\>Lab 04 – the title of your content\</title\>

\</head\>

\<body\>

\<header\>  
\<h1\>the title of your content\</h1\>  
\<div\>A subtitle\</div\>

\</header\>

\<article\>  
\</article\>

\<aside\>  
\</aside\>

\<footer\>

\<h2\>Citations\</h2\>

\</footer\>

\</body\>

\</html\>

Note: In the two places where it says, "*the title of your content*" you should
write the title of your content

2: Gather Content
=================

-   Using your Wikipedia content from Lab 3, extract the text and create *at
    least* these following elements:

-   For use in the HEADER, one (and only one) **H1** (which will be the name of
    the topic you selected)

-   Also in the HEADER, a subtitle

-   At least four second-level headings (**H2s**)

    -   Three of the headings go in the ARTICLE

    -   At least three **paragraphs** of text under each heading in the ARTICLE

    -   The last heading, with the lists, goes in the ASIDE

    -   Under the last heading, at least two **lists**: unordered, ordered or
        definition list (any combination)

-   In the ARTICLE, at least two **images** which may include diagrams, and
    captions for each

    -   You must wrap each \<img\> in the \<figure\> element.

    -   Inside the \<figure\> element along with the \<img\> you must include a
        \<figcaption\> element in which you'll write your caption for the
        image[^1]

        [^1]: You can make up the captions that will go with each image - just a
        couple of words that describe the image

    -   The images must be smaller than about 300px wide and larger than about
        200px wide

    -   Note: the best placement for the \<figure\> elements is right after an
        \<h2\>

-   In the FOOTER, three citations (hypertext links to other sources)

-   Also in the FOOTER, another citation, referring to the Wikipedia page(s) you
    used in this assignment

Take a look at the EXAMPLE at the end of this document. When you’re done, you
should have a document that kinda looks like that but with different content.

3: Create the HTML Document
===========================

*The point of this lab* **You must figure out how best to tag your content
semantically to identify each part of content.**

-   Populate the \<header\> element with content

    -   You’ll put your one \<h1\> in the \<header\>

    -   You'll but your subtitle in a \<div\> in the \<header\>

-   Populate the \<article\> element with \<h2\>s followed by paragraphs, and
    any other related content that belongs under each \<h2\>

-   One \<aside\> element to tag information that supports the content in your
    \<article\>.

-   Populate the \<footer\> element with content

    -   Put the citations/references in the footer element

    -   Also put links to the source(s) of your Wikipedia content in the footer

    -   You can also put your name and other info about yourself in the footer,
        if you want.

-   Remember: the HTML document MUST remain “semantically pure.” No tags to push
    content around! (Generally, that means no \<br\>, \<hr\> or extraneous \<p\>
    tags anywhere, and definitely no \<b\> or \<i\> tags.)

4: Upload your work
===================

When you are done with your webpage, use an FTP tool to access your account on
**urcsc170.org** (remember your FTP login information?) and upload your files
into a new folder named **lab04**

In a web browser (any), go to this address to check your handiwork:  
**www.urcsc170.org/accountname/lab04/start.html**  
(where “*accountname*” is your account name)

Remember: All files and folder names must always be all lowercase and no spaces.

4: Report your work
===================

Remember: Use the W3C validator (**validator.w3.org**) to check your work before
you report it!

-   In our Blackboard section, in Lab 04, create a new submission and post a
    link to your webpage to receive credit for this Lab.

Example
=======

NOTE: Do *not* use Shakespeare for your Lab 4!

![/Users/rkostin/Desktop/Screen Shot 2016-01-26 at 9.03.07 PM.png](media/78763079f20c696dfcfeb2d480e3f696.png)

…continued, next page:

![/Users/rkostin/Desktop/Screen Shot 2016-01-26 at 9.03.24 PM.png](media/a52b7a5c86f3ccd90379b769ad625f26.png)

![/Users/rkostin/Desktop/Screen Shot 2016-01-26 at 9.03.37 PM.png](media/37d9f95b6c35c1d981e3c5cd698f5511.png)
