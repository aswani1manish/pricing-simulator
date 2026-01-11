# DDP Price Calculator - Innovative Beauty Group

A web-based pricing calculator for computing DDP (Delivered Duty Paid) prices with component cost breakdowns.

## Features

1. **Product Information**
   - Text input for finished product name
   - Product name is included in PDF exports

2. **Component Management**
   - Add multiple components with detailed costs
   - Source country selection (14 countries available)
   - Component cost tracking
   - Freight cost tracking
   - Bulk Assembly cost tracking (fixed amount)
   - Scrap cost tracking (percentage of component cost)
   - Duties calculated as percentage of component cost

3. **Duties Calculation**
   - Enter duties as a percentage (e.g., 5.5%)
   - Automatically calculated based on component cost
   - Displays both percentage and dollar amount

4. **Price Summary**
   - Real-time totals for all cost categories
   - Configurable profit margin percentage
   - Final DDP price calculation

5. **PDF Export**
   - Export complete pricing breakdown to PDF
   - Includes all components with details
   - Professional formatting with tables
   - Summary section with totals

## Requirements

### For PDF Export Functionality
The PDF export feature requires internet access to load external libraries:
- jsPDF (v2.5.1) from cdnjs.cloudflare.com
- jsPDF AutoTable plugin (v3.5.31) from cdnjs.cloudflare.com

If you need offline functionality, download these libraries and update the script tags in `index.html` to reference local copies.

## Usage

1. Open `index.html` in a web browser
2. Enter the finished product name
3. Add components:
   - Enter component name
   - Enter component cost
   - Select source country
   - Enter freight cost
   - Enter bulk assembly cost
   - Enter scrap percentage (applied to component cost)
   - Enter duties percentage (if applicable)
4. Set expected margin percentage
5. View the price summary
6. Click "Export to PDF" to generate a detailed pricing document

## File Structure

```
pricing-simulator/
├── index.html          # Main application file (HTML, CSS, and JavaScript)
├── README.md          # This file
└── readme.txt         # Original project readme
```

## Technical Details

- **Technology**: Pure HTML5, CSS3, and vanilla JavaScript
- **No Build Process**: Can be opened directly in a browser
- **No Dependencies**: All code is self-contained except PDF generation libraries
- **Responsive Design**: Works on various screen sizes
- **Security**: Uses DOM manipulation to prevent XSS vulnerabilities

## Browser Compatibility

Works in all modern browsers that support:
- ES6 JavaScript features
- HTML5 form elements
- CSS Grid and Flexbox

## Future Enhancements

Potential areas for improvement:
- Save/load pricing configurations
- Import/export component data as CSV
- Currency selection
- Tax calculations
- Historical pricing comparisons
