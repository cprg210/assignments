  # Assignment 1: Static "Travel Experts" website
  ## Due Date
  This assignment is due Thursday, July 9th @ 8pm.

  ## Value
  This assignment will be marked out of 30 points and will be worth 50% of the frontend portion of this course (25% of the total).

  ## Requirements
  - You are building a website for the "Travel Experts" agency. They have provided the following project requirements below.
  - Create 3 pages named “index.html”, “register.html”, and login.html”.
  - **Assume that signing up new users is a primary goal of the company**. Design your website accordingly.
  - No frameworks are allowed for this project because the client is allergic to dependencies.

  ### Global Requirements
  - Each page should have a common page header, with the exception of the hero section on the home page (described in the next section).
  - Each page should have the same global navigation using `nav`, `ul`, `li` and `a` tags to link to the following pages and sections:
    - **Home**: site logo (icon font, svg or similar) and company title should link to `index.html`. 
      - on the home page, the logo/title can be included in the hero section instead of the primary navigation list.
      - on the internal pages, the logo/title can be separate from the main navigation list. For example, a common practice is to place the logo/title on the left side of the page header and the nav on the right.
    - **Destinations**: links to an image gallery section (built for the Javascript portion of this assignment) on the main page using a [document fragment link](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#Document_fragments). *This section can be empty until you build your image gallery in the Javascript portion of this course.*
    - **Contact Us**: links to the "Contact Us" section on the main page using a [document fragment link](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#Document_fragments).
    - **Login**: links to `login.html`.
    - **Sign Up**: links to `register.html`. This link can be labelled "Register" or similar if it better suits your design. 
  - Your primary navigation:
    - should have custom hover and click styles declared;
    - should highlight the current page if on Register or Login (since Gallery and Contact are on home page);
    - can have a different appearance on the home page as part of the hero section.
  - Define consistent font styles for the entire site:
    - `font-family`: use Google Fonts or Adobe Fonts for a primary font with appropriate fallbacks.
    - Balance your site text with appropriate line length, `line-height` and `font-size`. DO NOT use browser defaults. 
    - Two font faces (3 maximum) should be used for the site: one for the headings (`h1`-`h6`) and another for the rest of the site. A third may optionally be used for the primary navigation.
  - CSS should be linked as external stylesheets.
  - Each page should have a consistent footer section that includes copyright information. Include any other information you feel is appropriate.
  - The page should be minimally responsive. 
    - Page elements should be displayed in one column when viewed on a phone (assume portrait orientation).
    - No content should overflow when on mobile.
    - Note: navigation does not need to me responsive for this assignment (this will be included in the Javascript assignment).
  - All forms should:
    - be accessible:
      - include `label`s with all fields and inputs;
      - include `legend`s with all `fieldset`s.
    - have a valid submit button;
    - should submit to "#" using the `POST` method.

  ### Home page
  - [Hero section](https://envato.com/blog/exploring-hero-image-trend-web-design/): The home page should include a hero section with the following elements:
    - background image that takes up more than 50% of the viewport when the page first loads.
    - a site title (not the same as the company name) using `h1`.
    - a site tagline using `p`.
    - at least one `linear-gradient()`.
  - Gallery section: This can be blank until you complete the Javascript portion of this assignment.
  - Contact section: use lists and paragraph tags to display the contact information for the agency and the individual agents. Use the mailing address for SAIT as a placeholder.
    - Include a form that has fields for emailing the site owner. Since you don’t have a server-side script to process the data (yet), use a free [static form service](https://css-tricks.com/a-comparison-of-static-form-providers/). Follow the instructions for your chosen service when adding the form to your page.

  ### Register page
  - Primary navigation as described above.
  - Page header as described in the previous sections.
  - This page should not have enough content to create a scroll bar.
  - The footer should be visible at the bottom of the viewport.
  - Centered in the middle of the page should be an accessible form with the following fields:
    - Full Name (text field)
    - Email Address (email field)
    - Password (password field)
    - Confirm Password (password field)
    - Subscribe to Newsletter (checkbox)

  ### Login page
  - All requirements for the Register page apply, except:
  - Centered in the middle of the page should be an accessible form with the following fields:
    - Email Address
    - Password

  ## Marking Rubric
  Hand in your source code files by saving them in a .zip file and dropping it into the drop folder on Brightspace.

  Your mark is based on submitted work. Code will be examined using the following criteria.

  PLEASE NOTE: Assignments are due on the date specified by the instructor. One mark will be subtracted if the files are submitted within one week of the due date. Files submitted after 1 week of the due date will have one mark subtracted per additional day beyond one week that the file is late.

  ### Code Readbility
  - 3 points: Code is well-written, with consistent indentation, adequate white-space, and avoids long lines.
  - 2 points: Code is readable but indentation, white-space, line length could all be improved.
  - 1 point: Code is sloppy and hard to understand.

  ### Validation
  - 3 points: HTML and CSS validate with no errors.
  - 2 points: HTML and CSS some errors but an attempt has been made to fix them.
  - 1 point: HTML and CSS are a long way from validating.

  ### Logic Errors
  - 3 points: Code is free of logic errors (including design code).
  - 2 points: Code has some bugs that could not be found, but were documented and an attempt was made to fix them.
  - 1 point: Code has major bugs.

  ### Meeting Requirements
  - 3 points: Does everything the assignment requested.
  - 2 points: Does most of what the assignment requested.
  - 1 point: Only partially completed.

  ### Naming Standards
  - 3 points: Follows proper naming convention.
  - 2 points: Partially follows naming convention.
  - 1 point: Naming convention not followed.

  ### Design
  - 3 points: Code is well-planned, well-organized, modular, easy to maintain or enhance.
  - 2 points: Code could be organized better, could be difficult to maintain or enhance.
  - 1 point: Code is poorly organized, looks like it was written without much planning.

  ### Internal Documentation
  - 3 points: Code is thoroughly documented
  - 2 points: Documentation is partially done
  - 1 point: Documentation is very sparse

  ### File Submission
  - 3 points: Files are submitted to instructor by due date.
  - 2 points: Files are submitted within 1 week of due date.
  - 1 point: Files are not submitted within 1 week of due date. Beyond one week of lateness, one mark will be subtracted per additional day that the file is late.

  ### Introduction of Submission
  - 3 points: All files contain heading documentation identifying the author, date, course module and assignment.
  - 2 points: Some of the required information is missing.
  - 1 point: No identifying documentation.

  ### Filename
  - 3 points: Files are zipped into one file. Zip file name clearly indicates the course code, module/assignment name and student name.
  - 2 points: File name is not entirely clear on the required information.
  - 1 point: File name has none of the required information.