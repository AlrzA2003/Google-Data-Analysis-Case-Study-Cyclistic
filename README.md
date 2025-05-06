# Cyclistic Trip Analysis  

Cyclistic Trip Analysis is a data-driven project designed to examine bike usage patterns among **casual riders** and **annual members**. Using historical trip data, this project uncovers key behavioral insights that help inform **membership conversion strategies** and operational decisions.  

## Table of Contents  
- [Project Overview](#project-overview)  
- [Dataset](#dataset)  
- [Tools and Technologies](#tools-and-technologies)  
- [Data Processing](#data-processing)  
- [Key Findings](#key-findings)  
- [Results Sharing](#results-sharing)  
- [Business Implications](#business-implications)  
- [License](#license)  

## Project Overview  

This project analyzes **Cyclistic’s bike trip data** to identify differences in riding patterns between casual users and annual members. The goal is to extract insights that inform **marketing strategies**, **service optimizations**, and **customer engagement efforts**. By leveraging data science techniques, we provide actionable recommendations to enhance **membership conversion** and improve service efficiency.  

## Dataset  

The dataset used in this analysis is sourced from **Motivate International Inc.**, a credible first-party provider. The trip data spans **March 2024 to February 2025** and includes details on ride duration, user type, timestamps, and geographic coordinates. The raw dataset was obtained from [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html), and further processed for consistency and integrity.  

Additional geographical data (**ward1998.zip**) containing coordinates for Chicago has been integrated for spatial analysis within `annual_trips_process.ipynb`.  

The **complete dataset** used for this analysis is available at the following link:  
[Download Full Dataset](https://1drv.ms/u/c/32ad82fef2c1dc75/EdGTQ3_iwKVBhXW6pcvI3kEBmfTw_ezzONdN95BlTMwvRQ?e=mTaDw4).  

## Tools and Technologies  

This project is built using the following tools:  
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)  
- **Jupyter Notebook** (`annual_trips_process.ipynb`, `annual_trips_analyze.ipynb`, `annual_trips_share.ipynb`)  
- **R Markdown** (`cyclistics-trips.Rmd`) – Contains the full **written analysis** in report format  
- **CSS** (for styling reports, `styles.css`)  
- **PowerPoint** (`Annual_Trips_Insights.pptx`) – Offers **a more visual representation** of key findings  
- **Tableau Public Dashboard** ([Cyclistic Trip Analysis](https://public.tableau.com/views/Book2_17462764518790/HowdoannualmembersandcasualridersuseCyclisticbikesdifferently?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link))  

## Data Processing  

### **Preprocessing (`annual_trips_process.ipynb`)**  
- Merging raw data into a **single dataset** for improved accessibility  
- Removing **duplicates** (211 records) and filtering out **erroneous data**  
- Creating **additional fields** for analysis:  
  - **ride_length** (duration of each trip)  
  - **day_of_week** (categorizing ride start days)  
  - **length_dif_secs** (time difference in seconds)  

### **Analysis (`annual_trips_analyze.ipynb`)**  
- **Descriptive statistics** on ride duration and frequency  
- **Patterns in peak riding times** (weekday vs. weekend comparisons)  
- **Differences in bike type preferences**  
- **Seasonality analysis** (Monthly usage variations)  

### **Sharing & Visualization (`annual_trips_share.ipynb`)**  
- Generating plots for ride distribution trends (`monthly_ride_distribution.png`, `monthly_ride_distribution_by_member.png`)  
- Creating an **interactive dashboard** in Tableau Public  

## Key Findings  

### **Ride Length Trends**  
Casual riders have **longer trips on average (23 min 41 sec)** compared to annual members (**12 min 17 sec**), suggesting they primarily use Cyclistic for leisure rather than commuting.  

### **Weekday vs. Weekend Usage**  
- Casual riders **peak on Thursdays–Saturdays**, with fewer trips early in the week.  
- Annual members **have fluctuations in ridership**, peaking on Tuesdays and declining on Fridays & Saturdays.  

### **Seasonal Variations**  
Casual ridership **spikes in warm months (May–September)**, whereas annual members maintain **steady engagement** year-round.  

## Results Sharing  

The insights generated have been shared through multiple platforms:  
- **PowerPoint Presentation** (`Annual_Trips_Insights.pptx`) – Provides a **clear, visual representation** of key findings with graphs and charts.  
- **R Markdown Report** (`cyclistics-trips.Rmd`) – Contains the full **detailed written analysis**, explaining methodology and findings in-depth.  
- **Tableau Public Dashboard** ([Interactive Insights](https://public.tableau.com/views/Book2_17462764518790/HowdoannualmembersandcasualridersuseCyclisticbikesdifferently?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)) – Allows for **interactive exploration** of trip patterns.  

## Business Implications  

The findings present several strategic recommendations:  
- **Membership Promotions:** Incentives during casual riders' peak demand periods (Thursdays–Saturdays) to encourage annual subscriptions.  
- **Seasonal Marketing Campaigns:** Emphasizing membership benefits during summer peaks to increase engagement.  
- **Flexible Membership Models:** Trial memberships for casual riders with long trip durations.  

## License  

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.  

