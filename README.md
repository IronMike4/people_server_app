# People Server App

This project is a simple Express.js application that demonstrates basic CRUD operations using a JSON file (`people.json`) for data storage. The app allows you to add, update, check, and delete people from the `people.json` file through a RESTful API.

## Features

- **Add Person**: Add a new person to the `people.json` file using a POST request.
- **Update Person**: Update an existing person's name using a PUT request.
- **Check Person**: Verify if a person exists in the `people.json` file using a GET request.
- **Delete Person**: Remove a person from the `people.json` file using a DELETE request.
- **Greet**: A simple greeting endpoint that returns "Hello world" or a personalized greeting.

## Prerequisites

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

## Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/IronMike4/people_server_app.git
   cd people_server_app

2. **Install dependencies:**

   ```bash
   npm install

   ```

3. **Start the development server:**

   ```bash
   npm start

   ```

4. **Open the project in your browser:**
   Navigate to http://localhost:3000 to view the Express App.

## API Endpoints
1. **Greet**
 - GET /greet?name=yourName:
   - Greets the user by name. If no name is provided, it returns "Hello world".
   - Example: http://localhost:3000/greet?name=Jack
2. **Add Person**
 - POST /person?name=yourName:
   - Adds a new person to the people.json file.
   - Example: http://localhost:3000/person?name=Jack
3. **Update Person**
 - PUT /person?name=oldName&newName=newName:
   - Updates an existing person's name in the people.json file.
   - Example: http://localhost:3000/person?name=Jack&newName=Samantha
4. **Check Person**
 - GET /person?name=yourName:
   - Checks if a person exists in the people.json file.
   - Example: http://localhost:3000/person?name=Jack
5. **Delete Person**
 - DELETE /person?name=yourName:
   - Deletes a person from the people.json file.
   - Example: http://localhost:3000/person?name=Jack
6. **Error Handling**
 - If a person does not exist or if the route is incorrect, appropriate error messages are returned.

## Testing with Postman
You can use Postman to test the API:

1. **POST Request: Add a new person named Jack.**
 - URL: http://localhost:3000/person?name=Jack
 - Method: POST

2. **PUT Request: Update Jack to Samantha.**
 - URL: http://localhost:3000/person?name=Jack&newName=Samantha
 - Method: PUT

3. **GET Request: Check if Samantha exists.**
 - URL: http://localhost:3000/person?name=Samantha
 - Method: GET

4. **DELETE Request: Delete Samantha.**
 - URL: http://localhost:3000/person?name=Samantha
 - Method: DELETE

 ## Contact

[Michael Mahachi](mikhach@gmail.com)

## References

HyperionDev React - Express - Web Applications Task (PDF)