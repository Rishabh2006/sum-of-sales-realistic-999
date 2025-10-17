# Sales Summary Application (Task ID: sum-of-sales-realistic-999)

## Project Summary
This project is a lightweight, single-page web application (SPA) designed to process embedded CSV data, calculate the sum of the 'sales' column, and display the result prominently. The application adheres strictly to the requirement of being a single HTML file using in-memory processing and leveraging Bootstrap 5 for professional styling.

**Key Features:**
*   In-memory data processing (no external requests or storage dependencies).
*   Robust JavaScript logic to parse CSV data, identify the correct column header (`sales`), and perform summation.
*   Modern, responsive design using Bootstrap 5 from CDN.
*   The final sales figure is displayed prominently and formatted as currency.

## Setup Instructions
Since this application is a single HTML file with all dependencies linked via CDN, no local installation or build steps are required.

1.  Save the content of `index.html` into a file named `index.html`.
2.  Open `index.html` using any modern web browser (Chrome, Firefox, Edge, Safari).

The application will immediately load, parse the embedded data, calculate the total, and display the result.

## Usage Guide
Upon opening the `index.html` file, the user will see a centered card containing the calculated figure.

| Calculation Input (CSV) | Sales Column Data | Expected Output |
| :---------------------- | :---------------- | :-------------- |
| Laptop,1200             | 1200              |                 |
| Phone,850               | 850               |                 |
| Samartwatch,450         | 450               |                 |
| Tablet,600              | 600               | **$3,100**      |

The result displayed in the center of the page under the element `#total-sales` will be **$3,100**.

## Code Explanation

The core functionality resides within the embedded `<script>` tag in `index.html`.

### 1. Data Definition
The raw CSV data is stored in the `CSV_DATA` constant as a multi-line string.