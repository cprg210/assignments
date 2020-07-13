# Assignment 3 - Express Website with Pug/EJS Templates and Custom Gallery Endpoint
## Details
In this assignment, we are going to deploy a simple multi-page website using Express and a view engine (either EJS or Pug). It will have a dynamic "Destinations" gallery using a Node custom module.

## Instructions
Use the most current version of your Travel Experts website as a template for this assignment. Each page should have repeating page and layout elements such as a header, footer, navigation, etc. The index page may have a unique hero section that is different than the "internal" pages.

### Project and Server Setup
- Initialize a new project using npm.
- Install the following Node modules:
  - `express` module,
  - either `[pug](https://pugjs.org/api/getting-started.html)` or `[ejs](https://ejs.co/)`,
  - `moments` module.
- Serve static assets from a `public` directory.
- Return a custom 404 page when a file (or endpoint) cannot be found.

### Template Setup
For each page of your site:
- Create a template using either [Pug](https://pugjs.org/api/getting-started.html) or [EJS](https://ejs.co/) and store them in a `views` directory:
  - `index.pug`
  - `register.pug`
  - `login.pug`
- Move repeating page elements (`head`,`header`,`nav`,`footer`, etc) to separate template "partials" and save them to a `views/partials` directory.
- Include the appropriate template partials in each page template.
- Create a GET endpoint handler to render and serve each page template.
  - `GET /`
  - `GET /register`
  - `Get /login`

### Custom Node Module: Gallery Array
- Create a custom module that you can import at the top of your `app.js` file:

    ```js
    const gallery = require('./destinations.js');
    ```

- This custom module should return the array you used for your gallery loop in Assignment 2.
- This array will be required for the functionality below.

### JSON API Endpoint: `GET /destinations`
- Create the following endpoint handler in your Express app:
- `GET /destinations`
- The server should respond with a JSON array using the custom module described above.

### Frontend: Refactor destinations gallery
- Refactor your Destinations gallery from Assignment 2.
  - Your loop currently uses a locally defined array to display your destinations.
  - Refactor your code to, instead, retrieve the same array from a remote JSON endpoint hosted by your app (details below).
- Card design: each image should be displayed semantically using the `figure`, `img` and `figcaption` elements like so:
  - `figure`
    - `img` 
      - `src` -> small image
      - `alt` -> title
    - `figcaption` -> destination description

### Additional Requirements
- Each page should have a unique page `<title>`.
- The current page should be indicated/highlighted in the global navigation (i.e. maybe the Contact link has a different background when the user is on the Contact page).
- CSS for all pages should be linked to a single external stylesheet and be included in all pages using a template partial.
- The `footer` partial should contain a copyright notice for the current year using the `moment` module.

## Submitting Your Assignment
In order to receive a grade, you must:
1. Deploy your Express app to Heroku or similar online platform.
2. Zip your project (NOT including node_modules) and submit them to Brightspace.
3. Include a link to your GitHub repo as a comment with your Brightspace submission.

## Late Penalty
For this assignment, there will be a 10% late penalty for each day the assignment is late. No assignments will be accepted more than three days late.

## Marking Rubric
This assignment will be marked out of 30 points. 5 points will be given for each of the following:
1. Code Quality - Code is properly organized, indented and commented.
2. Server Setup - The server is properly setup based on the requirements above.
3. Template Setup - The templates are properly setup based on the requirements above.
4. Custom Node Module - The custom module that returns your gallery array based on the requirements above.
5. `GET /destinations` Endpoint - The GET `/destinations` endpoint based on the requirements above.
6. Additional Requirements - The site is properly setup based on the requirements above.