# Assignment 2: Website enhancements
## Due Date
This assignment is due Wednesday, July 12th @ 8pm.

## Value
This assignment will be marked out of 30 points and will be worth 50% of the frontend portion of this course (25% of the total).

## Requirements
- Using the code you wrote for Assignment 1, enhance your travel website.
- You should update existing code to fix bugs and modify the design as needed.

### Form validation
Use HTML5 form validation to enhance your registration and login forms:
- Make all fields required. Make it obvious to the user that they are required (convention is to use a red asterisk).
- Ensure the email field has the correct input type to enforce proper email formatting.
- To protect the user's privacy, all password fields should 
  - hide the characters typed into the form;
  - enforce a minimum length of 8 characters;
  - display a notice near the field notifying the user about the 8 character minimum length.
- Add custom CSS styles for `:invalid` fields (for example, add a red outline when invalid).

### Destinations image gallery
On your main page, create an array of objects (limit this to a reasonable number, perhaps 5 or 6 items). When the body of the page loads, loop through the array (i.e. using `array.forEach` or similar), get each object and add an image with description/link to a grid or flexbox gallery. 

Each object will define 
- the image `src` URL
- the image `alt` text
- description of a popular travel destination. 
- link URL that will open an external website (in a new window/tab) relating to the image

### Bonus points: Hamburger Menu
Up to 3 additional points (to a max of 100% for the assignment) will be awarded for a working hamburger menu:
- Full menu displayed for devices in 'landscape' orientation.
- Menu replaced by Hamburger Menu icon for devices in 'portrait' orientation.
- A JS click handler will toggle the menu when icon is clicked.

## Marking Rubric
Hand in your source code files by saving them in a .zip file and dropping it into the drop folder on Brightspace.

Your mark is based on submitted work. Code will be examined using the following criteria.

PLEASE NOTE: Assignments are due on the date specified by the instructor. One mark will be subtracted if the files are submitted within one week of the due date. Files submitted after 1 week of the due date will have one mark subtracted per additional day beyond one week that the file is late.

### Code Readability
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