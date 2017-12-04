## Project

Build a server-rendered full-stack app

### Task

- Build an app using the Express framework.
- Use a PostgreSQL database to store and retrieve your data.
- Use the retrieved data to populate a Handlebars template for _server-side_ rendering to be displayed on the front-end.

And conduct a technical spike (see below) in order to either:
  - Use promises throughout your application

Or:
  - Implement session management using middleware

### Goals

The primary aim of this project is to get comfortable with setting up an Express server and to discover the awesomeness of Handlebars! Spend time considering how to format your layouts, partials and helper functions.

Previous cohorts have built apps where users can share, for example, blog posts, jokes, photos etc. But the app can be about anything as long as you are covering project's technology tasks and goals.

### What's also important:

- Include tests and set up code coverage.
- Use Heroku or a similar service to host the app and the database.
- Try to include ES6 syntax on the server.

### Technical Spikes

**Promises**:
  - In order to get promises back from queries to your PostgresSQL database, you might consider using the [pg-promise](https://www.npmjs.com/package/pg-promise) module.
  - If your app makes api calls from the server, you could consider using the [request-promise-native](https://www.npmjs.com/package/request-promise-native) module.

**Middleware for Session Management**:

There are [two main middleware](https://expressjs.com/en/advanced/best-practice-security.html#use-cookies-securely) used with express for session management:
- [cookie-session](https://www.npmjs.com/package/cookie-session): stateless session management with signed cookies; session data is stored in the cookie.
- [express-session](https://www.npmjs.com/package/express-session): session data is stored server-side. For production a session store needs to be setup.

