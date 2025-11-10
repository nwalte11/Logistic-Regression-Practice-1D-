# Logistic-Regression-Practice-1D-

An interactive web application for visualizing and animating sigmoid curve fitting to 1D data. Upload your data and parameter updates, then watch the sigmoid curve evolve through iterations.

## Features

- 📊 **Interactive Visualization**: Upload CSV files and see your sigmoid fit come to life
- 🎬 **Animation Controls**: Play, pause, step through, and reset animations
- 📈 **Real-time Updates**: Watch parameters `a` and `b` update the sigmoid curve: y = 1/(1+e^-(ax+b))
- 🎨 **Modern UI**: Clean, responsive design that works on any device
- 🚀 **No Backend Required**: Everything runs in your browser using Plotly.js

## Quick Start

1. Open `index.html` in your web browser
2. Upload a data CSV file with `x` and `y` columns
3. Upload a parameters CSV file with `a` and `b` columns
4. Use the controls to animate through parameter iterations

## Sample Files

The repository includes sample CSV files to get you started:
- `sample_data.csv` - Example data points
- `sample_parameters.csv` - Example parameter iterations

## CSV Format

### Data File
Must contain two columns:
```csv
x,y
-3.0,0.0
-2.0,0.1
-1.0,0.3
0.0,0.5
1.0,0.7
2.0,0.9
3.0,1.0
```

### Parameters File
Must contain two columns representing the parameters for each iteration:
```csv
a,b
0.1,0.0
0.5,0.5
1.0,1.0
1.5,1.0
```

## Controls

- **▶ Play**: Automatically animate through all iterations
- **⏸ Pause**: Stop the animation at the current iteration
- **⏭ Step**: Manually advance one iteration at a time
- **🔄 Reset**: Return to the first iteration

## Technical Details

- Built with vanilla JavaScript (no frameworks required)
- Uses Plotly.js for high-quality interactive plots
- Sigmoid function: y = 1 / (1 + e^-(ax+b))
- Responsive design works on desktop, tablet, and mobile

## Browser Requirements

Modern web browser with JavaScript enabled. Tested on:
- Chrome/Edge (recommended)
- Firefox
- Safari

## License

Open source - feel free to use and modify!