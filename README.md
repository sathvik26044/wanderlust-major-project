# wanderlust-major-project
# Wanderlust
<h1>Overview</h1>
Wanderlust is a full-stack web application inspired by Airbnb, built to help users explore and book travel accommodations. This project leverages modern web development tools and follows the Model-View-Controller (MVC) architecture with a RESTful API design. Wanderlust demonstrates comprehensive user authentication, robust authorization, dynamic listings, and a visually engaging UI.

<h1>Technologies Used</h1>
Frontend: HTML, CSS, JavaScript, Bootstrap

Backend: Node.js, Express.js

Database: MongoDB (with Mongoose)

Architecture: MVC

Other: Font Awesome, various npm packages, cloud storage for images

<h1>Key Features</h1>
<h3>User Authentication & Authorization</h3>

Secure login/signup allows users to create accounts and access the application.

Passwords securely handled; sessions managed for protected routes.

<h3>Role-based Authorization</h3>

Listing Owners: Only the user who created a listing can edit or delete their property.

Reviews: Only the user who wrote a review is authorized to delete that review; others can view but not remove reviews.

All users can browse listings, search destinations, and view reviews and details.

<h3>Property Listings</h3>

Explore a marketplace of travel accommodations with high-quality images, location, price, and owner details.

Dynamic listing cards display: name, image, price/night, GST toggle for showing price with/without taxes.

Detailed page for each property includes a description, owner, price, location (city/country), and reviews.

<h3>Search & Explore</h3>

Search bar for destinations.

Navigation for trending locations, room categories, iconic cities.

Hosting Capabilities

Logged-in users (hosts) can create new listings with detailed information and images.

Review System

Users can leave reviews on stay experiences.

Only review authors can delete their own reviews; others can only read them.

Responsive UI/UX

Modern, mobile-friendly interface using Bootstrap components.

Project Structure
Folder / File	Description
controllers/	Backend logic for routes and functionality.
init/	Initialization scripts/configurations.
models/	Mongoose schemas/models for data entities (users, listings, reviews, etc.).
public/	Static assets (images, styles, client-side scripts).
routes/	RESTful API endpoint definitions (users, listings, reviews, etc.).
utils/	Utility functions and helpers.
views/	Templated pages rendered for endpoints (login, signup, listings, details, etc.).
app.js	Main application entry point, server configuration.
cloudConfig.js	Configuration for cloud services (e.g. image upload).
middleware.js	Custom Express middleware for error handling, authorization, etc.
package.json	Project dependencies and scripts.
package-lock.json	Exact dependency versions.
schema.js	Additional DB schemas.
Application Screens
Login/Signup Pages: Secure authentication flows for both new and returning users.

![Login Screenshot]

![Signup Screenshot]

Listings and Explore Pages: Browse all available properties, filter by categories, toggle tax visibility.

![Listings Screenshot]

![Explore Screenshot]

Property Details: View expanded details and reviews for a selected listing.

![Listing Details Screenshot]

<h3>How to Run</h3>
Clone the repository:

bash
git clone https://github.com/sathvik26044/wanderlust-major-project.git
cd wanderlust-major-project
Install dependencies:

bash
npm install
Configure Environment Variables:

Create a .env file in the root directory, set up your MongoDB URI, session secret, and other required variables.

Start the development server:

bash
npm start
Default: localhost:8080

Why Wanderlust?
This project was developed as a full-stack learning challenge for mastering Node.js, Express.js, MongoDB, RESTful API design, MVC architecture, and web security. It provides real-world scenarios for authentication, authorization, data modeling, and error-solving, making it an excellent reference for debugging and building scalable web apps.
