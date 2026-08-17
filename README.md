# cs465-fullstack
SNHU CS-465 Full Stack Development with MEAN

### Architecture
**Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page app (SPA).**

In this project for Travlr Getaways, I used Express with HTML, JavaScript, and Angular as a single-page app (SPA). Express and Handlebars were used for the main customer-facing website. The server uses the Express routes to determine which page the user is requesting and then uses the Handlebars templates to create the HTML that is shown in the browser. JavaScript is used to add functionality to the website and work with the information provided by the backend.

The admin side of the project uses Angular as a SPA. Compared to the Express pages, Angular doesn't need to reload the entire webpage every time the user moves to a different part of the app. Angular uses components to update specific parts of the page and services to communicate with the backend API. For example, the admin pages can retrieve, add, and edit trip information using API requests. The main difference is that Express and Handlebars rely more on the server to create webpages, while Angular handles more of the webpage in the browser.

**Why did the backend use a NoSQL MongoDB database?**

The backend used MongoDB because NoSQL databases work well with the MEAN stack and JavaScript. Compared to a SQL database that stores data in tables and rows, MongoDB stores data as individual documents, which in this case, works really well for the trip information in the Travlr Getaways app. MongoDB also works well with Node and Express, making it easier for the backend to communicate with the database. I used Mongoose to create models and manage the trip data, which allowed the app to easily add, retrieve, and update information.

---
### Functionality
**How is JSON different from JavaScript and how does JSON tie together the frontend and backend development pieces?**

JSON and JavaScript are different because JavaScript is a programming language, while JSON is a format that is used to store and transfer data. In this project, JSON connects the frontend and backend by allowing them to exchange information in a format both sides can understand. For example, when the Angular frontend requests trip information, the Express backend retrieves the data from the database and sends it back in the form of JSON. Angular can then use that JSON data to display the trips on the webpage. When an admin adds or edits a trip, the frontend can also send the information to the backend in the form of JSON, where it is processed and saved in the database.

**Provide instances in the full stack process when you refactored code to improve functionality and efficiencies, and name the benefits that come from reusable user interface (UI) components.**

During development, I refactored my code by separating the app into different parts, such as routes, controllers, models, services, and Angular components. For example, instead of putting all of the trip functionality in one place, I separated the API communication into its own service and used components for different tasks like adding and editing trips. This made the code easier to understand, maintain, and troubleshoot when I had issues. Reusable UI components also make development much more efficient since the same component can be used in multiple parts of an app without having to rewrite the same code. They also help keep design and functionality consistent throughout the entire app.

---
### Testing
**Methods for request and retrieval necessitate various types of API testing of endpoints, in addition to the difficulties of testing with added layers of security. Explain your understanding of methods, endpoints, and security in a full stack app.**

In a full stack app, HTTP methods and endpoints are used to allow the frontend and backend to communicate. Different methods are used for different actions, such as GET to retrieve information, POST to add new information, PUT to update existing information, and DELETE to remove information. An endpoint is a URL that is used to specifically handle one of these requests, such as the Travlr API endpoint used to retrieve trip information. I used Postman to test these endpoints and make sure they returned the correct information and handled requests properly. Security adds another layer to testing because some endpoints should only be available to authenticated users. In the Travlr app, JWT authentication was used to protect the administrative side, so the user's identity must be verified before they can access protected features.

---
### Reflection
**How has this course helped you in reaching your professional goals? What skills have you learned, developed, or mastered in this course to help you become a more marketable candidate in your career field?**

This course has helped me move closer to my goal of becoming a software developer, which is something I have always wanted to pursue. The course gave me hands-on experience building a full stack app and helped me better understand how the frontend, backend, API, and database work together. I also learned and improved my skills with the MEAN stack, including MongoDB, Express, Angular, Node.js, and Mongoose. I also learned how to create and test API endpoints, work with JSON, use Angular components and services, connect an app to a database, and add JWT authentication to protect the admin side of the app. I also improved my troubleshooting and debugging skills by working through problems across different parts of the app. I am now using what I learned in this course to start a personal software development project, which will give me an opportunity to continue practicing these skills and build something of my own.
