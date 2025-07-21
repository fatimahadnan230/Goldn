# FashioNova - AI Fashion Image Generator

## Overview

FashioNova is a React-based AI fashion image generator that allows users to create, save, and share fashion designs. The application features a modern, responsive web interface with a lavender and pink gradient design theme. It's built as a single-page application (SPA) optimized for GitHub Pages deployment with fallback support for client-side routing.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with modern hooks and functional components
- **Build System**: Vite (indicated by the bundled JavaScript structure)
- **Styling**: Tailwind CSS with custom gradient themes and Google Fonts (Poppins and Inter)
- **Deployment**: Static site deployment optimized for GitHub Pages

### Single Page Application Structure
The application uses client-side routing with proper fallback handling:
- `index.html` serves as the main entry point
- `404.html` provides identical content to handle SPA routing on GitHub Pages
- `.nojekyll` file prevents Jekyll processing to ensure proper asset serving

## Key Components

### User Interface
- **Design System**: Lavender and pink gradient theme with responsive mobile design
- **Typography**: Professional font stack using Poppins (headings) and Inter (body text)
- **Icons**: SVG-based favicon system with emoji fallback (👗)
- **SEO Optimization**: Complete meta tag setup including Open Graph and Twitter Cards

### Core Features
- **AI Image Generation**: Fashion design creation from text prompts (demo mode for GitHub Pages)
- **Favorites System**: Save and manage preferred designs
- **Responsive Design**: Mobile-first approach with maximum scale constraints
- **Demo Mode**: Automatic environment detection for GitHub Pages deployment

### API Layer
- **Mock Data**: JSON-based API responses for demonstration purposes
- **Endpoints**: 
  - `/api/favorites.json` - User favorites management
  - `/api/images.json` - Generated images storage
- **Environment Detection**: Automatic switching between demo and production modes

## Data Flow

### Client-Side Data Management
1. **State Management**: React hooks for local state management
2. **Data Persistence**: Browser-based storage for favorites (localStorage likely)
3. **API Integration**: Fetch-based requests to JSON endpoints in demo mode
4. **Image Handling**: Dynamic image loading and display system

### Demo Mode Operation
- Detects GitHub Pages environment automatically
- Uses static JSON files to simulate API responses
- Provides sample fashion images for demonstration
- Maintains full functionality without backend dependencies

## External Dependencies

### CDN Resources
- **Google Fonts**: Poppins and Inter font families
- **Replit Integration**: Development banner script for Replit environment

### Build Dependencies
- **React Ecosystem**: Core React libraries with JSX runtime
- **Vite Build System**: Modern bundling and development server
- **Tailwind CSS**: Utility-first CSS framework

## Deployment Strategy

### GitHub Pages Optimization
- **Automated Deployment**: GitHub Actions workflow (`.github/workflows/deploy.yml`)
- **Zero Configuration**: Ready for immediate deployment
- **Asset Management**: Proper asset bundling and cache management
- **Routing Support**: SPA routing handled via 404.html fallback

### Development Environment
- **Replit Integration**: Development banner and environment detection
- **Hot Reloading**: Vite-based development server
- **Environment Switching**: Automatic demo mode activation on GitHub Pages

### Production Considerations
- **SEO Ready**: Complete meta tag implementation
- **Performance Optimized**: Bundled assets with proper caching headers
- **Mobile Responsive**: Touch-friendly interface with viewport constraints
- **Error Handling**: 404 fallback ensures no broken routes

The architecture prioritizes simplicity and immediate deployment while maintaining professional standards for a fashion-focused AI application. The demo mode allows for full feature demonstration without requiring complex backend infrastructure.