# Overview

This is a single-file e-commerce catalog website for DIOB SHOP, specializing in adult products and various items sold through WhatsApp integration. The application displays products in three distinct categories: available items, special order items, and adult content books. Built as a monolithic HTML file with embedded CSS and JavaScript, it's designed to work offline and can be hosted on static platforms like GitHub Pages or opened directly in a browser without requiring a server.

## Brand Identity
- **Company Name**: DIOB SHOP
- **Slogan**: "Le marché central des sextoys et divers en ligne"
- **Logo**: Custom branded logo integrated in header with shopping cart icon design
- **Focus**: Adult products and various online items with WhatsApp ordering system

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Single File Design**: Complete application contained in one HTML file with embedded CSS and JavaScript for maximum portability and offline functionality
- **Responsive Layout**: CSS Grid and Flexbox-based layout system that adapts to different screen sizes
- **Component-Based Structure**: Modular JavaScript functions for product rendering, cart management, and WhatsApp integration
- **Static Asset Management**: External product images hosted on Pixabay with fallback handling

## Data Management
- **JSON-Based Catalog**: Product data stored in a separate `catalog.json` file with structured product information including IDs, titles, prices, and image URLs
- **Client-Side State**: Shopping cart state managed entirely in browser localStorage for persistence across sessions
- **Category-Based Organization**: Products organized into three distinct categories (available, special order, adult content) with different business rules

## User Interface Design
- **WhatsApp Theme**: Green color scheme (#25D366, #128C7E) matching WhatsApp branding
- **Card-Based Layout**: Product display using card components with images, titles, prices, and action buttons
- **Warning Systems**: Clear visual indicators for special order requirements and age restrictions
- **Accessibility**: Font Awesome icons and semantic HTML structure

## Business Logic
- **Cart Functionality**: Add/remove items with quantity management and total calculation
- **WhatsApp Integration**: Direct message composition with product details and cart contents
- **Special Order Handling**: 25% deposit requirement messaging for special order items
- **Age Verification**: Content warnings for adult material with purchase restrictions

# External Dependencies

## Third-Party Services
- **Pixabay CDN**: Product image hosting service for all product photographs
- **Font Awesome CDN**: Icon library for UI elements and WhatsApp branding
- **WhatsApp Web API**: Direct integration for order messaging and customer communication

## Browser APIs
- **LocalStorage API**: Client-side data persistence for shopping cart state
- **Window.open API**: WhatsApp message composition and navigation

## Static Hosting Requirements
- **GitHub Pages Compatible**: Designed for static file hosting without server-side requirements
- **Offline Functionality**: Complete application works without internet connection after initial load
- **Cross-Browser Support**: Compatible with modern web browsers without additional dependencies