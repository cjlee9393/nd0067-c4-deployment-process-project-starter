# Hosting a Full-Stack Application

## A brief description of the project

The project application, Udagram - an Image Filtering application, allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering service. It has two components:

Frontend - Angular web application built with Ionic framework
Backend RESTful API - Node-Typescript application

The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.

## Link to working front-end application

[Link to front-end application](http://myawsbucket-2028006.s3-website-us-west-1.amazonaws.com/)

## How to set up the project

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. 

2. In AWS, provision a s3 bucket for hosting the uploaded files.

3. Use root level package.json to install dependencies in the frontend app
    ```bash
    echo "NODE --version" 
    echo $(node --version)
    echo "NPM --version" 
    echo $(npm --version)
    npm run frontend:install
    ```
4. Install dependencies in the the backend API        
    ```bash
    npm run api:install
    ```
5. Lint the frontend
    ```bash
    npm run frontend:lint
    ```

6. Build the frontend app
    ```bash
    npm uninstall typescript
    npm install typescript@3.5.3
    npm run frontend:build
    ```
7. Build the backend API      
    ```
    apt-get update
    apt-get install zip
    npm run api:build
    ```
8. Deploy the application
    ```
    npm run deploy
    ```

## License

[License](LICENSE.txt)

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License