# Flight Delay Analysis Dashboard ✈️

Interactive Tableau dashboard built with 2015 US flight data (5.8 million records from the USDOT Flight Delays dataset on Kaggle). This project analyzes departure/arrival delays, cancellations, taxi times, and root causes across major US airlines and routes, with a focus on high-traffic hubs like Chicago (ORD). Created during my Data Analytics bootcamp at IT Career Hub, it showcases ETL, statistical analysis, and dynamic visualization skills.

## 🎯 Dataset & Scope
- **Source**: [USDOT Flight Delays on Kaggle](https://www.kaggle.com/datasets/usdot/flight-delays) — public dataset with ~5.8M flights from US carriers in 2015.
- **Key Columns Analyzed**: Origin/Dest airports, airlines, delay duration, cancellation status, taxi-out/in times, causes (weather, air system, late aircraft, airline issues, security).
- **Time Period**: January–December 2015.
- **Goal**: Uncover patterns in operational inefficiencies, similar to my maritime KPI monitoring experience (e.g., optimizing port turnaround times).

## 📊 Key Visualizations & Features
The dashboard is fully interactive with filters for:
- **Airports/Cities** (e.g., Chicago to NYC, LAX, ATL)
- **Airlines** (e.g., Southwest, Delta, JetBlue)
- **Months/Days** (Monday–Sunday trends)
- **Night/Day** operations
- **Delay Status** (delayed, cancelled, diverted, on-time)

### Main Views:
1. **Map View**: Geospatial network map centered on Chicago (ORD), showing routes with average departure delays (e.g., CHI-NYC: 231 min, CHI-LAX: 199 min). Yellow lines/arrows indicate delay severity; hover for route details.
2. **Overview Charts**:
   - **KPIs**: 17.5% delayed flights, 1.5% cancelled, avg delay 13.6 min, avg taxi time 23.2 min.
   - **Line Charts**: Delay timeline trends (peaks in late 2015), taxi time by airline (JetBlue ~23 min avg).
   - **Bar Charts**: Delay status by airline (Southwest highest delayed ~20%; Delta lowest on-time ~80%).
   - **Pie Chart**: Delay causes (Weather: 24% or 24,268 flights; Air System: 10% or 5,620; Late Aircraft: ~4%; No Delay: 35%).
3. **Drill-Down**: Switch between Map and Overview via buttons; dynamic tooltips and parameters for slicing (e.g., filter by "Weather" causes only).

## 💡 Key Insights
- **Top Delay Hubs**: Chicago (ORD) routes dominate delays — e.g., CHI-NYC (231 min avg departure delay) due to air traffic and weather.
- **Airline Performance**: Southwest leads in volume but has higher delay rates (~18% delayed); Delta excels in on-time (82%) and low taxi times.
- **Causes Breakdown**: Weather impacts 24% of delays (esp. winter months); air system issues (NAS) at 10%; cancellations peak at 1.5% in high-traffic periods.
- **Trends**: Delays spike on Thursdays/Saturdays; night flights show 15% higher taxi times vs. day.
- **Business Value**: Identifies optimization opportunities, like my past work automating maritime reports to cut 5 hours/week — here, could reduce airline turnaround by targeting weather-prone routes.

## 🔗 Live Dashboard
👉 [View on Tableau Public](https://public.tableau.com/views/Project_Flights_Final/FlightDelayDaschboard?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

Download the .twbx for local edits (requires Tableau Desktop).

## 🛠️ Tech Stack & Process
- **Tableau Desktop/Public** (2023+): Data blending, LOD expressions for % calculations, geospatial mapping with Mapbox.
- **ETL Prep**: Initial cleaning in Excel/Google Sheets (handled nulls, aggregated by airline/route).
- **Skills Demonstrated**: Dashboard design, A/B-style trend analysis, KPI visualization — bridging my 18+ years in shipping ops to aviation data.

## 📁 Repository Structure
- `/screenshots/` — Dashboard previews:
  - [map-view.png](screenshots/map-view.png) — Route network from Chicago.
  - [overview-charts.png](screenshots/overview-charts.png) — KPIs, pies, bars, and lines.
- `Flight_Delay_Dashboard.twb` — Upload your Tableau workbook here (optional, for reproducibility).
- `data_sample.csv` — Small anonymized sample from Kaggle (optional).

## 🚀 How to Explore/Replicate
1. Open the [live link](https://public.tableau.com/views/Project_Flights_Final/FlightDelayDaschboard?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).
2. Apply filters (e.g., select "Delta" airline + "Weather" cause) to see dynamic updates.
3. Download dataset from [Kaggle](https://www.kaggle.com/datasets/usdot/flight-delays) and connect in Tableau for custom analysis.
4. For code extensions: See my Python projects for SQL/ETL automation.

## 📈 Related Projects
- [CRM Data Analysis](https://github.com/Volzhyn/unified-dashboard) — Python/SQL optimization for education cohorts.
- [Product Analytics Cohorts](https://github.com/Volzhyn/Product-Analytics-Cohorts) — Retention and funnel viz.

**From Chief Officer (18+ years maritime KPIs) to Data Analyst — turning operational chaos into actionable insights!**  
Based in Löbau, Germany. Open to **remote/hybrid Data Analyst roles** (Dresden area). Connect: [LinkedIn](https://www.linkedin.com/in/yuriy-volzhyn) | volzhynyuriy@gmail.com

---

*Project from IT Career Hub Bootcamp (Dec 2024–Oct 2025). Data: Public USDOT via Kaggle (CC0 license). Insights based on 2015 analysis.*
