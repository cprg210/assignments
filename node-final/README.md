# Node Final - Deployed Travel Experts Website
## Details
In this assignment, we are going to deploy a multi-page website using Express, Pug/EJS and Mongoose. It will have a database-driven "Destinations" gallery deployed to Heroku and MongoDB Atlas.

## Instructions
Use the most current version of your Travel Experts website as a template for this assignment. 

Keep in mind that design elements will be ignored for this assignment with the exception of broken usability/accessibility. 

Aside from the endpoints defined below, you may layout and organize your site, including your Destinations gallery and single item pages, as you feel appropriate. 

BUT, please make sure your instructor doesn't have to hunt to find your code...

### Project setup
- Initialize a new project using npm.
- Dependencies:
  - `express`
  - `pug`|`ejs`
  - `dotenv`
  - `mongoose`
  - `cors`
  - `moments`
  - any others as you see fit to add (and document)
- Serve static assets from a `public` directory.
- Return a custom 404 page when a file (or endpoint) cannot be found.
- Mongoose connection authenticated using `.env` file.
  - .on event for errors
  - .once event for successful connection

### Views setup
All static HTML served with EJS or Pug view templates. For each page of your site using either EJS or Pug:
- Repeating page elements (`head`,`header`,`nav`,`footer`, etc) moved to separate template "partials" in a `views/partials` directory.
- Endpoint handlers to render and serve each page template. For example:
  - `GET /`
  - `GET /register`
  - `Get /login`

### Schema/model definition
- Define `Destinations` Mongoose Schema in a dedicated `/models` directory.
- Based on the above schema, require your compiled `Destination` model into your app.
- Remember, the above singular noun will determine the name of your MongoDB collection. It will be the plural of the noun (i.e. `destinations`).

### DB seed: Destination array
Your instructor may need to build a local version of your database to mark this assignment.
- Move the custom module you've been using for Destinations data -> `./seeds/destinations.js` 
- You'll find an example in [`/sample-code/backend/5-animals-mongoose`](https://github.com/cprg210/sample-code/tree/master/backend/5-animals-mongoose)

### Dynamic HTML endpoint: `GET /destinations/:id`
- Create the following endpoint handler in your Express app:
  - `GET /destinations/:id`
- Use `model.findOne()` to return a single image document from Atlas and render a view that displays a single destination on your web page.
- The page must at least include:
  - a larger version of the gallery image,
  - page heading,
  - longer description than on gallery.

### JSON API endpoint: `GET /api/destinations`
- Create the following endpoint handler in your Express app:
  - `GET /api/destinations`
- Use `model.find()` to return all destination documents from Atlas and return a JSON list when fetched.
- The JSON should render to an identical array that is returned by your db seed described above.

### Frontend: Destinations gallery using `fetch()`
- Refactor your Destinations gallery from Assignment 2.
  - Your loop currently uses a locally defined array to display your destinations.
  - Use `fetch()` to retrieve the same array from a remote JSON endpoint hosted by your app (details above).
- Card design: 
    - each Destination should be displayed semantically
    - Example:
        
        ```html
        <figure>
          <img src="#" alt="figure">
          <figcaption>Figure</figcaption>
        </figure>
        ```

### Additional requirements
- Each page should have a unique page `<title>`.
- The current page should be indicated/highlighted in the global navigation (i.e. maybe the Contact link has a different background when the user is on the Contact page).
- The page should be readable and usable on mobile.
- The `footer` partial should contain a copyright notice for the current year using the `moment` module. Middleware!

## Submitting Your Assignment
In order to receive a grade, you must:
1. Deploy your Express/Mongoose app to Heroku and Atlas.
2. Zip your project (NOT including node_modules) and submit them to Brightspace.
3. In a comment with your Brightspace submission, include links to:
    - your GitHub repo;
    - deployed site.

## Late Penalties
For this assignment, there will be a 10% late penalty for each day the assignment is late. No assignments will be accepted more than three days late.

## Marking Rubric
This assignment will be marked out of 50 points. 5 points will be given for each of the following:
1. **Code Quality** - The code is readable: indented, spaced and organized.
2. **Project documentation** - Project has a detailed README and comments to make your instructor's life easier. The longer it takes them to figure out your code...
3. **Project Setup** - The server is properly setup based on the requirements above.
4. **Views Setup** - The views are properly setup based on the requirements above.
5. **Schema/model definition** - Schema is properly setup based on the requirements above.
6. **DB Seed** - A database build file is provided based on the requirements above.
7. **Dynamic HTML Endpoint** - `GET /destinations/:id` is setup based on the requirements above.
8. **JSON API Endpoint** - `GET /api/destinations` is setup based on the requirements above.
9. **Frontend** - fetched Destinations gallery is setup based on the requirements above.
10. **Additional Requirements** - The site is properly setup based on the requirements above.