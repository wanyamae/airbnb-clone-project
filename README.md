# airbnb-clone-project

This is a project where, in 4 months, we will create a functional airbnb booking and management website.
I will be applying both front end and back end programming in this project, using different languages for different purposes.

# Team Roles
## Product Owner
 The product owner will have the vision for the project, and ensure that the final product meets the user requirements.

## Project Manager
The project manager will ensure that the project runs as per the plan, ensuring we do not fall back on the set timelines.

## Backend Developer
The backend developer will work to ensure that the software architect is current and up to date with the current standards, they will ensure that APIs are developed that ensure communication with the database, such that the data is secure and accessible when needed.

## Frontend Developer
The frontend developer will work to ensure that the software is practical and that the visuals are appealing to the users, maximizing the user interaction with the software.

# Technology Stack
## Django
A high-level Python web framework that encourages rapid development and clean, pragmatic design for building APIs. It handles backend logic, routing, authentication, and database operations.

## Python
A versatile, high-level programming language used for server-side development, scripting, and data processing. Django is built with Python.

## Vite + Vue:

### Vite
A fast frontend build tool that provides instant server start and lightning-fast hot module replacement for modern web projects.
### Vue
A progressive JavaScript framework for building user interfaces, especially single-page applications (SPAs).
HTML: The standard markup language for creating web pages and structuring content on the web.

## CSS
A stylesheet language used to describe the presentation and layout of HTML elements on a web page.

## SQL
A domain-specific language used to manage and query relational databases, storing and retrieving application data.

# Database Design
The Airbnb clone project will have tables such as Users, Listings, Bookings and Reviews

## Important Fields (across main tables)
- User ID (in Users table): Uniquely identifies each user.
- Listing ID (in Listings table): Uniquely identifies each property/listing.
- Booking ID (in Bookings table): Uniquely identifies each booking/reservation.
- Review ID (in Reviews table): Uniquely identifies each review.

## Relationships
- Users can create multiple Listings (one-to-many).
- Users can make multiple Bookings (one-to-many).
- Listings can have multiple Bookings (one-to-many).
- Users can leave multiple Reviews for Listings (one-to-many).
- Bookings and Reviews are linked to both Users and Listings via foreign keys.

## Example fields
- Users: `user_id, name, email, password`
- Listings: `listing_id, title, description, price, user_id (owner)`
- Bookings: `booking_id, user_id, listing_id, start_date, end_date`
- Reviews: `review_id, user_id, listing_id, rating, comment`

# Feature Breakdown

## User Management
Allows users to register, log in, and manage their profiles securely. This feature ensures that only authenticated users can access certain functionalities, such as booking properties or leaving reviews.

## Property Management
Enables property owners to list new properties, update details, and manage availability. This feature is essential for keeping the platform’s listings up-to-date and providing users with accurate information.

## Booking System
Lets users search for available properties, make reservations, and manage their bookings. This system handles date selection, availability checks, and booking confirmations, ensuring a smooth reservation process.

## Review and Rating System
Allows guests to leave reviews and ratings for properties they have stayed in. This feature helps maintain trust and transparency within the platform by providing feedback for future guests and property owners.

## Search and Filtering
Provides users with the ability to search for properties based on location, price, amenities, and other criteria. This makes it easier for users to find listings that match their preferences.

## Messaging System
Facilitates communication between guests and property owners through a built-in messaging platform. This ensures that users can ask questions and clarify details before making a booking.