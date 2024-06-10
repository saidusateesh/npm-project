#################### npm-project##################################

# Simple Node JS React NPM App with Jenkins and Docker

This project demonstrates the integration of Jenkins for continuous integration and Docker for containerization. The following steps outline the implementation:

## Jenkins Integration
- Added a `Jenkinsfile` to install npm packages, build the app, and serve it locally on port 3004.
- Modified the React app to include annotations of the npm packages used and a button to trigger the build process via Jenkins.

## Docker Integration
- Added Dockerfiles for Postgres, Redis, MongoDB, and Mongo-Express.
- Created a `Jenkinsfile.docker` to pull, build, and run these services as Docker containers locally.
- Optionally set up a local Docker registry to host these images securely.

### Accessing the Services
- The Node.js app is accessible on [http://localhost:3004](http://localhost:3004).
- The Jenkins server is accessible on [http://localhost:3000](http://localhost:3000).
- Mongo-Express is accessible on [http://localhost:8081](http://localhost:8081).

### Credentials
- MongoDB and Mongo-Express:
  - Username: ati
  - Password: ati1234

### Build and Run
To build and run the Docker containers, execute the Jenkins pipeline defined in `Jenkinsfile.docker`.

## Repository Link
Link to the repository: https://github.com/saidusateesh/npm-project
