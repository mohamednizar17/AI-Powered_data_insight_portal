# AI-Powered Data Insight Portal

A web application for analyzing and visualizing CSV data with AI-driven insights, featuring interactive data preparation, multiple chart types, and a user-friendly interface with hover animations.

## Features
- **Data Upload**: Upload CSV files for analysis.
- **AI-Driven Suggestions**: Automatic recommendations for handling missing values, outliers, normalization, and visualization types.
- **Data Preparation**:
  - Handle missing numerical/categorical values (mean, median, mode, remove).
  - Manage outliers (remove, cap).
  - Normalize numerical columns.
- **Data Visualization**:
  - Supports Bar, Scatter, Line, Pie, Bubble, Area, Stacked Bar, Histogram, Doughnut, and Radar charts.
  - Customizable X/Y axes, color picker, and index range.
  - Download charts as PNG and transformed data as CSV.
- **Interactive UI**:
  - Animated home page with floating particles and data icons.
  - Hover animations on Data Preparation (rotating gear) and Data Visualization (pulsing chart) options.
  - Responsive design for mobile and desktop.
- **Accessibility**: High-contrast colors, focus states, and semantic HTML.

## Prerequisites
- **Browser**: Modern browsers (Chrome, Firefox, Edge).
- **Node.js** (Optional): For local development with npm to manage dependencies.
- **Internet**: Required for CDN or local library hosting.

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/ai-data-insight-portal.git
   cd ai-data-insight-portal
   ```

2. **Install Dependencies** (Optional):
   If you prefer local libraries over CDNs:
   ```bash
   npm install
   ```
   The `requirements.txt` lists:
   - `chart.js@4.4.2`
   - `papaparse@5.4.1`

3. **Serve the Application**:
   - Use a local server (e.g., Live Server in VSCode or Python’s HTTP server):
     ```bash
     python -m http.server 8000
     ```
   - Open `http://localhost:8000` in your browser.

## Usage
1. **Upload CSV**:
   - On the homepage, click "Upload Your Data" to select a CSV file.
   - Example CSV:
     ```csv
     Region,Sales,Price
     North,100,10.5
     South,,15.0
     North,200,12.0
     West,150,100.0
     South,300,14.5
     ```

2. **Choose a Path**:
   - **Data Preparation**: Clean data with AI suggestions (e.g., fill missing values, cap outliers).
   - **Data Visualization**: Skip prep and visualize directly (with a warning if unprocessed).

3. **Data Preparation**:
   - Select options for numerical/categorical columns (e.g., mean fill, normalize).
   - Apply changes and download transformed data as CSV.

4. **Data Visualization**:
   - Choose X/Y axes, plot type, and color.
   - Set start/end indices for data subset.
   - Generate plots and download as PNG.
   - View legends for data insights.

5. **Interact**:
   - Hover over "Data Preparation" for a rotating gear (⚙️).
   - Hover over "Data Visualization" for a pulsing chart (📊).

## Project Structure
```
ai-data-insight-portal/
├── index.html         # Main application file
├── requirements.txt   # JavaScript dependencies
├── README.md          # Project documentation
└── /screenshots/      # (Optional) Screenshots or demo GIFs
```

## Screenshots
*(Add screenshots of the homepage, data preparation, and visualization pages here.)*

## Contributing
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m 'Add new feature'`).
4. Push to your branch (`git push origin feature-name`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See [LICENSE](LICENSE.md) for details.

## Contact
For issues or suggestions, contact [arnizz077@gmail.com] or open an issue on GitHub.

---

Built with:
- HTML5, CSS, JavaScript
- [Chart.js](https://www.chartjs.org/) for visualizations
- [PapaParse](https://www.papaparse.com/) for CSV handling
- Poppins font via Google Fonts
