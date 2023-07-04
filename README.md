# OAuth2 Project

Simple Node/Express application to sing up using OAuth 2.0 with a GitHub account.

## Configuration
To succesfully connect the app with GitHub, you must need to register an OAuth application in GitHub to obtain
the ClientID and Client Secret and add an .env file with this keys.

GITHUB_CLIENT_ID=<GITHUB_CLIENT_ID>
GITHUB_CLIENT_SECRET=<GITHUB_CLIENT_SECRET>

## Running the app
To run locally, run `npm install`, then `npm start`

Once the app is running locally, you can access the API at `http://localhost:3000/`

Log in to the app using your GitHub account. When you are logged in, you can go to the "/account" page and see details from your GitHub account displayed.

In this project, we implemented OAuth using the express-session module to manage user sessions authenticated using the passport module. We configured passport using the credentials from GitHub and implemented the URL routes for authentication. Finally, we implemented a middleware function to protect the route.

## Resources
- NodeJS
- Express
- Express-sessions
- Passport
- OAuth 2.0
- dotenv

