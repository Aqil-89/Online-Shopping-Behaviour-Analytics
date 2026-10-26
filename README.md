# ShopPulse — Online Shopping Behaviour Analytics

## Project overview
ShopPulse is a browser-based dashboard prototype for exploring online shopping session behaviour. It provides dashboard KPIs, filters, charts, a data explorer, behaviour analysis, CSV upload, filtered CSV export, and a simulated scan-versus-index performance demonstration.

## Current implementation
- **Frontend:** HTML, CSS, JavaScript
- **Charts:** Chart.js 4.4.1 loaded from a CDN
- **Data:** Built-in generated sample data (12,330 sessions) or a user-uploaded CSV
- **CSV input:** Expects the UCI Online Shoppers Purchasing Intention dataset column names
- **Performance page:** Simulates indexed lookups in the browser; it is **not** a real MongoDB benchmark

## Important scope note
This package contains the uploaded HTML dashboard only. It does not currently include a Python/Streamlit application, a MongoDB server integration, a Redis caching implementation, or a real backend API. Do not describe those components as implemented unless you add and test them separately.

The built-in sample data is generated in JavaScript and should not be presented as actual measured results from the UCI dataset. For report results based on the UCI dataset, upload the real dataset through the dashboard and verify the outputs.

## Run locally
1. Extract this folder.
2. Open `index.html` in a modern browser.
3. Select **Use Sample Data** or use **Choose CSV file** to load a compatible CSV.

The dashboard loads Chart.js from a CDN, so an internet connection is needed for charts to render.

## Dataset
UCI Online Shoppers Purchasing Intention Dataset:
https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset

## Team
- Syed Aqil
- Ashok G
- Shazil Khan
- Shivam

Course: Data Modelling with NoSQL Database (E1CSA 363)  
Institution: Alliance School of Advanced Computing, Alliance University  
Mentor: Dr. Subrata Pain

## Suggested next development steps
1. Connect the dashboard to a real backend/API.
2. Implement MongoDB storage, aggregation queries, and indexes.
3. Implement Redis KPI caching and cache invalidation.
4. Record reproducible MongoDB and Redis benchmark results.
5. Add verified screenshots and test instructions.
