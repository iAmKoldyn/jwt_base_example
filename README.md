# Golang JWT Authentication
# Run
``docker-compose up -d``  
Run the command `go install`  
Start the Fiber HTTP server and migrate the GORM model to the Postgres database by running `go run main.go`.  
To test the authentication flow of the Fiber API, import the file `Golang_GORM.postman_collection.json`.

## Steps

- Set up the Golang Project
- Setup PostgreSQL and pgAdmin with Docker
- Create the GORM Model
- Database Migration with GORM
    - Load the Environment Variables with Viper
    - Create the Database Pool with GORM
    - Migrate the GORM Model to the Database
- Create the JWT Authentication Controllers
    - SignUp User Fiber Context Handler
    - SignIn User Fiber Context Handler
    - Logout User Fiber Context Handler
- Get the Authenticated User
- Create the JWT Middleware Guard
- Register the Routes and Add CORS
- Testing the JWT Authentication Flow
    - Register a New Account
    - Log into the Account
    - Access Protected Routes
    - Logout from the API
