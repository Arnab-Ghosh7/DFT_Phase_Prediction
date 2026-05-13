# (Ba<sub>1-x</sub>Ca<sub>x</sub>)TiO<sub>3</sub> Phase Stability Prediction

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![UI: Responsive Dashboard](https://img.shields.io/badge/UI-Responsive%20Dashboard-blue)](#)

A machine learning and Density Functional Theory (DFT) driven dashboard designed to predict and analyze the phase stability of Calcium-doped Barium Titanate (Ba<sub>1-x</sub>Ca<sub>x</sub>)TiO<sub>3</sub>.

## Overview

This project provides an interactive web-based ML dashboard that visualizes phase transitions and electronic properties by bridging high-throughput DFT calculations with predictive machine learning models. The interface handles models trained on varying calcium doping concentrations ($x$ ranging from 10% to 50% at the Ba A-site).

## Features

- **Interactive ML Predictions**: Adjust features like Calcium doping percentage, Band Gap, Fermi Energy, and DOS (Density of States) to receive real-time phase stability predictions.
- **Cross-Composition Comparison**: Side-by-side analysis of model performance (e.g., SVM, Random Forest), probability of single-phase stability, and DFT features across all doping levels.
- **Physics-Informed Metrics**: Automatic calculation of fundamental parameters such as the Goldschmidt tolerance factor ($t$) and A-site mismatch ($\delta$).
- **Responsive UI & Themes**: Fully responsive design optimized for Desktop, Tablet, and Mobile, featuring seamless Light and Dark mode support.
- **Local Data Handling**: Secure, client-side CSV parsing. Drag and drop your DFT pipeline data (`phase_predictions_XX.csv`, `training_dataset_XX.csv`) to instantly populate the dashboard visualizations without server interactions.

## Technologies Used

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6)
- **Data Visualization**: [Chart.js](https://www.chartjs.org/) (v4.4.1)
- **Machine Learning**: Random Forest, SVM (RBF)
- **Physics Data**: Density Functional Theory (DFT) pipeline outputs

## Getting Started

### Prerequisites
No backend server or build process is required. You only need a modern web browser.

### Usage
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/Arnab-Ghosh7/DFT_Phase_Prediction.git
   ```
2. Navigate to the project directory and open the `bct web v2.html` file in any modern web browser.
3. Navigate to the **Upload Data** tab within the dashboard.
4. Drag and drop your pipeline output CSV files (e.g., `phase_predictions_10.csv` and `training_dataset_10.csv`). The application will automatically parse, cache, and display the insights across the Overview, Predict, and Compare tabs.

## Project Structure

- `bct web v2.html`: The core application containing the UI layout, styling, and JavaScript charting logic.
- `/bct 10`, `/bct 20`, `/bct 30`, `/bct 40`, `/bct 50`: Directories containing the original DFT computational and ML pipeline data at various doping thresholds.
- `BCT all present.docx`: Comprehensive project documentation and theoretical background.
- `LICENSE`: MIT License.

## License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.