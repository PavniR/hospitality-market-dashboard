# Airbnb Market Analytics & Consumer Sentiment Dashboard

## Project Overview
An interactive, enterprise-grade Power BI business intelligence application built to evaluate Airbnb property performance, pricing tier metrics, and granular consumer satisfaction scales. 

This interface incorporates an advanced user experience (UX) layout. It leverages state-based bookmarking toggles allowing end-users to seamlessly pivot between high-level performance trends and micro-level unstructured text reviews on a unified, real-estate-optimized display.

---

## Interactive Project Demo
*Since this project contains rich visual animations and toggle selections, watch the video below to see it in action:*

![Dashboard Demo Video](./dashboard_demo.mp4)

---
##  Quick Insights:

* **Privacy Over Budgets:** Most travelers choose Entire Homes or Private Rooms. Barely anyone books Shared Rooms, meaning premium properties drive the platform's core revenue.
* **Location Trumps Age:** A brand-new house does not automatically guarantee a higher price tag. Properties in premium neighborhoods command top dollar even if the building itself is quite old.
* **The Review Velocity Warning:** Properties with massive numbers of reviews piling up inside a single month are highly active but unstable. A sudden drop in recent monthly ratings means operations are slipping in real-time.
* **The Revenue Anchors:** Listings that maintain a high 4.5+ star rating over a massive historical volume of total reviews are the real backbone of the platform's user trust.
* **Strict Rules Burn Bookings:** Long, aggressive paragraphs in property house rules combined with strict cancellation policies scare away guests and leave rooms empty.
* **The Instant Booking Boost:** Turning on instant bookability bypasses host verification and triggers a massive spike in quick, last-minute booking volumes.
* **The Quality Trade-Off:** Instant-booking properties face slightly lower overall rating scores because hosts cannot filter out problematic or rowdy guests beforehand.
* **Verified Badges Pay Off:** Verified hosts can comfortably charge higher base prices and service fees because guests are willing to pay a premium for safety and scam protection.
* **Cluster Zones:** Properties cluster heavily around core geographic neighborhood zones, showing exactly where tourist demand is concentrated.

## Key Business & Analytical Insights

* **Spatial and Asset Stratification:** The listings reveals a high clustering of premium assets in key core `neighbourhood groups`. The market footprint is predominantly dominated by Entire Homes and Private Rooms, suggesting an urban travel demographic that prioritizes privacy over budget communal setups.
* **Price Elasticity & Fee Invariance:** Cross-filtering financial variables shows a linear relationship between `price` and `service fee`. Interestingly, tracking these metrics against the `Construction year` reveals asset age has a negligible impact on pricing power compared to historical review velocity and geographic positioning.
* **The Rules-to-Rating Friction:** Deep-dive analysis via the microscopic lens reveals a clear correlation: properties carrying highly restrictive configurations in `house_rules` experience distinct downward pressure on their `review rate number` scores, flagging a vital friction point for asset hosts to optimize.

---

## Interactive Features & UX Design

### 1. Macro-to-Micro UX Toggling
* **The Challenge:** Displays mapping customer feedback often suffer from a split screen clutter of charts vs dense data text tables.
* **The Solution:** Implemented native Power BI conditional selections. Users click an intuitive macro star-rating view or a detailed text-analysis lens icon. The platform utilizes underlying bookmarks to switch structural visual elements dynamically without reloading canvas contexts.

### 2. Multi-Tier Filtering
* Global slice parameters allow immediate cross-filtering by geographic territory, room type categories, and verified host tiers.
---

## Dashboard Data Architecture

### Page 1: Property Valuation & Performance Overview
* **KPI Matrix Summary:** Tracks aggregated listings totals, absolute average property prices, service charge thresholds, and baseline booking availability rates.
* **Property Distribution:** Segments the market footprint across Room Types (Entire Homes, Private Rooms, Shared Rooms) against host status parameters.
* **Geography Analysis:** Uses geospatial mapping parameters coordinates to detect hyper-local clustering patterns and real estate distribution across major neighborhood groups.

### Page 2: Customer Satisfaction & Review Velocity
* **What it tracks:** How fast guests leave reviews and what those ratings say about property quality.
* **Key Visuals:** Star-rating trends over time, tracking how review speed alters base scores, and an interactive micro-lens shaped text grid.
* **What the data says:** Highly active listings are vulnerable to quick rating drops if operations slip. Properties that hold high scores over a long historical volume are the core revenue anchors for the local market.

### Page 3: Booking Rules & Trust Analytics
* **What it tracks:** How host restrictions affect total bookings and overall customer trust.
* **Key Visuals:** Charts showing booking numbers for 'Instant Bookable' properties vs. traditional ones, and a breakdown of Strict vs. Flexible cancellation policies.
* **What the data says:** Chill hosts with flexible cancellation policies and clear verification badges get booked way faster and can command higher prices because guests feel safe booking them.
---

---

##  Tech Stack & How I Cleaned the Data
* **Platform:** Power BI Desktop.
* **Data Cleaning (Power Query):** The raw data was incredibly messy. I used Power Query to clean it up:
  * Stripped out currency symbols like `$` from the price columns so they could be calculated.
  * Replaced missing or corrupted values in structural columns so charts don't break.
  * Standardized spelling errors in neighborhood lists.

---

##  Smart DAX Formulas & Custom Measures
I heavily utilized **DAX (Data Analysis Expressions)** to write custom mathematical measures instead of just dragging raw columns. This means every number on the screen recalculates instantly when you click a filter:
* **Dynamic Averages:** Wrote formulas to track the average price changes and service fee ratios across different areas.
* **Review Velocity:** Created measures to track how fast listings accumulate reviews per month.
* **Rule vs. Rating Logic:** Built calculations that look at host rules and instantly output consumer satisfaction scores.
---

* **Analytical Dashboard Core:** [Click to open local `.pbix` Source File](./airbnb-dashboard.pbix) 

---
**Author** [Pavni Rastogi]  
