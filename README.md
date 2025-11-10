# Sigmoid Function Visualization

An interactive web application for visualizing and animating sigmoid function fits to data. This tool allows users to see how different parameter values (a, b) affect the sigmoid curve y = 1/(1+e^-(ax+b)) as it fits to a dataset.

## Features

- **Data Visualization**: Upload CSV data with x and y values to visualize
- **Parameter Animation**: Upload CSV with parameter updates to see the sigmoid curve evolve
- **Interactive Controls**: 
  - Play: Animate through all parameter iterations
  - Pause: Stop the animation
  - Step: Move forward one iteration at a time
  - Reset: Return to the first iteration
- **Real-time Updates**: Watch the sigmoid curve update as parameters change
- **No Backend Required**: Runs entirely in the browser using JavaScript and Plotly.js

## Usage

1. Open `index.html` in a web browser
2. Upload two CSV files:
   - **Data CSV**: Contains your x and y data points
   - **Parameters CSV**: Contains parameter values (a, b) for each iteration
3. Use the controls to animate through the parameter updates

## CSV File Formats

### Data CSV Format
The data file should have two columns with headers `x` and `y`:

```csv
x,y
-3,0
-2,0
-1,0.1
0,0.3
1,0.7
2,1
3,1
```

### Parameters CSV Format
The parameters file should have two columns with headers `a` and `b`. Each row represents one iteration:

```csv
a,b
0.1,0
0.3,0
0.5,0
0.7,0
0.9,0
1.0,0
```

## Sample Files

Two sample CSV files are included:
- `sample_data.csv`: Sample data points
- `sample_parameters.csv`: Sample parameter iterations

## Sigmoid Function

The sigmoid function implemented is:

**y = 1 / (1 + e^-(ax+b))**

Where:
- `x` is the input value
- `a` is the slope parameter
- `b` is the bias/offset parameter
- `e` is Euler's number (≈2.71828)

## Technical Details

- **Framework**: Vanilla JavaScript (ES6+)
- **Visualization**: Plotly.js
- **No Dependencies**: No build process or package manager required
- **Browser-based**: No server or database needed

## Getting Started

Simply open `index.html` in any modern web browser. No installation or setup required!

## Browser Compatibility

Works with any modern browser that supports:
- ES6 JavaScript
- File API
- Plotly.js

Tested on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+