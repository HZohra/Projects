# BiteWise — Dietary Restriction Meal Matcher

BiteWise is a full-stack web application that helps users discover allergy-safe
recipes and nearby restaurants based on dietary restrictions and allergens.
The platform combines recipe search, nutrition data, user profiles, and an
AI-powered chatbot to support healthier food choices.

This project was developed as part of a **CP317 Software Engineering group project**.

---

## Tech Stack

**Frontend**
- React
- Vite
- Tailwind CSS

**Backend**
- Node.js
- Express.js
- MongoDB

**Authentication**
- JWT (JSON Web Tokens)

**APIs**
- Edamam Recipe & Nutrition API
- OpenStreetMap / Overpass API

---

## Key Features

### User Authentication & Profiles
- Secure user registration and login using JWT
- Password reset functionality with token-based verification
- User profile management (dietary preferences, allergens, cooking time limits)
- Protected routes for personalized content

### Recipe Search & Management
- Recipe search with nutrition data using the Edamam API
- Multi-filter search combining dietary restrictions and keywords
- User-created recipes with full CRUD functionality
- Hybrid recipe database (API recipes + user-submitted recipes)
- Detailed recipe view with ingredients, instructions, and nutrition labels

### AI-Powered Chatbot
- Natural language recipe search (e.g. “quick vegan dinner ideas”)
- Intent and entity detection for diets, ingredients, and preferences
- Allergen substitution suggestions
- Context-aware responses with formatted recommendations
- Chat history and interactive UI

### Restaurant Finder
- Location-based restaurant discovery
- Radius filtering using latitude and longitude
- Nearby restaurant information via OpenStreetMap / Overpass API

---

## Project Structure

```txt
CP317_Group2_FinalProject/
├── backend/
│   └── bitewise-backend/
│       ├── src/
│       │   ├── app.js                 # Express server entry
│       │   ├── config/                # Database & API configuration
│       │   ├── middleware/            # Authentication middleware
│       │   ├── models/                # MongoDB schemas
│       │   ├── routes/                # API routes
│       │   ├── services/              # Business logic & chatbot logic
│       │   └── utils/                 # Helper functions
│       └── package.json
├── frontend/
│   ├── src/
│   │   ├── pages/                     # Application pages
│   │   ├── components/                # Reusable UI components
│   │   ├── context/                   # Auth & chat contexts
│   │   ├── api/                       # API calls
│   │   └── services/                  # Frontend utilities
│   └── package.json
└── README.md

🔗 Full code repository:
https://github.com/HZohra/Bitewise-fullstack
