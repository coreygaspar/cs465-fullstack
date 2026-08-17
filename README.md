# cs465-fullstack
SNHU CS-465 Full Stack Development with MEAN

### Architecture
**Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page application (SPA).**

In this project for Travlr Getaways, I used Express with HTML, JavaScript, and Angular as a single-page app (SPA). Express and Handlebars were used for the main customer-facing website. The server uses the Express routes to determine which page the user is requesting and then uses the Handlebars templates to create the HTML that is shown in the browser. JavaScript is used to add functionality to the website and work with the information provided by the backend.

The admin side of the project uses Angular as a SPA. Compared to the Express pages, Angular doesn't need to reload the entire webpage every time the user moves to a different part of the app. Angular uses components to update specific parts of the page and services to communicate with the backend API. For example, the admin pages can retrieve, add, and edit trip information using API requests. The main difference is that Express and Handlebars rely more on the server to create webpages, while Angular handles more of the webpage in the browser.

**Why did the backend use a NoSQL MongoDB database?**

The backend used MongoDB because NoSQL databases work well with the MEAN stack and JavaScript. Compared to a SQL database that stores data in tables and rows, MongoDB stores data as individual documents, which in this case, works really well for the trip information in the Travlr Getaways app. MongoDB also works well with Node and Express, making it easier for the backend to communicate with the database. I used Mongoose to create models and manage the trip data, which allowed the app to easily add, retrieve, and update information.

---
### Functionality
**How is JSON different from Javascript and how does JSON tie together the frontend and backend development pieces?**
