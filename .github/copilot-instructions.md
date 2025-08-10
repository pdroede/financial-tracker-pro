# Financial Tracker Pro - Trading Journal

## Project Overview
Professional trading tracker web application for recording and analyzing trading performance. The app simulates real trading evolution from 750 USDT to 978 USDT based on actual trading data.

## Key Features
- Real-time trade recording and statistics
- Portfolio evolution charts
- Win/loss analysis
- Support for Long/Short positions with leverage
- Export functionality (CSV/JSON)
- Local storage persistence

## Technical Stack
- Pure HTML/CSS/JavaScript
- Chart.js for visualizations
- Responsive design with alien-themed UI
- No external dependencies beyond Chart.js

## Trading Data Structure
```javascript
{
  id: timestamp,
  date: 'YYYY-MM-DD',
  symbol: 'ETHUSDT', 
  type: 'compra' | 'venda', // Long/Short
  quantity: number,
  entryPrice: number,
  exitPrice: number,
  leverage: number,
  result: number, // Calculated P&L
  percentage: number // ROI percentage
}
```

## File Structure
- `/src/pages/trading-tracker.html` - Main trading tracker application
- `/index.html` - Project landing page
- Auto-populated with real trading data on first load

## Development Notes
- LocalStorage automatically populated with historical trades
- Supports cryptocurrency trading pairs
- Fractal Shifts and Support/Resistance strategies implemented
- Real trading evolution: 750 → 978 USDT (+30.4% gain)
