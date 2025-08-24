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

<h3>Hosting Capabilities</h3>

Logged-in users (hosts) can create new listings with detailed information and images.

<h3>Review System</h3>

Users can leave reviews on stay experiences.

Only review authors can delete their own reviews; others can only read them.

<h3>Responsive UI/UX</h3>

Modern, mobile-friendly interface using Bootstrap components.

Project Structure
Folder / File	Description

<h5>controllers/</h5> -	Backend logic for routes and functionality.

<h5>init/	Initialization</h5> - scripts/configurations.

<h5>models/</h5> - Mongoose schemas/models for data entities (users, listings, reviews, etc.).

<h5>public/</h5> -	Static assets (images, styles, client-side scripts).

<h5>routes/</h5> -	RESTful API endpoint definitions (users, listings, reviews, etc.).

<h5>utils/</h5> - 	Utility functions and helpers.

<h5>views/</h5> -	Templated pages rendered for endpoints (login, signup, listings, details, etc.).

<h5>app.js</h5> -	Main application entry point, server configuration.

<h5>cloudConfig.js</h5> -	Configuration for cloud services (e.g. image upload).

<h5>middleware.js</h5> -	Custom Express middleware for error handling, authorization, etc.

<h5>package.json</h5> -	Project dependencies and scripts.

<h5>package-lock.json</h5> -	Exact dependency versions.

<h5>schema.js</h5> -	Additional DB schemas.

<h1>Application Screenshots</h1>

<h4>Login/Signup Pages</h4>: Secure authentication flows for both new and returning users.

<img width="1920" height="1020" alt="Screenshot 2025-08-24 140710" src="https://github.com/user-attachments/assets/52bdfc4b-726b-46bb-9c9e-4bcd6fdec504" />

<img width="1920" height="1020" alt="Screenshot 2025-08-24 140722" src="https://github.com/user-attachments/assets/58139ec1-a374-4811-ac5c-a4c65bc6823a" />

<h4>Listings and Explore Pages</h4>: Browse all available properties, filter by categories, toggle tax visibility.

<img width="1920" height="1020" alt="Screenshot 2025-08-24 140908" src="https://github.com/user-attachments/assets/73e30d86-f9ef-4238-a2e9-cd5622122b35" />

<img width="1920" height="1020" alt="Screenshot 2025-08-24 140927" src="https://github.com/user-attachments/assets/91f8263a-a455-48b0-915d-fc9d3105aefe" />

<img width="1920" height="1020" alt="Screenshot 2025-08-24 140935" src="https://github.com/user-attachments/assets/14a9f7fb-fa45-4caa-bc83-459ca18d71a3" />

<img width="1920" height="1020" alt="Screenshot 2025-08-24 140945" src="https://github.com/user-attachments/assets/c7f19704-c1a2-4b3a-bc46-63d0e74121f2" />

<h4>Property Details</h4>: View expanded details and reviews for a selected listing.

<h5>If Listing is Created by him/her, edit and delete option is visible</h5>

<img width="1920" height="1020" alt="Screenshot 2025-08-24 141226" src="https://github.com/user-attachments/assets/63a76828-d506-4c59-a85b-1bebf6c45fca" />

<h5>If him/her just came to view listing and their details</h5>

<img width="1920" height="1020" alt="Screenshot 2025-08-24 141206" src="https://github.com/user-attachments/assets/cac2a929-2439-40b8-ab0a-d66f48fef275" />

<h4>Reviews Schreenshot</h4>

<img width="1920" height="1020" alt="Screenshot 2025-08-24 141843" src="https://github.com/user-attachments/assets/4f058919-77ce-4983-9ba5-0074729d5fe9" />

<h4>Edit Page: Edit of Listing</h4>

<img width="1920" height="1020" alt="Screenshot 2025-08-24 141958" src="https://github.com/user-attachments/assets/adf370a0-057a-431b-9e95-6ba9784c681e" />

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
