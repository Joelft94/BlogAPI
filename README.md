# Blog API
This project consists of a blog-like API with two servers running on different ports.
The main server (running on port 3000) handles the frontend and routes for rendering pages, while the secondary server (running on port 4000) provides a RESTful API for managing blog posts.

# Installation

### Clone the repository:
git clone https://github.com/yourusername/blog-api.git

### Install dependencies
npm i

### Start both servers:
Open two separate terminal tabs and run both index.js and server.js


# Usage
## Frontend Server (Port 3000)

The frontend server serves static files and renders pages using EJS templates.
It fetches data from the backend server and displays it on the main page.

## Backend Server (Port 4000)
The backend server provides RESTful API endpoints for managing blog posts.
It uses an in-memory data store to hold the blog posts.

# API Endpoints

Backend Server (Port 4000)

## Get All Posts

Endpoint: GET /posts
Description: Retrieve all blog posts.
Response: JSON array of posts.

## Get a Specific Post

Endpoint: GET /posts/:id
Description: Retrieve a single post by its ID.
Response: JSON object of the post.

## Create a New Post

Endpoint: POST /posts
Description: Create a new blog post.
Request Body:

![image](https://github.com/Joelft94/BlogAPI/assets/107083554/b3cffcd4-68c4-4ef6-9764-68027e1f9dd0)

Response: JSON object of the created post.

# Update a Post

Endpoint: PATCH /posts/:id
Description: Partially update a post by its ID.
Request Body: Can include any of the post properties.
Response: JSON object of the updated post.

# Delete a Post

Endpoint: DELETE /posts/:id
Description: Delete a post by its ID.
Response: JSON object with a success message.




