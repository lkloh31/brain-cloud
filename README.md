# Brain Cloud (MEV)

**MEV** (short for “My Everyday View”) is a personal curation platform designed to centralize your daily online interactions — from news, weather, and finance to maps, journals, and games — all in one clean interface.
It helps users record experiences, organize travel and location-based information, and optionally enjoy small interactive features to encourage daily check-ins.

---

## Table of Contents
1. [Features](#features)
2. [Tech Stack](#tech-stack)
3. [Feature Breakdown & Contributors](#feature-breakdown--contributors)

---

## Features

### Primary Features
- **Daily Dose Dashboard**: Aggregates key information such as news, weather, and exchange rates with customizable ordering.
- **Map Interface**: Allows users to pin and filter locations with notes, ratings, and categories.
- **Journal Page**: Enables daily text entries with calendar integration and tagging system.
- **Authentication**: Secure registration and login functionality with JWT tokens.
- **Brain Games**: Collection of interactive games including Memory Match, Reaction Test, Tic-Tac-Toe, Sudoku, and Simon.
- **Responsive UI**: Works across desktop and mobile.

---

## Tech Stack
**Frontend**: React 19, TailwindCSS, Framer Motion, Mapbox GL JS, React Router, React Calendar  
**Backend**: Node.js, Express.js, PostgreSQL, JWT Authentication, bcrypt 
**External APIs**: NewsAPI, Open-Meteo Weather, ExchangeRate API, Mapbox  
**Version Control**: GitHub

---

## Feature Breakdown & Contributors
*(Features listed with the primary implementer)*

- **User Authentication Backend**  
  - Registration and login API endpoints with geolocation detection  
  - JWT token generation and verification middleware 
  - Password hashing with bcrypt and secure storage
  - User profile management and location tracking
  - **Implemented by:** [Fabiana, Princy]
    
- **User Authentication Frontend**  
  - Register/Login pages with form validation and error handling 
  - Integration with backend auth API using React Context  
  - JWT token storage in localStorage and protected routes
  - Responsive auth forms with loading states
  - **Implemented by:** [Lokkee, Joshua]

- **General Theme & Layout**  
  - Home page styling with MEV branding and welcome sections
  - Fixed navbar with responsive hamburger menu navigation
  - Overall Courier New typography and clean design system 
  - Mobile-first responsive design across all components
  - **Implemented by:** [Lokkee]
    
- **Daily Dose Dashboard**  
  - Drag-and-drop reorderable links using Framer Motion
  - News aggregation with NewsAPI, infinite scroll, and favorites system
  - Weather integration with Open-Meteo API and location search
  - Currency exchange rates with real-time conversion and favorites
  - Local storage for user preferences and customization
  - **Implemented by:** [Fabiana, Princy]

- **Map Page**  
  - Mapbox integration with interactive pin dropping and navigation
  - Location categorization (been there/want to go) with custom markers
  - Reverse geocoding and location details (notes, ratings, dates)
  - Sidebar navigation with click-to-fly functionality
  - CRUD operations for location management
  - **Implemented by:** [Lokkee]

- **Journal Page**  
  - React Calendar integration for date-based entry navigation 
  - Create/edit/delete journal entries with title, content, and tags  
  - Multiple entries per day with visual calendar markers
  - Form validation and responsive layout
  - PostgreSQL backend integration for persistent storage
  - **Implemented by:** [Joshua]

- **Games Collection**  
  - Collection of interactive games including Memory Match, Reaction Test, Tic-Tac-Toe, Sudoku, and Simon. 
  - Score persistence and leaderboard functionality
  - **Implemented by:** [Joseph]








































