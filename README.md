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

# API Security
 API security is needed to protect sensitive user data, prevent anauthorized access and ensure the integrity of the platform. Several key security measures will be implemented including:
 - Authentication to ensure tha only regostered users can access protected endpoints by verifying their identities using secure login mechanisms such as Json Web Tokens.
 - Authorization will ensure a role based access controls to ensure that users can only perform activities permitted for their role.
 - Rate Limiting will limit the number of requests a user or IP address can make in a given time frame. This will prevent abuse, such as brute-force attacks or denial-of-service attempts, ensuring the API remains available and responsive.
 - Data validation will ensure that all data is validated and sanitized to prevent commmon vulnerabilities such SQL injections anc Cross site scripting (XSS).
 - Secure payment will protect sensitive payment information using secure PCI-compliant third-party services to protect user's financial data and reduce the risk of fraud.

 # CI/CD Pipeline
 CI/CD (Continuous Integration and Continuous Deployment) pipelines automate the process of building, testing, and deploying code changes. This ensures that new features and bug fixes are integrated smoothly, tested automatically, and deployed quickly, reducing manual errors and improving development efficiency.

Implementing a CI/CD pipeline is important for maintaining code quality, catching issues early, and delivering updates to users faster. For this project, tools such as **GitHub Actions** can be used to automate testing and deployment workflows, while **Docker** can help create consistent environments for development and production.

By using CI/CD, the project benefits from faster feedback, reliable releases, and a more streamlined development process.

# UI/UX Design Planning

## Design Goals
The main goals for the UI/UX design are to create an intuitive, visually appealing, and responsive interface that makes it easy for users to browse, book, and manage properties. The design will focus on simplicity, accessibility, and seamless navigation to enhance the overall user experience.

## Key Features to Implement
- Clear navigation and layout for easy access to all sections
- Responsive design for optimal viewing on all devices
- Consistent branding and visual elements
- Fast and simple booking process
- User feedback through notifications and confirmations

## Primary Pages

| Page Name                | Description                                                                                   |
|--------------------------|-----------------------------------------------------------------------------------------------|
| Property Listing View    | Displays a list of available properties with filters and search options for easy browsing.    |
| Listing Detailed View    | Shows detailed information about a selected property, including images, amenities, and reviews.|
| Simple Checkout View     | Provides a streamlined booking form where users can review details and complete their booking. |

## Importance of User-Friendly Design
A user-friendly design is crucial in a booking system to ensure users can quickly find and reserve properties without confusion or frustration. Good UI/UX increases user satisfaction, reduces errors, and encourages repeat usage, which is essential for the success of the platform.