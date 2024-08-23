# Blog Node.js

Welcome to the **Blog Node.js** project! This is a simple blog application built with Node.js, Express, and MongoDB. It features user authentication, post creation, editing, and deletion, and a search functionality.

## Table of Contents

- Features
- Installation
- Usage
- Routes
- Environment Variables

## Features

- User authentication (login, logout)
- Create, edit, and delete blog posts
- Search functionality
- Admin dashboard
- Responsive design

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/lobzhanidzee/blog-NodeJs.git
   cd blog-nodejs
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

3. Create a `.env` file in the root directory and add the following environment variables:

   ```env
   JWT_SECRET=your_jwt_secret
   MONGO_URI=your_mongodb_uri
   ```

4. Start the application:
   ```sh
   npm run dev
   ```

## Usage

- Visit `http://localhost:8080` to view the blog.
- Visit `http://localhost:8080/admin` to access the admin login page.
- After logging in, you can access the admin dashboard to manage posts.

## Routes

### Public Routes

- `GET /` - Home page
- `GET /about` - About page
- `GET /contact` - Contact page
- `POST /search` - Search posts

### Admin Routes

- `GET /admin` - Admin login page
- `POST /admin` - Admin login
- `GET /dashboard` - Admin dashboard
- `GET /add-post` - Create new post page
- `POST /add-post` - Create new post
- `GET /edit-post/:id` - Edit post page
- `PUT /edit-post/:id` - Edit post
- `DELETE /delete-post/:id` - Delete post
- `GET /logout` - Logout

## Environment Variables

- `JWT_SECRET` - Secret key for JWT
- `MONGO_URI` - MongoDB connection URI
