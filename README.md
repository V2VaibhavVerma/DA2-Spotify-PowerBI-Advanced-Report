# Spotify Top-50 World Analytics Dashboard (Power BI)

## Project Overview

This project is an advanced **Power BI analytics dashboard** built on Spotify’s *Top-50 World* chart data.  
The report is designed to move beyond descriptive reporting and answer **product-level and strategy-level questions** such as:

- What characteristics define a Spotify hit?
- How stable or volatile is popularity over time?
- Do singles outperform albums?
- How does explicit content affect chart success?
- Which artists are consistently dominant versus viral?

The dashboard combines **advanced DAX measures**, **analytical visuals**, and **Spotify-inspired UX design** to simulate how a real-world music analytics or streaming product team would explore performance.

---

## Data Source & Structure

The dataset (`Top-50-World`) contains daily chart-level song metadata with the following key fields:

| Category | Columns |
|-------|--------|
| Time | `date`, `release_date` |
| Chart Performance | `position`, `popularity` |
| Song Metadata | `song`, `artist`, `duration_ms`, `is_explicit` |
| Album Metadata | `album_type`, `total_tracks`, `album_cover_url` |

Each row represents a song’s presence on the **Spotify Global Top-50** chart for a given day.

---

## Analytical Framework

This dashboard is structured around **five analytical pillars**:

1. **Chart Performance & Rank Dynamics**
2. **Popularity & Volatility Analysis**
3. **Song Characteristics & Optimization**
4. **Release Strategy & Lifecycle**
5. **Artist Dominance & Consistency**

Each pillar is supported by a **dedicated DAX measure layer** and purpose-built visuals.

---

## DAX Measure Architecture

The report uses a **measure-driven design**. All insights are derived from reusable DAX measures rather than calculated columns.

### Core Measure Categories

- **Base Metrics**
  - Total Songs
  - Unique Songs
  - Unique Artists
  - Chart Days

- **Popularity Intelligence**
  - Average / Max / Min Popularity
  - Popularity Standard Deviation
  - Popularity Volatility Index

- **Rank Analytics**
  - Average Position
  - Best & Worst Position Achieved
  - Top-10 Appearances
  - Top-10 Share %

- **Duration & Efficiency**
  - Average Duration (Minutes)
  - Popularity per Minute
  - Longest / Shortest Song

- **Content Classification**
  - Explicit vs Non-Explicit Performance
  - Explicit Content Share %

- **Release Strategy**
  - Singles vs Albums Count
  - Singles-to-Albums Ratio
  - Average Album Track Count

- **Lifecycle Metrics**
  - Days Since Release
  - Popularity Decay Rate

- **Artist Intelligence**
  - Songs per Artist
  - Artist Consistency Index

These measures are written using **context-aware DAX**, enabling correct behavior under slicing, filtering, and drill-down.

---

## Report Pages & Walkthrough

### 1. Overview (Executive Summary)

**Purpose:**  
Provide a one-screen snapshot of the Spotify chart ecosystem.

**Key Visuals:**
- KPI cards: Total Songs, Avg Popularity, Avg Duration, Artist Count
- Album artwork preview (dynamic image binding)
- Donut charts: Singles vs Albums, Explicit vs Non-Explicit
- Trend line: Average Popularity by Quarter
- Bar chart: Total Songs by Quarter

**Insights Enabled:**
- Market concentration
- Content mix trends
- Seasonality in popularity

---

### 2. Artists Analysis

**Purpose:**  
Evaluate artist dominance, consistency, and portfolio breadth.

**Key Visuals:**
- Songs by Artist (ranked bar charts)
- Artist Consistency Index bar chart
- Artist performance table with:
  - Songs per Artist
  - Avg Popularity
  - Max Popularity
  - Avg Duration

**Insights Enabled:**
- Superstar vs long-tail artists
- Consistent hitmakers vs one-hit performers
- Output quantity vs quality trade-offs

---

### 3. Songs Analysis

**Purpose:**  
Analyze song-level efficiency and performance drivers.

**Key Visuals:**
- Songs by Popularity per Minute
- Songs by Top-10 Appearances
- Song-level table with duration extremes
- Dynamic album cover linked to selection

**Insights Enabled:**
- Streaming-optimized song length
- Longevity vs peak performance
- Efficiency of attention capture

---

## Advanced Visualization Techniques Used

- **Dynamic Image Rendering**  
  Album covers rendered using URL binding.

- **Measure-Driven Ranking**  
  All ranking visuals use DAX measures instead of static sorting.

- **Cross-Page Filtering**  
  Artist and song selections propagate across pages.

- **Conditional Formatting**  
  Visual emphasis based on popularity, consistency, and dominance.

- **Spotify-Inspired UI**
  - Dark theme
  - High-contrast typography
  - Minimalist card layouts
  - Brand-consistent color palette

---

## Design Philosophy

The report is intentionally designed to feel like a **product analytics dashboard**, not a traditional BI report.

Principles followed:
- Minimal clutter
- High information density
- Clear visual hierarchy
- Business-question-first layout
- Storytelling through interaction

---

## Tools & Technologies

- **Power BI Desktop**
- **DAX (Advanced Measure Logic)**
- **Data Modeling & Context Transition**
- **Custom Visual Formatting**
- **GitHub for versioning & documentation**

---

## How to Use This Repository

1. Clone the repository
2. Open the `.pbix` file in Power BI Desktop
3. Review the DAX measures in Model View
4. Interact with slicers and visuals to explore insights
5. Extend with:
   - Rolling windows
   - Calculation groups
   - What-if parameters
   - Forecasting or anomaly detection

---

## Potential Extensions

- Rolling popularity momentum
- Rank movement (bump charts)
- Time-based calculation groups
- Genre-level enrichment
- Machine-learning-driven clustering

---

## Author Notes

This project is built as a **portfolio-grade analytics case study** demonstrating:
- Strong DAX fundamentals
- Analytical thinking
- Product sense
- Visual storytelling
- Real-world BI design standards

---

## Preview

![Spotify Power BI Dashboard – Overview](assets/overview.png)
![Artists Analysis Page](assets/artists.png)
![Songs Analysis Page](assets/songs.png)

> *(Screenshots can be added to the `/assets` folder and linked here.)*

---

## License

This project is for educational and portfolio purposes.  
Spotify is a registered trademark of Spotify AB. This dashboard is not affiliated with or endorsed by Spotify.
