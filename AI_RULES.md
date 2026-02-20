# AI Development Rules for DMS Protheus Application

## Tech Stack Overview

• **Core Framework**: Vanilla JavaScript with modern ES6+ features
• **Styling**: Tailwind CSS for utility-first styling approach
• **Charts**: Chart.js for data visualization
• **UI Components**: Pure HTML/CSS/JS implementation with custom styling
• **Deployment**: Static hosting ready (no build step required)
• **Responsive Design**: Mobile-first approach with responsive breakpoints
• **Security**: Client-side password protection for demonstration purposes

## Library Usage Guidelines

### ✅ Approved Libraries

1. **Tailwind CSS** - For all styling needs. Use utility classes exclusively for consistent design.
2. **Chart.js** - For all data visualization requirements. Already integrated and optimized.
3. **Google Fonts** - For typography enhancements (currently using Inter font family).
4. **Lucide Icons** - For iconography (can be added if needed).

### ❌ Restricted Libraries

1. **React/Vue/Angular** - Do not convert to frameworks. Maintain vanilla JS architecture.
2. **jQuery** - Not needed with modern vanilla JS capabilities.
3. **Bootstrap** - Tailwind CSS is our exclusive CSS framework.
4. **D3.js** - Chart.js is sufficient for our visualization needs.
5. **External UI component libraries** - Create custom components using Tailwind CSS.

### 🎨 Design System Rules

1. **Color Palette**: 
   - Primary: `#18181b` (Zinc 900)
   - Accent: `#dc2626` (Red 600)
   - Secondary: `#71717a` (Zinc 500)
   - Light: `#e4e4e7` (Zinc 200)

2. **Typography**: 
   - Font Family: Inter (loaded via Google Fonts)
   - Heading Scale: Use existing heading classes (text-xl through text-3xl)
   - Body Text: Base size with appropriate line-height

3. **Components**:
   - Use existing card styles with `.feature-card` class
   - Follow established button patterns
   - Maintain consistent spacing with Tailwind padding/margin utilities

### 📊 Chart Implementation Rules

1. Always use Chart.js for data visualization
2. Follow existing color scheme (`colors` object in JavaScript)
3. Maintain consistent chart container sizing with `.chart-container` class
4. Use existing animation configurations
5. Ensure charts are responsive and destroy properly during navigation

### 🔒 Security Considerations

1. Password protection is client-side only for demonstration purposes
2. Do not add any server-side functionality without explicit requirements
3. Keep sensitive information out of client-side code