# Modern SQL Editor

A powerful and modern SQL editor built with React 18 and Vite, designed for efficient data interaction. Write and execute SQL queries in a clean, intuitive tab-based interface with a visually appealing UI, enhanced by features for productivity and performance.

## Tech Stack

This project leverages cutting-edge technologies:

- **[Vite](https://vitejs.dev/)** - Lightning-fast frontend build tool for a superior development experience.
- **[React 18](https://react.dev/)** - The latest React library, featuring improved rendering capabilities and modern hooks for building dynamic user interfaces.
- **[React Bootstrap](https://react-bootstrap.github.io/)** - A comprehensive suite of Bootstrap components rebuilt for React, ensuring responsiveness and consistent styling.
- **[CodeMirror 6](https://codemirror.net/)** - A state-of-the-art code editor providing robust SQL syntax highlighting, autocompletion, and a customizable editing environment.
- **[React Table](https://react-table.tanstack.com/)** - A powerful and flexible library for building interactive tables with essential features like sorting, filtering, pagination, and more.

## Key Features

✨ **Intuitive User Interface**: Clean, responsive design with both light and dark editor themes to suit your preference. The dark theme provides enhanced readability with distinct color-coding for SQL elements.
✨ **Tab-Based Workflow**: Manage multiple SQL queries effortlessly with a tabbed interface, allowing you to work on different tasks simultaneously and switch between them seamlessly.
✨ **Intelligent SQL Query Editor**:
    * **Syntax Highlighting**: Enhances readability and reduces errors by visually distinguishing SQL keywords and syntax.
    * **Automatic Query Suggestion**: Speeds up query writing by suggesting relevant keywords and table/column names as you type.
    * **Autocompletion**: Completes words with a simple press of the "Enter" key after a suggestion, further accelerating your workflow.
    * **Line Wrapping**: Ensures long queries are easy to read without horizontal scrolling in the editor.
✨ **Database Object Explorer (Collapsible Sidebar)**:
    * Explore your database schema with a navigable list of tables, providing quick access to the data you need.
    * Clicking on a table in the sidebar automatically runs a `SELECT * FROM [tableName]` query, instantly displaying the table's contents.
    * The sidebar also displays the number of results and the time taken to fetch and render the data for quick performance insight.
    * Toggle the sidebar's visibility using a header button to maximize your workspace.
✨ **Interactive and Feature-Rich Results Table**:
    * **Resizable Columns**: Adjust column widths for optimal data viewing.
    * **Expandable Rows**: View complete data for rows with large content in a convenient pop-up.
    * **Pagination**: Navigate through large result sets with ease using built-in pagination.
    * **Header Sorting**: Sort data by clicking on column headers (ascending/descending).
    * **Horizontal and Vertical Scrolling**: Handle large datasets with comprehensive scrolling capabilities.
    * **Real-time Search and Filtering**: Quickly find specific data within results and columns using a dynamic search bar.
✨ **Query History (Recent Queries)**: Easily access and reuse recently executed or created queries from the sidebar.
✨ **Data Export**:
    * **Export as CSV**: Download query results as a CSV file for use with spreadsheet software.
    * **Export as JSON**: Export results as a JSON file for data interchange and web applications.
✨ **Fullscreen Mode**: Maximize your focus by toggling the application to fullscreen, expanding the editor and results area.
✨ **Local Session Persistence**: Your active session, including open tabs and query history, is automatically saved and restored on browser reload.
✨ **Welcoming First-Time Experience**: New users are greeted with a helpful welcome message and clear instructions on how to begin.

## Getting Started

### Prerequisites

- Node.js 16.x or higher
- npm 7.x or higher

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/Rohit9568/ATLNassignment.git
   cd modern-sql-editor

2. Install dependencies
   ```bash
   npm install
   ```

3. Start the development server
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:3000`

## Project Structure

```
sqleditor/
├── public/           # Static assets and data files
├── src/              # Source code
│   ├── components/   # React components
│   │   ├── navigation/  # Navigation components
│   │   ├── query/       # SQL editor components
│   │   ├── table/       # Table components
│   │   └── tabs/        # Tab management components
│   ├── css/          # CSS styles
│   ├── data/         # Data utilities and definitions
│   ├── hooks/        # Custom React hooks
│   ├── App.jsx       # Main application component
│   ├── App.css       # Application styles
│   ├── index.css     # Global styles
│   ├── main.jsx      # Application entry point
│   └── utils.jsx     # Utility functions
├── index.html        # HTML template
├── vite.config.js    # Vite configuration
└── package.json      # Dependencies and scripts
```


## Available Scripts

In the project directory, you can run:

### `npm run dev`

Runs the app in development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `npm run build`

Builds the app for production to the `build` folder.\
It optimizes the build for the best performance.

### `npm run preview`

Previews the production build locally.

## Performance Optimizations

- **Vite HMR**: Fast hot module replacement during development
- **Code Splitting**: Load components on demand for faster initial load
- **Dynamic Data Loading**: Fetch data only when needed
- **Modern React Patterns**: Functional components and hooks throughout
- **CSS Optimizations**: Clean, minimal styles for fast rendering
- **Lazy Loading**: Components and data are loaded only when they are required, contributing to a faster initial load and better resource management.

## Performance Metrics (Lighthouse & PageSpeed Insights)

The Modern SQL Editor is designed for optimal performance across devices. Here are the performance metrics obtained using Lighthouse and PageSpeed Insights:

**Lighthouse (Desktop):**

* **First Contentful Paint (FCP):** 0.8 s
* **Largest Contentful Paint (LCP):** 0.9 s
* **Total Blocking Time (TBT):** 10 ms
* **Cumulative Layout Shift (CLS):** 0.079
* **Speed Index:** 0.9 s
* **Accessibility:** 88
* **Best Practices:** 96
* **SEO:** 100

**PageSpeed Insights:**

* **Mobile Performance:** 91
    * **First Contentful Paint (FCP):** 2.9 s
    * **Largest Contentful Paint (LCP):** 2.9 s
    * **Total Blocking Time (TBT):** 0 ms
    * **Cumulative Layout Shift (CLS):** 0.03
    * **Speed Index:** 2.9 s
* **Desktop Performance:** 100
    * **First Contentful Paint (FCP):** 0.6 s
    * **Largest Contentful Paint (LCP):** 0.6 s
    * **Total Blocking Time (TBT):** 0 ms
    * **Cumulative Layout Shift (CLS):** 0
    * **Speed Index:** 0.6 s

These metrics demonstrate the application's commitment to providing a fast and responsive user experience on both mobile and desktop platforms. Further optimizations are planned based on the diagnostics provided by these tools.

## License

This project is open source and available under the MIT License.
