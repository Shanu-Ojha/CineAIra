# MovieFlix Frontend

A modern movie discovery application built with React, Tailwind CSS, and GSAP animations.

## Features

- **Home Page**: Displays Now Playing, Trending, Popular, and Top Rated movies
- **Search Page**: Search for movies and get AI-powered recommendations
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Smooth Animations**: GSAP-powered animations for a premium feel
- **Loading States**: Skeleton loaders and loading indicators
- **Netflix-like UI**: Modern, dark theme with movie poster cards

## Tech Stack

- React 19
- React Router DOM
- Tailwind CSS
- GSAP (GreenSock Animation Platform)
- Axios for API calls

## Getting Started

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open your browser and navigate to `http://localhost:5173`

## Backend Requirements

Make sure your backend server is running on `http://localhost:3001` with the following endpoints:

- `GET /api/tmdb/nowplaying` - Now playing movies
- `GET /api/tmdb/popular` - Popular movies  
- `GET /api/tmdb/toprated` - Top rated movies
- `GET /api/tmdb/trending` - Trending movies
- `GET /api/tmdb/search?query=` - Search movies
- `GET /api/ai/recommend?query=` - AI recommendations

## Project Structure

```
src/
├── components/
│   ├── Navbar.jsx          # Navigation with search
│   ├── HeroSection.jsx     # Hero banner with featured movie
│   ├── MovieRow.jsx        # Horizontal movie row
│   ├── MovieCard.jsx       # Individual movie card
│   ├── SearchResults.jsx   # Search results display
│   └── SkeletonLoader.jsx  # Loading skeleton
├── pages/
│   ├── Home.jsx            # Home page
│   └── Search.jsx          # Search page
├── App.jsx                 # Main app component
├── index.css               # Global styles
└── main.jsx                # Entry point
```

## Features in Detail

### Home Page
- Hero section with rotating featured movies
- Movie rows for different categories
- Smooth scroll animations
- Responsive grid layout

### Search Page
- Real-time search functionality
- Skeleton loading states during AI recommendation processing
- Separate sections for search results and AI recommendations
- Error handling and retry functionality

### Animations
- GSAP-powered smooth transitions
- Hover effects on movie cards
- Loading animations
- Staggered content reveals

## Styling

The application uses Tailwind CSS with custom utilities for:
- Netflix-like dark theme
- Responsive design
- Custom scrollbars
- Smooth transitions
- Loading animations#
