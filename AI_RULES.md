# AI Development Rules for DMS Protheus Application

## Tech Stack Overview

• **Core Framework**: Vanilla JavaScript with modern ES6+ features
• **Styling**: Tailwind CSS with custom configuration and CSS variables
• **Charts**: Chart.js for data visualization
• **UI Components**: Native HTML/CSS with custom-styled semantic elements
• **Icons**: Unicode emojis and SVG for visual elements
• **Fonts**: Google Fonts (Inter) for typography
• **Responsive Design**: Mobile-first approach with responsive breakpoints
• **Authentication**: Simple client-side password protection
• **Architecture**: Single-page application with tab-based navigation
• **Data Management**: In-memory JavaScript objects for content storage

## Library Usage Guidelines

### ✅ Approved Libraries & Their Uses

• **Tailwind CSS**: Primary styling solution - use exclusively for all layout and design
• **Chart.js**: Required for all data visualization - no alternative charting libraries allowed
• **Google Fonts**: Only for Inter font family - no additional font imports
• **Native JavaScript**: All interactivity and DOM manipulation must use vanilla JS

### ❌ Prohibited Libraries

• **React/Vue/Angular**: No frontend frameworks allowed - this is a vanilla JS project
• **jQuery**: Not permitted - use native DOM APIs instead
• **Bootstrap**: Not allowed - Tailwind CSS is our exclusive CSS framework
• **D3.js**: Not permitted - Chart.js is our only charting solution
• **Lodash/Underscore**: Not allowed - use native JavaScript methods
• **Any build tools**: No Webpack, Vite, or similar bundlers - this is a static site

### 🎨 Styling Rules

• Use Tailwind CSS utility classes exclusively for styling
• Define all custom values in CSS variables (:root)
• Maintain consistent color palette using existing brand colors
• Follow mobile-first responsive design principles
• Use existing animation classes rather than creating new ones

### 📊 Data Visualization Standards

• Use Chart.js for all charts and graphs
• Maintain consistent color scheme across all visualizations
• Ensure all charts are responsive and accessible
• Include proper labels, legends, and tooltips where appropriate

### 🧠 Architecture Principles

• Keep all content in the dataStore object for easy maintenance
• Use modular functions for rendering different sections
• Implement tab-based navigation without page reloads
• Maintain state in the appState object
• Ensure all interactive elements are keyboard accessible

### 🔒 Security Considerations

• Password protection is client-side only - not suitable for truly sensitive data
• No external API calls or data fetching mechanisms
• All content is statically embedded in the HTML file
• No user input validation beyond password checking