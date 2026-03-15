# Revenue_Forecasting_Performing_Arts_Setting
This repository contains work on ticket sales forecastability and forecasting for performing arts events.

## Contents

- `notebooks/01_AMI_Assessment.ipynb`  
  AMI-based assessment of booking-curve forecastability by tier.

- `notebooks/02_Ticket_Sales_Forecast.ipynb`  
  Forecasting workflow for ticket sales using features such as Tier, Order Days from Opening, and Days in Season.

## Main variables used

- Order Days from Opening
- Ticket Count
- Event
- Tier
- Days in season
- Venue_Capacity
- Season order
- SeasonMaxDay
## Project Structure

Revenue_Forecasting_Performing_Arts_Setting

├── notebooks  
│   ├── 01_AMI_Assessment.ipynb  
│   Forecastability analysis using Auto Mutual Information (AMI)  
│  
│   └── 02_Ticket_Sales_Forecast.ipynb  
│   Forecasting models for theatre ticket sales  
│
├── src  
│   Reusable Python functions for forecasting and analysis  
│
├── data  
│   Documentation of expected dataset structure (raw data not included)  
│
└── outputs  
    Generated figures and analysis outputs
## Workflow

1. Assess booking curve predictability using **AMI analysis**.
2. Use insights from forecastability diagnostics to design forecasting features.
3. Train forecasting models for ticket sales using booking curve features.
    
