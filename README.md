# Website Traffic Analytics Dashboard

A modern, interactive dashboard for analyzing website traffic patterns and predicting future trends. Built with React, TypeScript, and Chart.js.

![Dashboard Preview](https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&q=80&w=2426)

## Features

### Real-time Analytics
- **Unique Visitors**: Track daily unique website visitors
- **Page Views**: Monitor total page views across your site
- **Session Duration**: Analyze user engagement through session length
- **Bounce Rate**: Measure the percentage of single-page visits

### Advanced Visualizations
- Interactive time series charts
- Historical data trends (30 days)
- Future predictions (7 days)
- Confidence intervals for forecasts
- Week-over-week performance comparisons

### Predictive Analytics
- Linear regression modeling
- Weekly seasonality patterns
- Trend analysis
- Uncertainty visualization
- Automated forecasting

## Technology Stack

- **Frontend Framework**: React 18 with TypeScript
- **Styling**: Tailwind CSS
- **Charts**: Chart.js with react-chartjs-2
- **Date Handling**: date-fns
- **Icons**: Lucide React
- **Build Tool**: Vite
- **Package Manager**: npm

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm (v6 or higher)

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

## Project Structure

```
src/
├── components/          # React components
│   ├── MetricCard.tsx  # Individual metric display
│   └── TrafficChart.tsx# Time series visualization
├── utils/
│   └── mockData.ts     # Data generation utilities
├── types.ts            # TypeScript interfaces
├── App.tsx             # Main application component
└── main.tsx           # Application entry point
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## Customization

### Adding New Metrics

1. Add the metric to the `TrafficData` interface in `src/types.ts`
2. Update the mock data generation in `src/utils/mockData.ts`
3. Add a new `MetricCard` component in the dashboard grid

### Modifying Predictions

The prediction algorithm can be customized in `src/utils/mockData.ts`:
- Adjust the prediction window by modifying `daysToPredict`
- Modify the uncertainty calculation
- Implement different forecasting algorithms

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Chart.js for the powerful charting library
- Tailwind CSS for the utility-first CSS framework
- Lucide React for the beautiful icons
- The React team for the excellent framework
