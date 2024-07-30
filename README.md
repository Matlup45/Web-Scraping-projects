# Web-Scraping-projects

# Project Scraper for Registered Projects

## Overview

**This Python script scrapes the details of the first 6 projects listed under the "Registered Projects" heading on the [Haryana RERA Public Dashboard](https://hprera.nic.in/PublicDashboard). It extracts the following fields from each project's detail page:
- GSTIN No
- PAN No
- Name
- Permanent Address**

## Prerequisites

Make sure you have Python installed. This script also requires the following Python packages:

- `selenium`
- `pandas`

Additionally, you need to have `chromium-chromedriver` installed on your system.

## Installation

To set up the environment, follow these steps:

1. **Install Required Packages**

  Run the following commands to install the required Python packages:

   ```bash
   pip install selenium pandas
```
Install and Configure Chromium Driver

For Debian-based systems (e.g., Ubuntu), use the following commands:
```
   apt-get update
   apt install -y chromium-chromedriver
   cp /usr/lib/chromium-browser/chromedriver /usr/bin
```

**Code Explanation
**
The script uses selenium to automate the browser and scrape data.

It waits for elements to be visible and ensures that the loading spinner disappears before extracting data.

The details are fetched from the project's modal and saved into a pandas DataFrame.

The DataFrame is then saved as a CSV file.

***Contributing***
If you want to contribute to this project, please fork the repository and submit a pull request with your changes. Make sure to include tests for any new features or bug fixes.


