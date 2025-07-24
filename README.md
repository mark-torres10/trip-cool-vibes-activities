# Road Trip Planner 🗺️

A Next.js web application that transforms your Google Maps route into an adventure by discovering amazing stops along the way. Perfect for long road trips where you want to break up the journey with interesting restaurants, scenic viewpoints, and local attractions.

## 🎯 Purpose

Planning a 10-hour road trip? This app helps you:
- **Paste your Google Maps route** and get intelligent stop suggestions
- **Set your departure time** and preferred stop intervals (every 2-4 hours)
- **Discover local gems** - restaurants, attractions, scenic spots along your exact route
- **Export a new itinerary** back to Google Maps with all your selected stops included

## ✨ Key Features

### Current Vision
- **Smart Route Analysis**: Parses Google Maps URLs and calculates optimal stop points
- **Time-Based Suggestions**: Find places to visit based on when you'll arrive (perfect for meal times!)
- **Curated Recommendations**: High-quality restaurants, attractions, and viewpoints near your route
- **Seamless Export**: Generate a new Google Maps itinerary with all selected stops
- **Mobile-First**: Designed for use during your actual trip

### Example Use Case
> "I'm leaving at 9 AM for a 10-hour drive. I want to stop for lunch around 12-2 PM and dinner around 6-8 PM, plus maybe a scenic viewpoint in between. Show me what's along my route!"

## 🛠️ Technology Stack

- **Framework**: Next.js 14 with App Router
- **Deployment**: Vercel
- **Styling**: Tailwind CSS
- **APIs**: Google Maps Platform (Maps, Places, Routes)
- **Database**: PostgreSQL (Vercel Postgres)
- **Authentication**: NextAuth.js

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- Google Cloud Platform account with Maps API access
- Vercel account (for deployment)

### Development Setup
```bash
# Clone the repository
git clone <repository-url>
cd road-trip-planner

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Add your Google Maps API keys

# Run development server
npm run dev
```

Visit `http://localhost:3000` to see the application.

## 📋 Implementation Plan

This project is built iteratively with clear milestones:

1. **Foundation** - Basic Next.js setup and Vercel deployment
2. **Maps Integration** - Google Maps API integration and URL parsing
3. **Route Analysis** - Calculate stop points and travel times
4. **Places Discovery** - Find and rank nearby attractions
5. **User Interface** - Interactive stop selection and customization
6. **Export Feature** - Generate new Google Maps itineraries
7. **Enhancement** - Mobile optimization and performance
8. **Advanced Features** - Templates, real-time updates, and filtering

See [SPECS.md](./SPECS.md) for detailed implementation specifications.

## 🎨 Design Philosophy

**Simple but Powerful**: The core workflow should be:
1. Paste Google Maps link
2. Set departure time and preferences  
3. Browse suggestions
4. Export new itinerary

**Mobile-First**: Designed for use during actual trips on mobile devices

**Quality over Quantity**: Better to suggest 3 amazing stops than 20 mediocre ones

## 📊 MVP Scope

The first version focuses on:
- ✅ Basic route parsing and visualization
- ✅ Time-based stop calculation
- ✅ Restaurant and attraction discovery
- ✅ Simple export to Google Maps
- ✅ Mobile-responsive design

Future versions will add trip saving, user accounts, templates, and advanced filtering.

## 🔑 Required APIs

- **Google Maps JavaScript API**: For map display and route visualization
- **Google Places API**: For finding restaurants and attractions
- **Google Routes API**: For detailed route information and timing
- **Google Maps URLs API**: For generating shareable itineraries

## 🤝 Contributing

This project follows a milestone-based development approach. See [SPECS.md](./SPECS.md) for current tickets and implementation details.

## 📱 Deployment

Designed for easy deployment on Vercel:
```bash
# Deploy to Vercel
vercel --prod
```

Environment variables needed:
- `GOOGLE_MAPS_API_KEY`
- `NEXT_PUBLIC_GOOGLE_MAPS_API_KEY`
- `DATABASE_URL` (for user features)

## 🗺️ Roadmap

- **Phase 1**: Core functionality (MVP)
- **Phase 2**: User accounts and trip saving
- **Phase 3**: Advanced filtering and preferences
- **Phase 4**: Collaborative planning and sharing
- **Phase 5**: Mobile app and offline features

---

*Turn your road trip into an adventure - one stop at a time!* 🚗✨
