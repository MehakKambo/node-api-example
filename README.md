# Subscriber Management API
This is a simple **RESTful API** for managing subscribers built using **NODE JS** and **MongoDB**. It allows you to perform CRUD operations (Create, Read, Update, Delete) on subscriber records.

# Getting Started
## Prerequisites
- Node.js and npm (Node Package Manager)
- MongoDB

## Installation
1. Clone the repository:
``` bash
git clone https://github.com/yourusername/Subscriber-Management-API.git 
cd Subscriber-Management-API
```
2. Install dependencies:

```bash
npm install
```

3. Start the server:

```bash
npm run devStart
```
The server will start on http://localhost:3000.

# Usage
## API Endpoints
| Methods | Endpoints                          | Access  | Description                                    |
| ------- | ---------------------------------- | ------- | -----------------------------------------------|
| GET     | /subscribers                       | Public  | Get a list of all subscribers                  |
| GET     | /subscribers/:id                   | Public  | Get details of a specific subscriber by ID     |  
| POST    | /subscribers                       | Public  | Create a new subscriber                        |
| PATCH   | /subscribers/:id                   | Private | Update details of a specific subscriber by ID  |
| DELETE  | /subscribers/:id                   | Private | Delete a subscriber by ID                      |


# Examples
- To get all subscribers: `GET http://localhost:3000/subscribers`
- To get a specific subscriber: `GET http://localhost:3000/subscribers/123` where `123` is the id
- To create a new subscriber:
``` bash
POST http://localhost:3000/subscribers
Body: {
  "name": "John Doe",
  "subscribedToChannel": "MyChannel"
}
```
- To update a subscriber: 
``` bash
PATCH http://localhost:3000/subscribers/123
Body: {
  "name": "Updated Username"
  "subscribedToChannel": "Updated Channel"
}
```

- To delete a subscriber: `DELETE http://localhost:3000/subscribers/123`

# Contributing
Contributions are welcome! If you have any enhancements, bug fixes, or suggestions, feel free to submit a pull request.

