# UI-Dashboards Setup Guide

## Prerequisites

### Required Software
- **Web Browser**: Chrome, Firefox, Safari, or Edge (latest version)
- **Text Editor**: VS Code, Sublime Text, or any code editor
- **Git**: For version control (optional but recommended)

### No Additional Dependencies Required
This project is built using vanilla HTML, CSS, and JavaScript, so no additional installations are needed.

## Project Structure

```
alliance-2025-aditya-9944/
├── ui-dashboards/
│   ├── dashboard.html          # Step 1: Cards 1 (Dashboard Metrics)
│   ├── dashboard.css           # Styling for Cards 1
│   ├── cards2.html            # Step 3: Cards 2 (Product Cards) - API Ready
│   ├── cards2.css             # Styling for Cards 2
│   ├── charts.html            # Step 4: Charts (Bar & Pie Charts)
│   ├── charts.css             # Styling for Charts
│   ├── table.html             # Step 5: Table (Data Table with Loading/Error States) - API Ready
│   ├── table.css              # Styling for Table
│   ├── images/                # Product images directory
│   │   ├── iphone.png
│   │   ├── macbook.png
│   │   └── ... (other product images)
│   └── SETUP.md               # This file
```

## Installation & Setup

### Step 1: Clone or Download the Project
```bash
# If using Git
git clone <repository-url>
cd alliance-2025-aditya-9944/ui-dashboards

# Or simply download and extract the project files
```
### Step 2: Open the Application
1. Navigate to the `ui-dashboards` folder
2. Open `dashboard.html` in your web browser
3. The application will load immediately - no build process required
4. After cloning it run it on live server.

### Step 3: Navigate Between Sections
Use the sidebar navigation to switch between different sections:
- **Cards 1**: Dashboard metrics (Total Orders, Ordered Items, etc.)
- **Cards 2**: Product cards with images and pricing (API Ready)
- **Charts**: Interactive bar and pie charts
- **Table 1**: Data table with loading/error states (API Ready)

## API Integration Status

#### **Cards 2 (Product Cards)**
- **API Endpoint**: `http://interview.surya-digital.in/get-products`
- **Features**:
  - Loading state with spinner
  - Error handling with retry button
  - Dynamic product card generation
  - Fallback for missing images
  - Responsive grid layout

#### **Table 1 (Data Table)**
- **API Endpoint**: `http://interview.surya-digital.in/get-people-list`
- **Features**:
  - Loading state with spinner
  - Error handling with retry button
  - Location formatting (handles escaped commas)
  - Currency formatting (Indian Rupee)
  - Status badge color coding
  - Responsive table design
  - Custom API response parser for comma-separated format

#### **Table 1 (Paginated)**
- **API Endpoint**: `http://interview.surya-digital.in/get-people-list?page=1`

## Features Implemented

### Step 1: Cards 1 (Dashboard Metrics)
- Four metric cards with hardcoded data
- Responsive design with hover effects
- Clean, modern UI matching Figma design

### Step 2: Sidebar Navigation
- Left sidebar with navigation items
- Active state highlighting
- Seamless navigation between sections

### Step 3: Cards 2 (Product Cards)
- 12 product cards in responsive grid layout
- Product images, titles, descriptions, and pricing
- Status labels (New, Out of Stock)
- Stock information and sales data
- Responsive design (3-column → 2-column → 1-column)
- **API Integration Ready** with loading/error states

### Step 4: Charts
- Interactive bar chart (Sale By Device)
- Interactive pie chart (Revenue Contribution)
- Chart.js integration with hover tooltips
- Purple color scheme matching design
- Responsive chart containers

### Step 5: Table (Data Table)
- Complete data table with 8 columns
- Loading state with spinner animation
- Error state with retry functionality
- Status badges with color coding
- Indian Rupee formatting
- Responsive table design
- **API Integration Ready** with proper data formatting

## Technical Details

### Technologies Used
- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with Flexbox and Grid
- **Vanilla JavaScript**: Interactive functionality with async/await
- **Chart.js**: Chart library for data visualization

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Responsive Design
- Desktop: Full layout with sidebar
- Tablet: Adjusted grid layouts
- Mobile: Single column layouts with mobile navigation

## Data Sources

### Current Implementation
- **Cards 1**: Hardcoded metric data
- **Cards 2**: API-ready with loading/error states
- **Charts**: Hardcoded chart data
- **Table**: API-ready with loading/error states

### API Integration Features
- **Loading States**: Professional spinners during data fetch
- **Error Handling**: User-friendly error messages with retry options
- **Data Formatting**: Proper handling of escaped characters and currency
- **Fallback Handling**: Graceful degradation for missing data
- **Responsive Loading**: Loading states adapt to screen size
