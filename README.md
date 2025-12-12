# SalesTrack – README

## Overview

SalesTrack is a web-based application that helps businesses log sales transactions, monitor regional and product-wise performance, and generate visual dashboards for better decision-making. It offers analytics charts, progress tracking, automated alerts, dark/light mode, and structured data handling—all running directly in the browser using HTML, CSS, and JavaScript.

This README explains the project setup, features, architecture, calculation logic, and challenges.


## Features / Functional Requirements

### Core Functionalities

* Log and categorize sales transactions by:

* Product
* Region
* Salesperson
* Generate bar-chart-based analytics dashboard using Chart.js
* Track total sales and monitor progress
* Responsive layout for desktop and mobile
* Export-ready design (reports can be captured as screenshots)

### Optional Enhancements Included

* Automated alerts when sales targets are reached
* Predictive insight foundation (structured data ready for modeling)
* Interactive drill-down analytics through categorized grouping
* Dark/Light mode toggle for UI accessibility


## Project Structure

/salestrack
 │
 ├── index.html      # Main website (HTML, CSS, JS written inline)
 ├── README.md       # Documentation (this file)
 └── assets/         # (Optional) Images or styles if added later


## How to Run the Project

No installations required.

1. Download or copy the HTML code.
2. Save it as **index.html**.
3. Open it directly in any browser (Chrome, Edge, Firefox).
4. The website will load instantly—no server needed.


## How It Works (Logic Breakdown)

### **1. Adding a Sale**

Each sale entry includes:

* Product name
* Region
* Salesperson
* Sale amount (₹)

These are stored in a JavaScript list:

salesData = [ { product, region, person, amount } ]


### **2. Total Sales Calculation**

Total = sum of all sale amounts


### **3. Regional Analytics**

For each region:

Region Total = sum(amount where sale.region matches selected region)


Displayed using **Chart.js** bar graph.

### **4. Automated Target Alerts**

If total sales exceed ₹2,00,000 → popup alert triggers once.

### **5. Dark/Light Mode**

Uses a class toggle:

document.body.classList.toggle("dark-mode")


## Libraries Used

* **Chart.js CDN** – for bar charts
* No external frameworks required


## Deliverables Covered

*  HTML, CSS, JavaScript source code
*  README file with setup, features, modules, and explanations
*  Analytics dashboard screenshots (user can generate by running)
*  GitHub-ready structure
*  Suitable for academic/project report documentation


## Challenges Addressed

* Designing meaningful dashboards for complex sales data
* Handling real-time UI updates without backend support
* Representing trends clearly using visual charts
* Creating a simple and responsive UI for all devices
* Balancing feature-rich analytics with lightweight browser performance


## Future Enhancements

* CSV/Excel export feature
* Predictive analytics using regression or ML
* Multi-user login & secure data storage (Node.js / Firebase backend)
* Sales target configuration panel
* Advanced drill-down analytics (product-wise, salesperson-wise)

