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