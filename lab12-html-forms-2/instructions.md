# Lab 12: HTML Forms, Part 2
*Due: Wednesday, March 28, 2018 at 9:00 AM (before the next lab comes out)*

For this lab you will integrate the non-working HTML form from Part 1 into your lab website and power it with a PHP script.

The first half of this lab is simply creating a new webpage and integrating it into your existing lab website.

The second half of this lab (to be published after the lecture on Tuesday, March 27) will involve editing the *script* that makes the HTML form work.

## Step 1: Copy Lab 10

- Make a copy of your Lab 10 (*not Lab 11!*) - put it in a folder named **lab12**

## Step 2: Create a New Webpage for your HTML Form

- Make a duplicate of one of your existing webpages - any of them *except* start.php - name it: **contact.php**
- Edit the new **contact.php** file:
  - Delete the ARTICLE and ASIDE and all their contents
- Get your Lab 11 file, **contact.html** and copy-out the FORM element (all of it, from the opening FORM tag to the closing FORM tag) and paste it into the new **contact.php** file, under the *nav.inc* statement
- Edit your **inc/nav.inc** file:
  - Add a list item to the new **contact.php** file
  - Have the text for the link say something like "Contact Us" ...or something like that
  - Save and close the **inc/nav.inc** file

## Step 3: Add Styles to the HTML Form

- Edit the **contact.php** file:

  - In the opening FORM tag change the **action="#"** attribute to:<br> `action="form-processor.php"`
  - Add `class="full-width"` to the opening FORM tag

- Save and close the **contact.php** file

- Edit the **css/styles.css** file:

  - Add a class named **.full-width** to the group selector that sets the grid-column to 1/3 like this...

    ```css
    header, footer, .lead, nav, .full-width {
    	grid-column: 1 / 3;
    }
    ```

- Save and close the **css/styles.css** file

- Edit the **inc/html-top.inc** file:

  - Change the TITLE to say "Lab 12..." instead of Lab 10

  - Add a new LINK to a new stylesheet (that you'll create next) like this

    ```css
    <link rel="stylesheet" href="css/forms.css">
    ```

- Save and close the **inc/html-top.inc** file

- Create a new file in the **css** folder named **forms.css**

- Edit the new **css/forms.css** file

  - Here you can add whatever styles you want to make your HTML form look like it's a part of your website.  At the bare minimum, try these styles...

  ```css
  form { 
  	margin-top: 30px;
  }
  textarea {
  	width: 100%;
  	height: 100px;
  }
  ```

  ...do more as you'd like.  (Not graded.)

- Save and close the **css/forms.css** file


## Step 4: Create the Form Processor File

- Make a duplicate of one of your existing webpages - any of them *except* start.php or contact.php - name it: **form-processor.php**

- Edit the new **form-processor.php** file:
  - Delete the ARTICLE and ASIDE and all their contents

- Under the *nav.inc* statement, add a MAIN element with an attribute: `class="full-width"` and add some content like this:

  ```html
  <main class="full-width">
    <h2>Thank You <?php echo $_POST['name']; ?></h2>
    <p>Go back to <a href="contact.php">the contact page</a>.</p>
  </main>
  ```

  ...be really careful with that embedded PHP element in the H2 (to be explained later); make sure you enter it exactly like that; other than that edit the other text anyway you want.

- Save and close the **form-processor.php** file

<hr>

## Stop!

That's it for now.  After the lecture on Tuesday, March 27, the rest of the instructions will be posted here.